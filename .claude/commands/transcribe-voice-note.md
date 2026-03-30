Transcribe a voice note using AssemblyAI, then apply the transcribed instructions as editing commands.

Steps:
1. Find the voice note file. If the user provides a path, use that. Otherwise, search the repo for recent audio files (mp3, wav, m4a, ogg, webm) and ask the user to confirm which one.
2. Source the API key: look for ASSEMBLYAI_API_KEY in `~/.api-keys/ai_services.env` or the environment. If not found, check `~/.bashrc`.
3. Upload the audio file to AssemblyAI:
   ```
   UPLOAD_URL=$(curl -s -X POST "https://api.assemblyai.com/v2/upload" \
     -H "Authorization: ${ASSEMBLYAI_API_KEY}" \
     --data-binary @"$AUDIO_FILE" | jq -r '.upload_url')
   ```
4. Request transcription:
   ```
   TRANSCRIPT_ID=$(curl -s -X POST "https://api.assemblyai.com/v2/transcript" \
     -H "Authorization: ${ASSEMBLYAI_API_KEY}" \
     -H "Content-Type: application/json" \
     -d "{\"audio_url\": \"${UPLOAD_URL}\"}" | jq -r '.id')
   ```
5. Poll for completion (check every 5 seconds):
   ```
   curl -s "https://api.assemblyai.com/v2/transcript/${TRANSCRIPT_ID}" \
     -H "Authorization: ${ASSEMBLYAI_API_KEY}" | jq -r '.status'
   ```
6. Once status is "completed", extract the text:
   ```
   curl -s "https://api.assemblyai.com/v2/transcript/${TRANSCRIPT_ID}" \
     -H "Authorization: ${ASSEMBLYAI_API_KEY}" | jq -r '.text'
   ```
7. Display the transcription to the user.
8. If the transcription contains editing instructions for the essay (e.g. "add a paragraph about...", "change the section on..."), ask the user if they'd like to apply those as a new iteration using the `/claude-version-iterator` workflow.
9. If the transcription is general content or notes, save it to a file in the repo and let the user decide what to do with it.

$ARGUMENTS
