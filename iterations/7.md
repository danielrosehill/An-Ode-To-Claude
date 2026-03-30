# On Why Claude Is Awesome

*Context: This started out as one of those things I post on X after coffee. Then it got too long so I started typing it in a notepad. V1: No-AI*

Claude Code is a masterpiece of software engineering:

Strip away the parts of technology that tend to break and cause compatibility problems (the UI) and you're left with the most basic primitive of computing - the terminal - and nothing other than a cursor standing in the way of frontier AI.

## Tearing Down the Moat

I've been using Linux for a long time - like 20 years long time.

But - *channeling the grumpy writer in me, which is never far beneath the surface, at least until I've had my morning coffee* - I've always bristled at some of the gatekeeping that goes on in technology.

Is one a "dev" or not? I mean, why should that even matter? And why is that so often held out as a yardstick?

We see this idea echoed all the time, in contexts that are subtle or less so. It has led to a massive fixation on "coding" - like coding bootcamps, that aim to condense what really takes years to master into days or weeks - that has often been nonsensical and myopic. Often, the obsession about mobilising a code-literate workforce has been spearheaded by those who have the least hands-on understanding of the change they are seeking to drive. Few seem to have predicted that the transformative differentiator may be leveraging non-sentient beings to write code rather than writing it themselves - or that the dawn of that era may be lurking right around the corner.

So that Claude Code is contributing to the undoing of a strange moat in tech is both fitting and ironic. Which is good because firewalling tech teams between "business" and "technical" users never really made a whole lot of operational sense. You don't need to know much code to admin a Linux server or do some pretty serious devops stuff. Many Python devs couldn't set up a load balancer to save their life. Backend devs probably aren't great at writing embedded software. And many sysadmins couldn't seat a stick of RAM or swap out a CPU cooler if their job depended on it (okay, I exaggerate a little).

Even limiting our conception of what's real technology to hardware is too restrictive. Without product and marketing people, your product mightn't sell and your Python devs would be fighting with the hardware guys over who gets to eat the last sandwich in the fridge. The roles matter less than the mission of different skillsets coming together to make the world better - a process in which technology, we tend to forget, will never be more than just a component.

It plays into a weird form of pointless elitism and gatekeeping that no longer needs to exist in a world in which AI agents are already generating a majority of code in production. Through its sheer proficiency in generating code, Claude Code has arguably made its own title obsolescent. Or at least expedited that process.

While Anthropic have rolled out Cowork as a friendlier "middle ground" Claude Code, I predict that the breaking down of the last vestiges of this tech moat will be the ultimate direction. Technology tends ultimately towards convergence and integration. This is part of Claude Code's appeal: give me one great tool and not ten blunt screwdrivers. The moat will be fully torn down once we accept that the things about technology development that seem offputting and scary - the repos, the terminals - are just best practices for digital work that can be applied and adopted across contexts.

## Beyond Code

Which is why I think that calling Claude Code Claude "Code" and marketing it primarily as dev tooling is actually an unnecessary constraint on its potential.

The non-code use-cases are too legion to list. But even a short enumeration can show some of their surprising diversity.

Claude can execute commands on the Linux terminal (or on Windows). You can connect it to a Jewish texts MCP ([Sefaria](https://www.sefaria.org/)) and pull in and typeset your own Pesach Haggadah. I've used it to typeset documents (with [Typst](https://typst.app/)); render videos; organise photos.

I've used Claude Code to cook up silly lyrics about carrot cakes that I then run through [Suno](https://suno.com/) and play to our son to try to get him to sleep. I've used it to edit videos programmatically with [MLT](https://www.mltframework.org/) and melt, normalise audio tracks, destem music, and install and configure tools I would never have figured out on my own.

I've also used Claude Code to create multi-agent orchestration projects - like Agent UN - that have allowed me to explore the frontiers of what agentic AI and synthetic personas could be used for. But some of the most meaningful applications have been deeply personal ones. I've used it to try to identify a diet that could work for me after digestive surgery - sifting through research, cross-referencing with my specific restrictions, and helping me feel less lost in a sea of conflicting nutritional advice. I've used it to summarise medical notes ahead of doctor's appointments, turning a stack of disorganised records into something coherent I could actually discuss. I've used it to plan out a monthly budget and make what usually feels like a scary, anxiety-inducing task feel manageable and structured.

And then there was the small claims case. I used Claude to gather and organise evidence against an intimidating and abusive landlord. That one was especially powerful. It felt like levelling the playing field - like having a tireless legal researcher in my corner who could help me build a coherent case from a mess of emails, photos, and receipts. The landlord even tried to weaponise AI against us, claiming that our photographic evidence was AI-generated. The irony was not lost on me.

I've also used Claude to create a dashboard that alerts me to when rocket alerts are happening across Israel. These tools exist, sure - but none fit my goldilocks requirements (I wanted to see volume-based alerting not just for my area). I estimate that Claude has personally created more than half of the tools that I regard as indispensable daily work drivers. I used it to build a transcription app, a personal repository manager, and an NFC reader/writer utility. I couldn't find one for my NFC reader so I got Claude to make one.

Claude has saved my home server by writing a superb backup utility and I even used it to probe the hardware and then spec out the most cost efficient upgrade path, pulling in context from local hardware suppliers, calculating the difference between local RRP and international prices to find the most reasonable deals, and then parsing the spec sheets to assure compatibility. This process took all of 30 minutes. It would otherwise have taken days. I could never have justified the time. And the savings from that project alone far exceeded the price of the monthly sub.

Unlike a software company, Claude doesn't have to think about whether it would be financially profitable to produce this software (it wouldn't). I don't have to beg for the time of developers or deal with annoyed project managers who want to know why I'm pulling their dev onto "just" website work (I've been there). I don't have to hide my curiosity from Claude or share my knowledge gaps. If I don't know what I'm doing, I ask Claude to break it down.

But this isn't just about cost savings - it's about something more fundamental. 

We are witnessing the dawn of personalised software. The idea of using software that somebody else has made for a mass market - accepting their compromises, their priorities, their idea of what you need - seems increasingly untenable and, frankly, a little ridiculous. Why should I settle for a one-size-fits-all tool when Claude can build me exactly the tool I need in thirty minutes? I predict this will be the future: a shift in software development from a centralised group of software companies producing for the masses to something radically decentralised, where software is generated directly for and by the end user. The democratising effect of this cannot be overstated. It levels a playing field that has been tilted for decades - not just between "technical" and "non-technical" people, but between those who could afford to commission custom software and those who had to make do with whatever was available.

Many of the most fulfilling applications I've found for Claude are in the realm of systems administration. You could say that I've "pioneered" the idea of what I call a [Claude Space](https://claude.danielrosehill.com/ideas/claude-spaces/) - essentially using a repo as a launching pad for Claude to work on an ongoing project: like, say, optimising a Home Assistant setup. The idea is simple but powerful: the repository *is* the application. No build step, no deployment. You clone a repo, open Claude Code, and you have a pre-configured workspace for a specific domain - budgeting, sysadmin, legal research, writing, whatever you need. I think it's one of the most neglected ideas in the Claude Code ecosystem and I continue to be surprised that more people haven't run with it.

I use Claude constantly to fix things on my computer. Or - if I'm being honest - just because saying "hey, could you clean up my desktop - delete the images and working data" is easier than right clicking and moving stuff into the bin.

## The Terminal Paradox

Claude Code is also a paradox. In an era in which AI has never been more powerful, we have reverted to .... a terminal to use it.

There's something humbling, too, about building a good CLI in 2026. Anyone can build a flashy GUI. But often flashy GUIs mask buggy and poorly QA-ed products. In software, the GUI - the windows that make computers easy to use - are often the most brittle part of the tool.

It's not that good UI isn't vital (I'm a huge advocate for it and it receives way too little attention). But Claude Code directs its energy, and focuses its value, on the parts of the tool that actually make a transformative difference: the functions themselves. Other than a weird blob-like mascot, it offers no flashier UI than a white blinking cursor set against a terminal. By living just on top of the execution layer, Claude Code gets you straight under the hood. The visual layers that extend it past the purely command level layer - like browser use - are nice-to-have. But the future of agentic on computer is almost certainly going to happen at the cleaner level at which Claude Code natively lives.

I have ADHD, something I make no secret of. Claude is becoming a powerful ally. I'll use it to do things that would ordinarily make my brain scream "STRESS!" like planning a weekly schedule. But the UI - this is my contention, at least - is actually highly accommodating to ADHDers. Cluttered UIs are my pet peeve. And even though I've been using Linux for a long time, I always felt that using CLIs "just because" made little sense. Who has the mental bandwidth to keep a million parameters in their head? Claude is the first CLI I've used that I like so much that I've memorised the operators without expending any effort to do so.

These feel like the most natural and logical applications to me. Such that using Claude Code in repositories sometimes feels like I'm pushing it into places it shouldn't go. While I understand why it exists, and why it has to in many contexts, the sandboxing and constant safety prompts actually make little sense to me: I want Claude to be fluid and I'm fine with it occasionally breaking things. If I wasn't, I wouldn't be using it.

## Reliability Over Brilliance

During the course of the year I've been using Claude Code - every single day - I've watched it grow up. The biggest transformation I've seen has been the jump to 4.6. The change: Claude became reliably good. Way too much conversation in agentic AI goes into the very blurry concept of AGI and increasing raw reasoning power.

From my perspective: give me reliability any day over PhD-level intelligence. 4.5 was great but often introduced regressions - it would fix one thing and break another, or nail a complex task and then fumble something simple. 4.6 was the Rubicon for me because it's the first AI tool I can trust to reliably get things right. That is what's much more huge than the occasional flashes of brilliance. Consistent competence beats sporadic genius every time.

## Making Agentic AI Approachable

Claude Code has done another great service to the world of AI: it's made agentic AI approachable enough that it's not too difficult to begin actually experimenting with it.

I've made the point before that agentic AI is insanely backend-heavy. Telegram Bots - while endearing and functional - are not production-level tools for interfacing with AI agents. That they are accepted as an almost default way of talking to backends is telling.

The reason might be that for the frontend to be useful you need to stand up an agentic backend which is a very complicated and multifaceted task once you begin breaking out what sounds like a simple proposition ("just get AI to do things").

I'm convinced that a huge driver of the discourse around the "confusion" about agentic AI is because just defining agentic AI by reference to its essential quality - that it *does* things - is actually far too non-specific. By this definition, ChatGPT with an MCP connection has as much right to be called an agent as does an enterprise workflow that features an AI parser but which will never be directly interacted with by even a single user.

But before building out sprawling workflows in Python - or in N8N - we need a safe place to try out those ideas. Agentic frameworks tend to be either code-first - defining a multiagent architecture from code is a big barrier to entry - or low-code solutions that free you from code but also add so much vendor lock-in that you've now got a scale constraint. They also tend to be ... a very unsatisfying experience.

Claude Code provides a compelling middle ground that was for too long simply absent. The framework gets criticised for relying heavily upon globs of markdown documents - hey, aren't skills just a cluster of MD files?! - but praised for that same decision very rarely. By standardising core parts of its harness on markdown, Claude Code means that essentially anybody can begin seeing how natural language can create compelling technology solutions that can be built with AI even if they ultimately don't use them.

There's a common worry that tools like Claude Code will degrade technical skills - that if AI writes the code, people will stop learning how it works. I've found the opposite to be true. Claude Code has been one of the most powerful motivators I've encountered to learn *more* about technology. I'm more motivated to understand coding than I have ever been, even if I don't envision myself doing much of the actual writing. When Claude builds something for me, I want to understand what it built and why. The use case I think of as "do and then teach" - where Claude executes a task and then walks you through what it did, what the code means, and asks if you have any questions - is going to be huge. It's a mode of learning that barely exists yet but feels like one of the most natural applications of agentic AI: not replacing the human's understanding, but building it up through doing real work together.

## Words Are My Code

Words are my code. That natural language has become a bridge towards configuring technology is the part of the AI revolution that continues to make me smile. It feels like two parts of what I love that never found a way to get along and were always told that they were mutually exclusive can now jive off one another. Claude is the magic that makes the connection.

I stubbornly resist Grammarly because in its obsessive desire to enforce grammar, it tends to lose those deliberately ungrammatical sentences that make playing with language fun. Claude, however, has my full confidence. Even as an AI enthusiast, as a writer and as a creative - it takes quite a bit of trust to feel comfortable in letting anything overwrite me.

After writing this, I'll ask Claude to fix my typos - effectively turning it into a spellcheck (I'll carefully preserve the original). I've used it to clean data and.... the list could go on. Claude helps with just about anything. I could ask Claude to then do some more extensive edits and when I feel like it's ready to be shared use the Contentful MCP to push it up to my blog (or use a newsletter MCP to bounce it over to friends).

Before Claude, I would have squirmed at the thought of paying $200 a month for a subscription. But in a world where even the cost of bread and cheese has become non-trivial, and SaaS that overpromises and underdelivers has become the norm, Claude has slashed so many expenses and created so much value that that feels like a genuine bargain. I feel like I could probably end my phone contract if I really wanted to. Claude would probably coach me through how to do it and then code a PBX before I had time to locate my last invoice.

Their marketing: "to do - everything" is one of the very best marketing slogans I've ever seen. It's simple, effective, and describes the product well. And great technology marketing slogans aren't a dime a dozen.

Claude Code is the only technology product I can ever say I have found addictive - but in the best possible way. It makes every flash of what seemed like brilliance you've had seem only a few minutes away.

I prototype and experiment with it at a pace that is sometimes furious. This is my anxiety at work. I assume that at some point Claude may be taken away - perhaps that $200 will be $1000 a month! As a father, if I can find a block of time to advance some open source projects, I seize it. Claude gets straight to task.

Sometimes Claude is so good at everything that I can just turn off the computer and go out and do other things. This is the promise of AI: that it will make technology help us to live more efficient lives. It is not to make more technology. Meeting this bar is not easy. Claude Code is one of the few products that can truly lay claim to having reached that threshold. At least in my view.

Happy first birthday, Claude Code! It's been a wild ride so far. You've put up with my sometimes dreadful prompting. Helped expand upon my weird ideas. Improved my life. And changed my workday: I start each morning with at least a mild jolt of optimism about what fun new things can be cooked up today. I can't wait to see what the next iterations bring!

---

*For a fuller picture of what Claude Code can do beyond coding, see my [Claude Code Projects Index](https://github.com/danielrosehill/Claude-Code-Projects-Index) and [claude.danielrosehill.com](https://claude.danielrosehill.com/).*