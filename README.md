## Hi, I'm Sanjey

I'm a first year student at Wilfrid Laurier, doing a double degree in Computer Science and Business Administration. I'm also a Growth Engineering Intern at [Magic Hour](https://magichour.ai) (YC W24), and an Expert on [Codeforces](https://codeforces.com/profile/SS28).

I like making what comes to my head.

## Projects

### [Faultline](https://github.com/1SS28/faultline)

Crash tests for AI agents. Faultline breaks a tool call partway through, like a refund that goes through but times out before the agent hears back, and then checks what actually happened on the other side. In the demo, a naive agent retries and refunds $258 on a $129 order, while one with a stable idempotency key refunds exactly once. Each failure it finds becomes a regression test you can run in CI.

`TypeScript` `Node.js` `PostgreSQL` `React`

### [GeoDashML](https://github.com/1SS28/GeoDashML)

Teaching an RL agent to play Geometry Dash. I wrote a C++ mod that freezes the game and steps it one 240 Hz physics tick at a time, so Python can drive it as a Gymnasium environment. A search bot beats Stereo Madness in 3,956 attempts, and a PPO agent trained backwards from that run has now beaten it too, after 183,634 attempts. The lab notebook has every bug I hit along the way, a few of them in the game itself.

`C++` `Geode` `Python` `PyTorch` `Gymnasium`

### [Climbing Beta](https://github.com/1SS28/climbing-beta)

Point it at a bouldering wall and it finds the holds, sorts them into routes by colour, and works out a sequence of moves. The hold detector is YOLO11 fine-tuned on about 6,000 holds. PyTorch was too big to deploy, so the [phone app](https://climbing-beta-theta.vercel.app) runs the model in your browser with ONNX and WebGPU, and your photo never gets uploaded.

`Python` `YOLO11` `ONNX` `WebGPU`

### [Triangulate](https://github.com/1SS28/Triangulate)

Rebuilds an image out of overlapping triangles with no ML and no graphics libraries, just C++ and least squares. I mostly made it because I like geometry.

`C++`

## At Magic Hour

Open-source apps I've built on Magic Hour's API as part of my internship.

- **[pod2video](https://github.com/1SS28/pod2video)** turns an audio podcast into vertical clips where the host lip-syncs to their real voice, for about $0.60 to $0.90 a clip. The [template repo](https://github.com/1SS28/pod2video-template) runs it on GitHub Actions: each new episode opens an issue with free previews, and you comment `/render 2 5` to get those clips.
- **[Autonomous Listing Agent](https://github.com/1SS28/autonomous-listing-agent)**: text a product photo to a Telegram bot and it comes back as a live eBay listing. I wrote its three MCP servers (eBay, Etsy and file transfer), OAuth flows included. Etsy gets as far as a finished draft.
- **[GitHub Wrapped](https://github.com/1SS28/github-wrapped)** turns your year on GitHub into a 60-second video, with a narrator who roasts your commit habits. Still in progress, but it runs end to end. ([website](https://github-wrapped-2026.vercel.app))

## Smaller things

- [FilingDiff](https://github.com/1SS28/FilingDiff) pulls and validates a company's latest 10-Q filings from SEC EDGAR. The comparison part isn't built yet.
- [Stitch Taskbar Buddy](https://github.com/1SS28/Stitch_Taskbar_Buddy) is an animated Stitch that sits above the taskbar and gets sleepy at night. It was my first Electron app, made as a gift.

## Contact

- Email: sanjeyselvendra8@gmail.com
- [LinkedIn](https://www.linkedin.com/in/sanjey-selvendra-581626326/)
