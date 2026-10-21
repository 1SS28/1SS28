## Hi, I'm Sanjey

I'm in first year at Wilfrid Laurier, doing a double degree in Computer Science and Business Administration. Outside of class I do competitive programming ([Expert on Codeforces](https://codeforces.com/profile/SS28)) and spend a lot of time on math and finance.

I'm also an API Growth Intern at [Magic Hour](https://magichour.ai) (YC W24), where I build open-source apps on top of their API.

I like projects that make me learn something I don't know yet: a new API, a weird file format, a game's internals. Most of what's below started that way.

## Projects

### [GeoDashML](https://github.com/1SS28/GeoDashML)

Can a reinforcement learning agent learn to beat a Geometry Dash level, and how many attempts does it need compared to a person? I wrote a C++ mod that freezes the game and steps it one 240 Hz physics tick at a time over a socket, so Python can drive it like a Gymnasium environment. A search bot clears Stereo Madness in 3,956 attempts, and I'm now training a PPO agent on a curriculum built from that run. The lab notebook in the repo has every bug I ran into, including a few in the game itself.

`C++` `Geode` `Python` `PyTorch` `Gymnasium`

### [Climbing Beta](https://github.com/1SS28/climbing-beta)

Take a photo of a bouldering wall and it finds the holds, groups them into routes by colour, and searches for a sequence of moves up the route. The detector is YOLO11 fine-tuned on about 6,000 holds. PyTorch was too big to deploy, so the [phone app](https://climbing-beta-theta.vercel.app) runs the model in your browser through ONNX and WebGPU, and your photo never gets uploaded.

`Python` `YOLO11` `ONNX` `WebGPU`

### [pod2video](https://github.com/1SS28/pod2video)

Turns an audio-only podcast into vertical clips where the host on screen lip-syncs to their real voice. It picks the best moments, shows you free previews, and only renders the ones you choose, at about $0.60 to $0.90 a clip. If you don't want to install anything, the [template repo](https://github.com/1SS28/pod2video-template) runs it on GitHub Actions: each new episode opens an issue with previews, and you comment `/render 2 5` to get those clips.

`Python` `Magic Hour API` `GitHub Actions` `ffmpeg`

### [Autonomous Listing Agent](https://github.com/1SS28/autonomous-listing-agent)

Text a product photo to a Telegram bot and it comes back as a live eBay listing, with cleaned-up product shots from Magic Hour. Etsy works up to a finished draft. I wrote the three MCP servers the agent uses (eBay, Etsy, and file transfer), including the OAuth flows for both marketplaces.

`Node.js` `MCP` `OAuth 2.0` `Cloudflare Workers`

### [Triangulate](https://github.com/1SS28/Triangulate)

Rebuilds an image out of overlapping triangles. There's no ML and no graphics library, just C++ and some least squares. I mostly made it because I like geometry.

`C++`

### [GitHub Wrapped](https://github.com/1SS28/github-wrapped)

Your year on GitHub as a 60-second video, with a narrator who roasts your commit habits. Still a work in progress, but it runs end to end. [Website](https://github-wrapped-2026.vercel.app)

`Python` `Magic Hour API` `ffmpeg`

### Smaller things

- [FilingDiff](https://github.com/1SS28/FilingDiff): pulls and validates a company's latest 10-Q filings from SEC EDGAR. The comparison part isn't built yet.
- [Stitch Taskbar Buddy](https://github.com/1SS28/Stitch_Taskbar_Buddy): an animated Stitch that sits above the taskbar and gets sleepy at night. My first Electron app, made as a gift.

## Contact

- Email: sanjeyselvendra8@gmail.com
- [LinkedIn](https://www.linkedin.com/in/sanjey-selvendra-581626326/)
