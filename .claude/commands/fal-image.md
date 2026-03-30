Generate images using fal.ai's Nano Banana 2 model and save them to the `images/` directory.

Steps:
1. Parse the user's instructions below for: prompt description, aspect ratio preference, and number of images.
2. If no aspect ratio is specified, default to `16:9`. Available ratios: auto, 21:9, 16:9, 3:2, 4:3, 5:4, 1:1, 4:5, 3:4, 2:3, 9:16, 4:1, 1:4, 8:1, 1:8.
3. If no resolution is specified, default to `1K`. Options: 0.5K, 1K, 2K, 4K.
4. Enhance the user's prompt to be more descriptive and detailed for better image generation results, while preserving their intent. Add style cues, lighting, composition details. Show the enhanced prompt to the user before generating.
5. Source the FAL API key: `source /home/daniel/.api-keys/ai_services.env`
6. Generate each image using curl:
   ```
   curl -s -X POST "https://fal.run/fal-ai/nano-banana-2" \
     -H "Authorization: Key ${FAL_KEY}" \
     -H "Content-Type: application/json" \
     -d '{"prompt": "...", "aspect_ratio": "...", "resolution": "...", "output_format": "png"}'
   ```
7. Extract the image URL from the response using `jq -r '.images[0].url'`.
8. Download each image to the `images/` directory with a descriptive filename (kebab-case, numbered sequentially based on existing files).
9. Display each downloaded image to the user using the Read tool so they can review it.
10. If the user is unhappy with a result, offer to regenerate with an adjusted prompt.

Pricing reference (so the user knows): $0.08/image at 1K, $0.06 at 0.5K, $0.12 at 2K, $0.16 at 4K. Web search adds $0.015.

$ARGUMENTS
