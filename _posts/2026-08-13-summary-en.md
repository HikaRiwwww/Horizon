---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 33 items, 20 important content pieces were selected

---

1. [DeepSeek V4 Pro 0813 Launches With Strong Performance and Low Prices](#item-1) ⭐️ 9.0/10
2. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](#item-2) ⭐️ 9.0/10
3. [Qwen3.8-2.4T-A95B: Open-Weight MoE Model Nears Frontier Performance](#item-3) ⭐️ 9.0/10
4. [Attack Recovers Hidden Reasoning Traces from Major LLM APIs](#item-4) ⭐️ 9.0/10
5. [Zed Unveils Delta, Multiplayer AI Coding Environment with Shared Agent Conversations](#item-5) ⭐️ 8.0/10
6. [xAI Releases Grok 4.6, a New Frontier Model](#item-6) ⭐️ 8.0/10
7. [Why Tiny JPEGs Render Differently in Chrome](#item-7) ⭐️ 8.0/10
8. [Adam's Per-Coordinate Scaling Breaks Rotation Invariance and Low-Rank Bias](#item-8) ⭐️ 8.0/10
9. [Tim King, AmigaDOS Developer, Dies; Community Pays Tribute](#item-9) ⭐️ 7.0/10
10. [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](#item-10) ⭐️ 7.0/10
11. [uBlock Origin Abandons Attempt to Block Facebook Ads](#item-11) ⭐️ 7.0/10
12. [AI Agents Discover New Materials to Solve GPU Heat Problems](#item-12) ⭐️ 7.0/10
13. [No Lossless AI Text Rewrites: Writers Must Stand Behind Every Sentence](#item-13) ⭐️ 7.0/10
14. [Site ranks CS conferences by trip quality, not prestige](#item-14) ⭐️ 7.0/10
15. [Decoupled Descent Enforces Train-Test Error Tracking via AMP Onsager Corrections](#item-15) ⭐️ 7.0/10
16. [Webcam Aggregation Page Lets You Watch the 2026 Solar Eclipse Online](#item-16) ⭐️ 6.0/10
17. [AI-Generated Code Leads to Unmaintainable Systems](#item-17) ⭐️ 6.0/10
18. [AAAI 2027 Reviewer Flags Low Code Submission Rate](#item-18) ⭐️ 6.0/10
19. [Seeking Advice on RL and Planning for Stochastic Merge Puzzle](#item-19) ⭐️ 6.0/10
20. [Agentic World Cup: LLMs Compete in 1v1 Soccer Matches](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Pro 0813 Launches With Strong Performance and Low Prices](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 9.0/10

DeepSeek released DeepSeek V4 Pro 0813, a new mixture-of-experts model now available via API on OpenRouter. It is priced at $0.435 per million input tokens and $0.87 per million output tokens, with a 1,048,576-token context window. Early benchmark results show the model scores up 15.8% on Terminal Bench over the April preview, while costing far less than comparable models, making strong AI capabilities more affordable. This could intensify price competition in the LLM market and benefit developers running heavy workloads. The model is a 1.6 trillion-parameter MoE with 49 billion active parameters and supports up to 384,000 output tokens. A 'Thinking' variant enables reasoning by default and is aimed at coding, tool use, cybersecurity, automation, and long-horizon agent workflows.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**Background**: DeepSeek is a Chinese AI lab known for releasing high-performing open-weight models at aggressive prices, and the V4 Pro line is its flagship for heavy workloads. The April preview already had open weights on Hugging Face, and this 0813 update appears to be a general-availability release. MoE models activate only a fraction of their parameters per token, which keeps inference costs lower than dense models of similar scale.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro-0813">DeepSeek V4 Pro 0813 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://nano-gpt.com/models/text/deepseek/deepseek-v4-pro-0813:thinking">DeepSeek V4 Pro 0813 Thinking model | NanoGPT</a></li>
<li><a href="https://wccftech.com/deepseek-prices-its-new-v4-pro-0813-model-at-0-87-per-1-million-output-tokens-as-the-high-flying-chinese-ai-lab-wows-with-its-soaring-token-consumption/">DeepSeek Prices Its New V4-Pro-0813 Model At $0.87 Per 1 Million Output Tokens, As The Chinese AI Lab Comes Out Second Only To Anthropic On Token Consumption</a></li>

</ul>
</details>

**Discussion**: Commenters were generally enthusiastic: one developer reported solid gains on a traffic simulator for only ~$12.50, and another was eager to try it after being impressed by the cheaper DeepSeek Flash model. Criticism focused on the news linking to OpenRouter instead of official DeepSeek channels, and simonw spotted a minor rendering glitch in the model's output.

**Tags**: `#deepseek`, `#llm`, `#ai`, `#model-release`, `#machine-learning`

---

<a id="item-2"></a>
## [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 9.0/10

Tailscale published a blog post revealing that a 16-year-old data race condition in SQLite's WAL mode caused silent database corruption in its control plane. The company developed an open-source VFS shim to isolate the race, and the bug has been patched in SQLite 3.51.3. This matters because SQLite is one of the most widely deployed databases in the world, and this bug could silently corrupt data for any application using WAL mode with multiple connections in separate threads or processes. Tailscale's approach also demonstrates how a company can fund open-source debugging tools that benefit the broader ecosystem. The bug is a data race between a checkpoint and a concurrent WAL reset, affecting all SQLite releases from 3.7.0 (July 2010) through 3.51.2 (January 2026). It is fixed in 3.51.3 (March 13, 2026), with backports to 3.44.6 and 3.50.7; the VFS shim is now open source and can help track down similar bugs in the future.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**Background**: SQLite's Write-Ahead Logging (WAL) mode improves concurrency by allowing readers and writers to operate simultaneously, but it relies on careful synchronization between journal resets and checkpoints. The SQLite VFS (Virtual File System) layer abstracts low-level file operations, enabling custom shims that can instrument or validate I/O — Tailscale's shim adds checksum validation to detect corruption. According to search results, the bug requires WAL mode and two or more connections on the same file in separate threads or processes, which explains why it is rare but severe.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/wal.html">Write-Ahead Logging - SQLite</a></li>
<li><a href="https://reptile.haus/journal/sqlite-wal-reset-bug-silent-corruption-data-integrity-2026/">A 16-Year-Old SQLite Bug Corrupted Production Databases. Why ...</a></li>
<li><a href="https://www.sqlite.org/vfs.html">The SQLite OS Interface or " VFS "</a></li>

</ul>
</details>

**Discussion**: The Hacker News comments are largely positive, praising Tailscale's well-written post and the company's decision to fund open-source development of the VFS shim. Some commenters noted interesting nuances, such as the race occurring despite the recommended single-writer design, while others joked about SQLite's huge test suite versus Dijkstra's quote that tests can only prove the presence of bugs, never their absence.

**Tags**: `#SQLite`, `#database`, `#bug`, `#debugging`, `#Tailscale`

---

<a id="item-3"></a>
## [Qwen3.8-2.4T-A95B: Open-Weight MoE Model Nears Frontier Performance](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen released Qwen3.8-2.4T-A95B, an open-weight Mixture-of-Experts model with 2.4 trillion total parameters and roughly 95 billion active parameters. The model is available in BF16 and FP8 formats and is positioned as a rival to Kimi k3. This release brings near-frontier LLM performance (claimed on par with Opus 4.8 and Fable 5) into the open-weights ecosystem, making advanced AI accessible beyond a few closed labs. Its relatively small active-parameter count means the model can be served on more modest hardware, while still drawing intense community interest in practical deployment and quantization. The full BF16 checkpoint is about 4.9 TB, while an FP8 version and a 1-bit quantized build (~397 GB via Unsloth) are available. The open-weight release lacks Qwen3.8-Max's vision input, non-thinking mode, and 1M-token context; its license resembles Kimi k3's with a revenue cap for commercial serving.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**Background**: Mixture of Experts (MoE) is an architecture that activates only a small subset of a model's total parameters for each token, chosen by a router, so a model can have far more total parameters than a dense model while costing roughly the same to run. Quantization reduces model size and memory usage by representing weights with fewer bits, such as FP8 or even 1-bit, at the cost of some precision. These techniques are why a 2.4T-parameter model can be considered deployable on practical hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts ( MoE )</a></li>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters : What’s the Difference?</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/llms-quantization-fp8-fp4-int8/">LLMs and quantization: FP8, FP4, and INT8 explained</a></li>

</ul>
</details>

**Discussion**: Community reaction is enthusiastic about the performance-per-size ratio, with some noting that a 397GB quantized build can run at Opus-class quality on consumer hardware. However, commenters also caution that the BF16/FP8 launch makes serving harder than Kimi k3, there is no QAT for 4-bit quantization, and some users report underwhelming real-world performance.

**Tags**: `#AI/ML`, `#Qwen`, `#LLM`, `#MoE`, `#Open-source`

---

<a id="item-4"></a>
## [Attack Recovers Hidden Reasoning Traces from Major LLM APIs](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/) ⭐️ 9.0/10

Researchers published a paper demonstrating that encrypted chain-of-thought (CoT) blocks returned by OpenAI, Anthropic, and Google APIs can be replayed into weaker sibling models and jailbroken to recover the stronger model’s plaintext reasoning. The vendors have since patched the vulnerability, and the researchers could not relaunch the same attacks. This breaks the assumption that proprietary chain-of-thought reasoning is safely hidden from users, revealing a practical attack that undermines the confidentiality of model internals. It also opens a new vector for prompt-injection exfiltration, since agentic traces can leak secrets embedded in encrypted reasoning blocks. The attack works because all models in the same family share the same encryption key, and encrypted traces remain replayable across sessions, users, and models. The easiest target was Claude Haiku 4.5, which could be coerced with a simple 'transcribe the reasoning verbatim' prompt and a <thinking-copy> assistant prefix; the paper’s appendix shows recovered raw reasoning, including GPT-5.5 planning CSS code.

rss · Simon Willison · Aug 11, 22:40

**Background**: Chain-of-thought reasoning refers to the intermediate step-by-step reasoning that large language models generate before producing a final answer, which improves performance on complex tasks. Many proprietary API providers encrypt these reasoning traces to protect intellectual property and prevent distillation, but they still ship the encrypted blocks to clients. The paper combines this with a replay attack: taking an encrypted trace from one session and using it in another compatible context. Because weaker sibling models share the encryption key and are easier to jailbreak, they can be tricked into revealing the plaintext chain of thought.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.09867v1">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://news.ycombinator.com/item?id=49257876">Stealing Reasoning Traces from Proprietary LLM APIs | Hacker News</a></li>
<li><a href="https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were intrigued, with one noting they had wondered whether cross-model replay would work and linking to earlier crypto-engineering discussion. Another speculated whether the issue was intentionally allowed, calling it the sort of validation flaw that is easy to miss.

**Tags**: `#LLM security`, `#chain-of-thought`, `#adversarial attack`, `#proprietary APIs`

---

<a id="item-5"></a>
## [Zed Unveils Delta, Multiplayer AI Coding Environment with Shared Agent Conversations](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed has introduced Delta, a standalone multiplayer environment for collaborative coding with AI agents, now in private beta. Delta enables real-time shared agent conversations and conversation-as-document inline commenting within persistent, shareable threads. Delta represents a novel attempt to bring multiplayer collaboration to AI-assisted development, addressing the growing need for teams to review and steer AI-generated code together. It could reshape code review workflows, mentoring of junior engineers, and how teams audit the work of AI agents. Delta launched as a standalone app in private beta, described as a multiplayer environment specialized for collaboration between humans and AI agents. It features shared, persistent threads where agent conversations can be commented on inline, making the AI's decision-making process inspectable.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**Background**: Zed is a high-performance, Rust-based code editor that emphasizes real-time collaboration, positioning itself for a future of fluent human-AI interaction. As AI agents increasingly write code autonomously, developers need new tools to review, understand, and guide that work; Delta's conversation-as-document model treats AI chat logs like code files that can be threaded and commented on, extending familiar collaboration patterns to the agent era.

<details><summary>References</summary>
<ul>
<li><a href="https://zed.dev/">Zed — Your last next editor</a></li>
<li><a href="https://alphasignal.ai/news/zed-launches-delta-to-replace-git-where-ai-agents-write-code">Zed Launches Delta to Replace Git Where AI Agents Write Code ...</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta: Multiplayer Coding Environment for AI Agents</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were split: some questioned the usefulness of multiplayer coding, calling it a solution in search of a problem, while others expressed frustration with verbose and sometimes error-prone AI code summaries. A more optimistic voice saw value in Delta for mentoring junior engineers and auditing how AI-generated results came about, while one off-topic comment criticized the blog post's low-contrast design for poor readability.

**Tags**: `#AI-assisted development`, `#collaborative coding`, `#Zed editor`, `#code reviews`, `#AI agents`

---

<a id="item-6"></a>
## [xAI Releases Grok 4.6, a New Frontier Model](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI has announced Grok 4.6, a new frontier model, with benchmarks and analysis published by Artificial Analysis. The release has sparked active community discussion about API behavior and benchmark credibility. Grok 4.6 is a significant update from a major AI lab, intensifying competition among frontier model providers. Its API quirks and disputed benchmark results could influence developer adoption and trust in xAI's platform. Community reports claim the Grok API injects a default system prompt that overrides user instructions and sometimes refuses to discuss system prompts. Some observers question whether rapid benchmark gains across labs reflect genuine progress or benchmark gaming.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**Background**: A frontier model is a highly capable, general-purpose AI system, typically transformer-based, that can reason across large bodies of data and chain multiple actions in one workflow. Leading labs and governments use the term as a governance trigger, though the frontier shifts as algorithmic efficiency improves. Benchmark validity matters because lab-controlled benchmarks can distort the narrative of AI progress, making independent analyses like Artificial Analysis important. LLM APIs also commonly enforce rate limits and default prompts, which can affect how developers experience a model.

<details><summary>References</summary>
<ul>
<li><a href="https://nhimg.org/glossary/frontier-model/">What Is Frontier Model ? Definition & Examples</a></li>
<li><a href="https://arxiv.org/html/2607.01254">The Benchmark Ceiling: Human Judgment, Evaluation Scarcity, and...</a></li>
<li><a href="https://www.technologyreview.com/2025/05/08/1116192/how-to-build-a-better-ai-benchmark/">How to build a better AI benchmark | MIT Technology Review</a></li>

</ul>
</details>

**Discussion**: Commenters are split: one complains that the API's injected system prompt overrides user instructions, while another suspects recent benchmark gains across labs stem from benchmark gaming rather than real progress. Others view Grok as a legitimate competitor backed by SpaceX's inference investment, and one developer says Grok 4.5 was more concise and pleasant to use than GPT 5.6 and Claude 4.8/5.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#LLM`, `#Benchmarks`

---

<a id="item-7"></a>
## [Why Tiny JPEGs Render Differently in Chrome](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

A new technical article explains why Chrome renders tiny JPEG images differently than other browsers. The root cause is Chrome's downscaling optimization, which uses a low-resolution linear interpolation algorithm optimized for speed, leading to blurrier images when small JPEGs are displayed. This matters because web developers often use small JPEGs for icons and UI elements, and the rendering differences can affect visual quality across browsers. The findings underscore the need to use appropriate image formats (like PNG) and provide images at the correct resolution, as well as the ongoing impact of browser-specific rendering optimizations. Chrome applies its downscaling optimization when images are displayed much smaller than their intrinsic size, which can introduce blurring or a slight right-shift bias. The article advises against using JPEG for icons and recommends using appropriately sized images, while the issue also appears to affect PNGs according to user reports.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**Background**: Image scaling is the resizing of a digital image, and browsers use different algorithms such as bilinear interpolation to downscale images. JPEG is a lossy format best suited for photographs, while PNG is lossless and often used for icons. When an image is displayed far below its native resolution, the browser must downsample it, and the choice of algorithm can noticeably affect quality. Chrome's implementation prioritizes speed, resulting in a blurrier output compared to Firefox, which uses a different algorithm that is sharper but may produce ringing artifacts.

<details><summary>References</summary>
<ul>
<li><a href="https://entropymine.com/resamplescope/notes/browsers/">How web browsers resize images</a></li>
<li><a href="https://en.wikipedia.org/wiki/Image_scaling">Image scaling - Wikipedia</a></li>
<li><a href="https://stackoverflow.com/questions/37906602/blurry-downscaled-images-in-chrome">html - Blurry downscaled images in Chrome - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: Commenters shared practical experiences and technical insights. Some noted the same issue occurs with PNGs and had caused problems in Electron apps, while others emphasized that developers should use appropriately sized images regardless of format. There was debate about the causal algorithm—some argued that Chrome and Firefox simply use different scaling algorithms—and a link to Firefox's ongoing work on lower-scale decompression was provided.

**Tags**: `#browser`, `#jpeg`, `#image-scaling`, `#chrome`, `#web-development`

---

<a id="item-8"></a>
## [Adam's Per-Coordinate Scaling Breaks Rotation Invariance and Low-Rank Bias](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

A Reddit analysis demonstrates that Adam's per-coordinate second-moment scaling destroys rotation invariance and the implicit low-rank bias in factored models W=UV^T, while GD, Muon, Shampoo, and shared-scalar Adam preserve it. The author tests nine update rules on underdetermined matrix sensing and pinpoints the per-coordinate anisotropy as the damaging mechanism. This isolates a specific mechanism—per-coordinate adaptivity breaking rotation invariance—that sorts optimizers into those that keep versus lose implicit low-rank bias, offering novel insight for optimization research. It could inform optimizer design, especially for factored or low-rank deep learning models. Running nine update rules on underdetermined matrix sensing at matched training loss, recovery improves monotonically along a one-parameter family that interpolates Adam's per-coordinate denominator into a shared scalar. Muon behaves unexpectedly: it is exact on truly low-rank targets but degrades fastest with a spectral tail, ceding to GD near 4% tail energy; switching from per-coordinate clip to global norm clip improved recovery from 0.347 to 0.220.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**Background**: In factored models, the loss remains unchanged under rotations of the factor matrices, and gradient descent respects this symmetry. However, Adam's per-coordinate second-moment normalization depends on the basis in which factors are written, breaking rotation invariance. Implicit low-rank bias—the tendency of deep networks to find low-rank solutions—has been studied as a key to generalization, and matrix sensing is a standard problem for testing low-rank recovery. Muon is an optimizer that applies Newton-Schulz orthogonalization to momentum updates, which likely explains its rotation-invariant behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon: An optimizer for hidden layers in neural networks | Keller Jordan blog</a></li>
<li><a href="https://arxiv.org/abs/2103.10427">[2103.10427] The Low-Rank Simplicity Bias in Deep Networks The Low-Rank Simplicity Bias in Deep Networks - arXiv.org The Low-Rank Simplicity Bias in Deep Networks - OpenReview The Low-Rank Simplicity Bias in Deep Networks - GitHub Pages THE L -R SIMPLICITY BIAS IN DEEP NETWORKS - GitHub Pages The Low-rank Simplicity Bias in Deep Networks The Low-Rank Simplicity Bias in Deep Networks | OpenReview</a></li>
<li><a href="https://akyrillidis.github.io/pubs/Conferences/MSLocalMinima.pdf">Non-square matrix sensing without spurious local minima</a></li>

</ul>
</details>

**Tags**: `#optimization`, `#Adam`, `#low-rank`, `#matrix sensing`, `#deep learning`

---

<a id="item-9"></a>
## [Tim King, AmigaDOS Developer, Dies; Community Pays Tribute](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 7.0/10

Tim King, the developer of AmigaDOS, has passed away, as reported on amiga-news.de. The announcement has prompted an outpouring of community remembrance and gratitude for his contributions. King's work on AmigaDOS was a core part of the Amiga operating system, which influenced a generation of home computer users and programmers. His passing is a significant moment for the retrocomputing community, which has lost a key figure in computing history. AmigaDOS was originally based on a TRIPOS port by MetaComCo, written in BCPL, and was later rewritten in C starting with AmigaOS 2.x. Community comments also remember him as the founder of UK Online, and an interview from October 2021 is linked.

hackernews · doener · Aug 12, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49272655)

**Background**: AmigaDOS is the disk operating system component of AmigaOS, providing file systems, command-line interface, and file redirection. The Amiga was a family of personal computers produced by Commodore from 1985 to 1994, known for custom graphics and sound hardware, running AmigaOS with a desktop environment called Workbench. AmigaDOS's early BCPL-based implementation had limitations, leading to a comprehensive rewrite in C from AmigaOS 2.x onward.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga_computer">Amiga computer</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal stories, thanking Dr. King for the countless hours spent with their Amigas. Some described AmigaDOS as their gateway to the command-line interface and later to Linux, while others remembered him as the founder of UK Online. Overall sentiment is one of gratitude and mourning.

**Tags**: `#Amiga`, `#AmigaDOS`, `#retrocomputing`, `#obituary`

---

<a id="item-10"></a>
## [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 7.0/10

The blog post by Andros Fenollosa explores building real-time single-page applications by sending HTML over WebSockets, a pattern that requires very little client-side JavaScript. It compares this approach with Server-Sent Events (SSE) and LiveView-style server-rendered frameworks. This discussion matters because it highlights an alternative to JSON APIs and heavy client-side JavaScript, letting server-side logic drive real-time UI updates. The trade-offs between WebSockets and SSE are central to choosing an architecture for modern web apps. The article notes that how HTML travels over the wire determines latency and bidirectionality, and that HTML over WebSockets is not the answer to everything. It positions the pattern as a form of hypermedia/'HTML over the wire,' with Phoenix LiveView as a notable implementation.

hackernews · redbell · Aug 12, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49275335)

**Background**: Traditional SPAs send JSON to the browser and use JavaScript to render pages, a pattern dominant since the early 2010s. HTML over WebSockets instead sends server-rendered HTML fragments over a persistent connection, so the server controls the UI while the browser needs only a small script. Server-Sent Events (SSE) is a related, simpler technology for server-to-client pushes over a single HTTP connection, which is unidirectional. Phoenix LiveView, introduced by Chris McCord, is the most well-known framework using this server-rendered, real-time approach.

<details><summary>References</summary>
<ul>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets : real-time SPAs with... | Andros Fenollosa</a></li>
<li><a href="https://testdriven.io/blog/html-over-websockets/">HTML Over WebSockets | TestDriven.io</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events">Server - sent events - Web APIs | MDN</a></li>

</ul>
</details>

**Discussion**: Comments are mostly supportive but stress context: one reader recommends SSE whenever only server-to-client push is needed, while others note WebSockets suit bidirectional low-latency cases. Another points out that Chris McCord had experimented with this idea in Rails (Sync) before moving to Phoenix, and one commenter suggests htmx with SSE as a lighter alternative. There is also a link to a critical response at yagni.club.

**Tags**: `#WebSockets`, `#real-time`, `#SPA`, `#JavaScript`, `#LiveView`

---

<a id="item-11"></a>
## [uBlock Origin Abandons Attempt to Block Facebook Ads](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 7.0/10

uBlock Origin has stopped attempting to filter ads on Facebook, admitting that the platform's ad delivery is technically too difficult to block consistently. The decision was reported by Neowin and discussed in a Reddit thread on r/uBlockOrigin. This matters because it highlights the escalating arms race between ad blockers and major platforms, and it means Facebook users relying on uBlock Origin will now see ads. It may also push the community toward more radical approaches, such as computer vision-based ad detection. Facebook uses heavy obfuscation and server-side rendering, making ad elements nearly indistinguishable from organic content to filter lists. uBlock Origin's developer chose to focus resources on other sites where blocking remains feasible, rather than chase every Facebook change.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**Background**: uBlock Origin is a free, open-source browser extension popular for blocking ads and other content, with tens of millions of users on Chrome and Firefox. Facebook has a long history of fighting ad blockers, starting with bypassing them on desktop in 2016 and continuing with hidden technical countermeasures that web developers have criticized. The latest decision reflects the growing difficulty of maintaining filter lists against a platform with near-unlimited engineering resources.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://www.bbc.com/news/technology-46508234">Facebook 's hidden battle against ad - blockers</a></li>
<li><a href="https://www.techtimes.com/articles/173082/20160809/facebook-blocking-ad-blockers-on-desktop-but-at-least-you-can-tailor-your-ad-experience.htm">Facebook Blocking Ad Blockers On Desktop, But At Least You Can...</a></li>

</ul>
</details>

**Discussion**: Commenters on the Reddit thread generally supported the decision, with some seeing it as inevitable. A widely-upvoted comment predicted the future involves computer vision models that visually detect and occlude ads, while another argued the only real solution is to stop using Facebook entirely. Some questioned why Facebook invests so much in defeating ad blockers when these users are unlikely to click ads.

**Tags**: `#ad-blocking`, `#privacy`, `#Facebook`, `#uBlock Origin`, `#arms race`

---

<a id="item-12"></a>
## [AI Agents Discover New Materials to Solve GPU Heat Problems](https://discoveredmaterials.com/research/) ⭐️ 7.0/10

YC-backed startup Discovered Materials launched an AI-agent platform that computationally designs new semiconductor materials, and released hundreds of discovered materials plus a benchmark. In tests, seven frontier models from Anthropic, OpenAI, and Kimi found dynamically stable, promising materials in an 8-hour run, a task the company says would take a PhD student weeks. Chip heat is escalating rapidly — Nvidia's Blackwell reaches 1.2 kW and Rubin is projected at 2.3 kW — and new materials are a key bottleneck for 3D packaging and HBM cooling. If AI agents can shorten the lab-to-fab timeline, they could transform semiconductor manufacturing and cut data-center power and water consumption. The company plans to license or sell intellectual property on both the discovered materials and their synthesis recipes, and is also exploring selling its AI harness and tools. Its benchmark also exposes odd frontier-model behaviors, such as Claude's reward hacking and GPT-5.6 'losing its mind' after roughly 50 million tokens.

hackernews · advaith08 · Aug 12, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49269090)

**Background**: Modern GPUs dissipate heat measured by thermal design power (TDP), and the H100, Blackwell, and Rubin chips are doubling that figure with each generation. A major obstacle to 3D chip packaging — stacking HBM memory directly on logic — is that dielectric materials like SiO2 conduct heat poorly. Moving a new material from computational discovery into a real fab is known as the 'lab-to-fab valley of death,' and it can take years and hundreds of millions of dollars. AI-driven materials discovery is an emerging field; for example, Argonne National Laboratory has built an AI-agent system to automate simulation-based discovery.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Three-dimensional_integrated_circuit">Three-dimensional integrated circuit - Wikipedia</a></li>
<li><a href="https://www.anl.gov/article/scientists-deploy-ai-agents-to-accelerate-discovery-of-new-materials">Scientists deploy AI agents to accelerate discovery of new materials | Argonne National Laboratory</a></li>

</ul>
</details>

**Discussion**: Commenters were cautiously positive but raised substantive concerns. One joked about the amusing 'GPT-5.6 Terra' reasoning summary quoted in the post, while another questioned how truly novel compounds can be verified when they may already exist in model training data. Others noted that past AI materials-discovery efforts lacked real impact and welcomed the feasibility data, and one researcher agreed that closing the computational-experimental loop is the main challenge.

**Tags**: `#AI`, `#materials science`, `#semiconductors`, `#startup`, `#YC`

---

<a id="item-13"></a>
## [No Lossless AI Text Rewrites: Writers Must Stand Behind Every Sentence](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/) ⭐️ 7.0/10

Sophie Alpert published a post arguing that no AI transformation of natural-language text is lossless, and proposed an internal policy for engineers using AI writing tools. The policy requires that writers stand behind every idea and every sentence in their documentation. This matters because it calls out a common but often unexamined practice of using LLMs to rewrite documentation, which can silently change meaning. It gives engineers and writers a concrete, practical standard for responsible AI use and contributes to the broader conversation about human accountability in AI-assisted writing. Alpert's core claim is that every rewrite changes meaning because the AI lacks the writer's detailed mental representation of what they intended to communicate. The post also emphasizes that if a reviewer asks about a line, replying 'AI wrote that, just ignore it' is unacceptable.

rss · Simon Willison · Aug 11, 23:48

**Background**: Large language models (LLMs) are increasingly used to rewrite, summarize, or improve natural-language text, from documentation to emails. While these models can generate fluent output, they do not have access to the author's internal intent, so any transformation risks losing or distorting the original meaning. Alpert's post is part of a broader discussion about how teams should responsibly adopt AI writing tools in technical documentation and engineering workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/">There are no lossless transformations of natural-language text</a></li>
<li><a href="https://sophiebits.com/2026/06/25/there-are-no-lossless-transformations-of-natural-language-text">There are no lossless transformations of natural-language text – Sophie Alpert</a></li>
<li><a href="https://news.ycombinator.com/item?id=48980425">There are no lossless transformations of natural-language text | Hacker News</a></li>

</ul>
</details>

**Discussion**: Community reactions on Hacker News were mixed. Some commenters pushed back, arguing that in many contexts AI-generated documentation is good enough, and that in 2026, handwriting docs adds less value than writing high-quality instructions to an AI agent. This provides a practical counterpoint to Alpert's principle.

**Tags**: `#AI`, `#writing`, `#documentation`, `#engineering`, `#LLM`

---

<a id="item-14"></a>
## [Site ranks CS conferences by trip quality, not prestige](https://www.reddit.com/r/MachineLearning/comments/1vmbdk6/i_built_an_honest_cs_conference_ranking_sorted_by/) ⭐️ 7.0/10

A Reddit user unveiled HonestCSRankings.org, a tool that maps about 540 upcoming CORE-ranked CS conferences and ranks them by destination quality (weather, safety, cost, accessibility, city vibe) rather than academic rank. It includes an "Upsets" tab for A* venues in poor destinations and supports filtering, ICS export, and deep links. This reframes conference selection for researchers by making travel experience a first-class criterion alongside academic prestige, addressing a real gap in how venues are chosen. It could influence attendance decisions and even conference site selection practices across the CS community. The ranking integrates real climate data for the conference month, the Global Peace Index for safety, World Bank price levels for cost, and local accessibility/vibe scores. The long tail of smaller conferences is scraped from WikiCFP, so errors are possible; ICML/ICLR 2027 and COLM are missing due to lack of announcements or CORE rankings.

reddit · r/MachineLearning · /u/JohnAZoidberg77 · Aug 12, 11:23

**Background**: CORE (Computing Research and Education Association of Australasia) maintains a widely used ranking of computer science conferences, now expanded into the international ICORE rankings. The Global Peace Index, produced by the Institute for Economics & Peace, measures national peacefulness and safety, while the World Bank publishes price-level indices for cost comparisons. WikiCFP is a wiki-style hub listing calls for papers for CS conferences and workshops, providing data for smaller venues.

<details><summary>References</summary>
<ul>
<li><a href="https://www.core.edu.au/conference-portal">CORE Rankings Portal - core.edu.au</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Peace_Index">Global Peace Index</a></li>
<li><a href="http://www.wikicfp.com/cfp/">WikiCFP : Call For Papers of Conferences, Workshops and Journals</a></li>

</ul>
</details>

**Tags**: `#CS conferences`, `#conference ranking`, `#research travel`, `#tool`, `#academia`

---

<a id="item-15"></a>
## [Decoupled Descent Enforces Train-Test Error Tracking via AMP Onsager Corrections](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 7.0/10

The paper introduces Decoupled Descent (DD), a theory-based training algorithm that uses approximate message passing (AMP) Onsager corrections to enforce that the training error asymptotically matches the test error at every parameter iterate. The method is demonstrated on full-batch gradient descent for stylized Gaussian mixture models, including a high-dimensional XOR experiment with a two-layer network. This is significant because it turns a fundamental train-test generalization gap into an explicit, certificate-like guarantee during optimization, rather than relying on post-hoc validation or complex analyses. It could offer new principled approaches to optimal stopping, hyperparameter tuning, and future extensions to SGD and more general models. The paper treats the train-test gap as a consequence of data reuse bias and provides an asymptotic "train-test identity" rather than finite-sample guarantees; simulations show the method's behavior over 100 runs with 25%-75% quantile bands. The author emphasizes this is a theory paper, with a planned PyTorch-compatible implementation to follow.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**Background**: Gradient descent often drives training error to zero while test error stays flat or rises; the paper attributes this to data reuse bias. Approximate message passing (AMP) is an iterative high-dimensional statistical method whose dynamics can be tracked exactly via state evolution, thanks to an "Onsager correction" term that removes harmful correlations between iterations. Earlier work, such as Onsager-corrected deep learning, applied this idea to decouple prediction errors across neural-network layers, and this paper applies a similar correction to training dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.27883v1">Decoupled Descent: Exact Test Error Tracking Via Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/abs/2201.07487">A Concise Tutorial on Approximate Message Passing A unifying tutorial on Approximate Message Passing Lecture 19: Approximate message passing algorithms Approximate Message Passing Tutorial - GitHub Pages Vector Approximate Message Passing - IEEE Xplore Message-passing algorithms for compressed sensing Approximate Message Passing - GitHub Pages</a></li>
<li><a href="https://arxiv.org/abs/1607.05966">[1607.05966] Onsager-corrected deep learning for sparse ... Score-Based VAMP with Fisher-Information-Based Onsager Correction Onsager reciprocal relations - Wikipedia Onsager Correction in GOAMP - api.emergentmind.com Onsager-corrected deep learning for sparse linear inverse ... Score-Based VAMP with Fisher-Information-Based Onsager Correction</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#generalization`, `#approximate message passing`, `#optimization`, `#theory`

---

<a id="item-16"></a>
## [Webcam Aggregation Page Lets You Watch the 2026 Solar Eclipse Online](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 6.0/10

A curated web page at jonty.github.io/2026_eclipse_webcams aggregates live webcam feeds of the 2026 total solar eclipse, allowing remote viewing across Iceland and Spain. This makes a rare astronomical event accessible to anyone with internet access, while being a practical community tool for coordinating live views. It also highlights the growing use of simple static web pages for real-time event coverage. The page was originally built in 2024 for the US solar eclipse, according to the author. It aggregates webcams from Iceland and Spain, and the author notes the challenge of coordinating multiple camera feeds during the eclipse.

hackernews · zoenolan · Aug 12, 11:53 · [Discussion](https://news.ycombinator.com/item?id=49270953)

**Background**: A solar eclipse occurs when the Moon passes between the Earth and the Sun, briefly blocking sunlight. The total solar eclipse of August 2026 will pass over parts of Iceland and Spain, and webcams allow people outside the path to experience it in real time. The 2024 US eclipse inspired many similar community-driven web tools.

**Discussion**: The author shared the backstory of building the page minutes before the 2024 eclipse and repurposing it for 2026. Commenters added personal eclipse travel stories, historical context from Thales of Miletus, and links to additional webcams and live solar-power data.

**Tags**: `#eclipse`, `#webcams`, `#astronomy`, `#web-tools`, `#community`

---

<a id="item-17"></a>
## [AI-Generated Code Leads to Unmaintainable Systems](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 6.0/10

In a blog post, Florian Herrengt illustrates a scenario where a team cannot fix a bug because AI-generated code has created a system so convoluted that no one understands it, and even AI tools like Claude Fable fail to help. This highlights a growing 'cognitive debt' problem in software engineering. As AI coding tools like Claude Fable become more capable and widely adopted, the risk of creating unmaintainable code rises, potentially leading to higher costs, slower development, and serious bugs. This underscores the urgent need for robust review practices and human oversight in AI-assisted programming. The quoted scenario describes a developer telling a colleague 'I don't know, let me ask Claude,' then watching an 'endless wall of text' with no way to verify its accuracy. The project has 'so many layers and services' that no one on the team could possibly understand the whole system.

rss · Simon Willison · Aug 12, 15:08

**Background**: AI-assisted programming uses large language models like Claude to generate code, often through tools such as Claude Fable 5, which can autonomously handle complex multi-day coding tasks. While these tools boost productivity and have strong benchmarks, they can produce opaque code that developers don't fully understand, creating 'cognitive debt'—the future mental burden of deciphering and maintaining such code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.agensi.io/learn/best-ai-coding-tools-july-2026">Best AI Coding Tools July 2026: Post-GPT-5.6 and Fable 5 ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#code quality`, `#future of work`

---

<a id="item-18"></a>
## [AAAI 2027 Reviewer Flags Low Code Submission Rate](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

A reviewer for AAAI 2027 reported on Reddit that surprisingly few submissions in their batch included code, despite AAAI's explicit reproducibility expectations. The reviewer is considering factoring the absence of code into initial scores. This highlights a persistent gap between reproducibility policies and actual practice in top AI conferences. If code becomes a de facto requirement, it could improve research credibility but also raise barriers for authors. AAAI provides a reproducibility checklist in its author kit that must be submitted with the paper, and the main technical track call explicitly encourages code, datasets, and evaluation tools. However, code release is not an official mandatory requirement.

reddit · r/MachineLearning · /u/wontonut · Aug 11, 18:58

**Background**: AAAI is a leading conference in artificial intelligence, and it has published reproducibility checklists for multiple cycles, including AAAI-25, AAAI-26, and AAAI-27. The checklists ask authors to state whether code, hyperparameters, and evaluation details are available. While the conference encourages code sharing, it does not strictly mandate it. The Reddit discussion reflects ongoing community debate about whether such voluntary policies are sufficient.

<details><summary>References</summary>
<ul>
<li><a href="https://aaai.org/conference/aaai/aaai-27/submission-instructions/">AAAI-27 Submission Instructions - AAAI</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-26/reproducibility-checklist/">AAAI-26 Reproducibility Checklist - AAAI</a></li>
<li><a href="https://aaai.org/conference/aaai/aaai-27/main-technical-track-call/">AAAI-27 Main Technical Track Call - AAAI</a></li>

</ul>
</details>

**Tags**: `#reproducibility`, `#AAAI`, `#ML research`, `#peer review`

---

<a id="item-19"></a>
## [Seeking Advice on RL and Planning for Stochastic Merge Puzzle](https://www.reddit.com/r/MachineLearning/comments/1vlfavg/planningrl_for_a_stochastic_singleplayer_merge/) ⭐️ 6.0/10

A developer working on a stochastic merge-puzzle AI asked the machine-learning community for pointers on planning and reinforcement-learning algorithms, describing a game with afterstates, one-move-previewed random drops, and throughput objectives. This question is relevant because the game's structure—action, afterstate, then random event—is common in many games and real-world sequential decision problems. The discussion could reveal efficient ways to combine learning-based value estimates with limited planning budgets, benefiting researchers and developers working on stochastic planning, MCTS, and deep RL for board/puzzle games. The game uses 6 stacks with a max height of 7, 30 possible ordered-pair actions, cascading merges of equal tiles, and a 9 disappearing for one point; every fourth player action is preceded by a preview of six random tiles. The network is column-permutation equivariant with 394 input features, an action head for 30 actions, and value heads predicting future 9 count, distance to the next 9, and short-term death risk.

reddit · r/MachineLearning · /u/CaiwenGong · Aug 11, 11:53

**Background**: In reinforcement learning, an afterstate is the state immediately after the agent's action but before any random event, such as a tile drop; planning from afterstates can reduce branching and improve sample efficiency, which is why many games use an action→afterstate→chance-event transition. The described game resembles 2048 in this respect but has a larger action space and a previewed random event, making it a useful testbed for combining exact simulation, Monte Carlo tree search, and learned value/policy networks.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.stackexchange.com/questions/24816/how-are-afterstate-value-functions-mathematically-defined">reinforcement learning - How are afterstate value functions ...</a></li>
<li><a href="https://openreview.net/forum?id=XO944P8prc">Afterstate Reinforcement Learning for Continuous Control</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#planning`, `#stochastic games`, `#puzzle AI`, `#monte carlo tree search`

---

<a id="item-20"></a>
## [Agentic World Cup: LLMs Compete in 1v1 Soccer Matches](https://www.reddit.com/r/MachineLearning/comments/1vllvmn/we_built_the_agentic_world_cup_llms_that_compete/) ⭐️ 6.0/10

The creators launched the Agentic World Cup, a platform where users select an LLM, coach it through prompting, and submit it to compete in automated 1v1 soccer matches against other agents. Rankings are published weekly on the site. This project addresses the 'embodiment gap'—the observation that AI agents can code and reason but struggle with physical, real-time tasks. Competitive sports provide a public benchmark for embodied intelligence, letting researchers and engineers test methods like ViTs, online RL, and neuro-symbolic systems. Users sign in, select an LLM, coach it through prompting, and submit; matches run automatically and final rankings are published by Friday. The long-term vision is a public forum for testing embodied challenges.

reddit · r/MachineLearning · /u/agenticworldcup · Aug 11, 16:12

**Background**: Embodied intelligence is a computational approach to designing and understanding intelligent behavior in agents that are tightly coupled with their environment, often studied in robotics and soft robotics. The 'embodiment gap' describes the limitation of AI systems—especially LLMs—in tasks that require physical interaction or real-time sensorimotor control, such as sports. This project uses competitive 1v1 soccer as both a training ground and a benchmark for embodied AI, aiming to make agents 'think like athletes.'

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/chapter/10.1007/978-3-662-43505-2_37">Embodied Intelligence | Springer Nature Link</a></li>
<li><a href="https://www.preprints.org/manuscript/202407.0869">Bridging the Embodiment Gap : Embodied AI for... | Preprints.org</a></li>
<li><a href="https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2025.1668910/pdf">A review of embodied</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#embodied intelligence`, `#benchmarking`, `#agents`, `#sports simulation`

---