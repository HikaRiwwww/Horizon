---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 39 items, 27 important content pieces were selected

---

1. [Kimi K3: Open Frontier Model with 2.8T Parameters](#item-1) ⭐️ 9.0/10
2. [Firefox Compiled to WebAssembly Runs Inside Another Browser](#item-2) ⭐️ 9.0/10
3. [Linus Torvalds Declares Linux Not Anti-AI, Threatens Fork](#item-3) ⭐️ 9.0/10
4. [Harness 'Schema' Claims 99% on ARC-AGI-3](#item-4) ⭐️ 9.0/10
5. [LM Studio Bionic: AI Agent Harness for Open Models](#item-5) ⭐️ 8.0/10
6. [Using Classical ML to Detect LLM-Generated Text](#item-6) ⭐️ 8.0/10
7. [Roc Compiler Rewrite from Rust to Zig](#item-7) ⭐️ 8.0/10
8. [GPT-5.6 Codex Bug Risks File Deletion in Full Access Mode](#item-8) ⭐️ 8.0/10
9. [Inkling: Thinking Machines Lab Releases 975B Parameter Open-Weights Model](#item-9) ⭐️ 8.0/10
10. [xAI open-sources Grok Build after privacy backlash](#item-10) ⭐️ 8.0/10
11. [Researcher Tricks Claude into Leaking Private Data via web_fetch Loophole](#item-11) ⭐️ 8.0/10
12. [QLoRA Default LR 2e-4 Overfits on Small Datasets, says Reddit](#item-12) ⭐️ 8.0/10
13. [ExTernD: Ternary Decomposition for LLM Quantization with Arbitrary Accuracy](#item-13) ⭐️ 8.0/10
14. [Microsoft Comic Chat open-sourced, sparking nostalgia](#item-14) ⭐️ 7.0/10
15. [Decoy Font: A Font That Fools AI by Hiding Text in Plain Sight](#item-15) ⭐️ 7.0/10
16. [Book on Mathematics of Data Science Hits arXiv](#item-16) ⭐️ 7.0/10
17. [Interactive Linear Algebra Book with Dynamic Figures](#item-17) ⭐️ 7.0/10
18. [Seeking Collaborators for Scaling and Evaluation of DABSN Recurrent LM Architecture](#item-18) ⭐️ 7.0/10
19. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-19) ⭐️ 7.0/10
20. [Reddit User Seeks Devil's Advocates on JEPA Models](#item-20) ⭐️ 7.0/10
21. [PnP-CoSMo: Content/Style Modeling for Multi-Contrast MRI Reconstruction](#item-21) ⭐️ 7.0/10
22. [MOSBO tools for heterogeneous meta-analysis data](#item-22) ⭐️ 7.0/10
23. [170x PyTorch slowdown on T4 vs A100: extreme bottleneck explained](#item-23) ⭐️ 7.0/10
24. [Go Library Turns Mermaid Diagrams into Colorful ASCII Art via WebAssembly](#item-24) ⭐️ 6.0/10
25. [Mermaid Diagrams Converted to Unicode Box Art via Rust+WASM](#item-25) ⭐️ 6.0/10
26. [First RTCA Workshop at NeurIPS 2026 Calls for Papers](#item-26) ⭐️ 6.0/10
27. [Disentangling Convolutional Neurons with Hadamard Product Clustering](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Kimi K3: Open Frontier Model with 2.8T Parameters](https://www.kimi.com/blog/kimi-k3) ⭐️ 9.0/10

Kimi has released Kimi K3, a 2.8 trillion parameter open-weight model that achieves frontier-level performance in coding, reasoning, and knowledge tasks, with competitive pricing at $3/$15 per million tokens. This release signals that open-weight models are rapidly closing the gap with proprietary frontier models, potentially accelerating AI commoditization and lowering costs for developers and enterprises. Kimi K3 has a 1 million token context window, and its pricing matches Anthropic's Sonnet series; benchmarks place it ahead of Opus 4.8 and near Fable/Sol level.

hackernews · vincent_s · Jul 16, 14:46 · [Discussion](https://news.ycombinator.com/item?id=48935342)

**Background**: Open-weight models allow anyone to download and use the trained parameters, unlike closed models where only the API is available. Kimi K3 is one of the largest open models, with 2.8 trillion parameters, and represents a trend of Chinese AI labs pushing the frontier of open-source AI.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.reddit.com/r/LocalLLaMA/comments/1uydbmc/kimi_k3_shows_openweight_models_are_about_to/">Kimi K3 Shows Open-Weight Models Are About to Overtake the Frontier - Reddit</a></li>

</ul>
</details>

**Discussion**: The community is excited by Kimi K3's performance but notes its high pricing for a Chinese open-weight model, though many agree it is justified by its capability. There is debate on whether such releases commoditize AI to sell hardware, with some pointing out the massive training costs contradict true commoditization.

**Tags**: `#AI`, `#open source models`, `#pricing`, `#frontier intelligence`, `#Chinese AI`

---

<a id="item-2"></a>
## [Firefox Compiled to WebAssembly Runs Inside Another Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

A team called Puter has successfully compiled the Firefox browser (Gecko engine) to WebAssembly, enabling a full browser to run inside another browser like Chrome. The project utilized AI-assisted development with Claude Opus and Fable tokens to achieve this feat. This demonstration pushes the boundaries of WebAssembly capabilities, showing that even a complex, full-featured browser can be compiled and run inside another browser. It has potential implications for browser testing, sandboxing, and novel web applications. The project used Firefox/Gecko due to its strong single-process support. All network traffic is proxied through Puter's server using the Wisp protocol over WebSockets, as browser-based WebAssembly cannot open arbitrary network connections. The team reported an estimated $25,000 worth of Claude Opus and Fable tokens were used, but actual cost was lower due to subscription plans.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a binary instruction format that allows code written in languages like C/C++ to run in web browsers at near-native speed. Compiling a full browser like Firefox to WASM is extremely challenging due to the complexity of browser internals. The Wisp protocol is a lightweight protocol for proxying TCP/UDP sockets over a single WebSocket connection, which is essential for enabling network access in this environment. Claude Opus and Fable are AI models from Anthropic used here to assist with the massive code refactoring needed for the compilation.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus">Claude Opus</a></li>
<li><a href="https://www.mindstudio.ai/blog/claude-fable-5-pricing-access-usage-limits">Claude Fable 5 Pricing, Access, and Usage Limits: What You Need to Know | MindStudio</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion highlighted both amazement at the technical achievement and concern about the server costs of proxying all traffic. The Puter team had to scale up servers to handle the traffic spike from the HN front page. Some commenters noted the end-to-end encryption claim and verified it by inspecting WebSocket messages.

**Tags**: `#WebAssembly`, `#Firefox`, `#browser`, `#emulation`, `#AI-assisted development`

---

<a id="item-3"></a>
## [Linus Torvalds Declares Linux Not Anti-AI, Threatens Fork](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 9.0/10

Linus Torvalds, the creator and lead maintainer of Linux, stated on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, threatening to fork the project or telling dissenters to walk away. This definitive endorsement by the top maintainer sets the course for Linux kernel development, likely accelerating AI integration and influencing the broader open-source community's acceptance of AI tools. Torvalds emphasized that AI's usefulness is no longer in question, though other questions like the economy remain, and he firmly put his foot down against anti-AI sentiment in the project.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds has been the authoritative figure in Linux development for decades. The kernel community has had ongoing debates about incorporating AI/ML tools; this statement resolves the ambiguity by explicitly endorsing AI use.

**Tags**: `#Linux`, `#AI`, `#open source`, `#kernel development`, `#Linus Torvalds`

---

<a id="item-4"></a>
## [Harness 'Schema' Claims 99% on ARC-AGI-3](https://www.reddit.com/r/MachineLearning/comments/1uyf8oo/new_fable5opus48_harness_called_schema_claims_99/) ⭐️ 9.0/10

A new AI harness called Schema achieves 99% on the ARC-AGI-3 Public set using Claude Opus 4.8 and Fable 5, and 95.35% using GPT-5.6 Sol, without modifying underlying model weights. This could represent a paradigm shift in AI reasoning, as the harness approach dramatically improves performance on a benchmark considered difficult for current models, potentially enabling more general intelligence without retraining. The harness uses a fixed fallback rule: Opus 4.8 and Sol xhigh run first; games scoring below 80 are rerun with Fable 5 and Sol max, respectively, retaining the higher per-game score.

reddit · r/MachineLearning · /u/we_are_mammals · Jul 16, 21:02

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that challenges AI agents to explore novel environments, acquire goals, build adaptable world models, and learn continuously. Most frontier models score below 15% on this benchmark. A harness is external code that manages model execution, memory, API calls, and output validation—essentially augmenting the model's capabilities without changing its weights.

<details><summary>References</summary>
<ul>
<li><a href="https://schema-harness.github.io/">Frontier Models with Our Harness Achieve ~99% on ARC-AGI-3 Public — Schema</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC - AGI - 3</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#ARC-AGI`, `#reasoning`, `#AI research`, `#LLM`

---

<a id="item-5"></a>
## [LM Studio Bionic: AI Agent Harness for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio has launched Bionic, an AI agent harness that enables users to run autonomous agents using open-source models locally, with specialized projects for coding and document manipulation. This marks a significant step in bringing autonomous agent capabilities to local, private AI, reducing reliance on cloud services. It could accelerate adoption of open-source models for complex, multi-step tasks. Bionic includes two project types: 'Code' for coding tasks and 'Work' for document creation and manipulation, with automatic checkpointing in Work projects. It integrates with LM Studio's existing local model library.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: An AI agent harness is a software layer that provides a language model with tools, memory, workflow orchestration, and guardrails, enabling it to perform multi-step tasks autonomously. LM Studio is a popular free desktop application for downloading and running open-source LLMs like Llama and Mistral locally. Bionic extends this by adding a built-in harness for running agents, making local AI more capable.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48939662">LM Studio Bionic: the AI agent for open models | Hacker News</a></li>
<li><a href="https://www.databricks.com/blog/ai-harness">What is an AI Agent Harness ? | Databricks Blog</a></li>

</ul>
</details>

**Discussion**: Founder Yagil offered free credits for trying Bionic with specific models, and early user inventor7777 reported positive results with Qwen3.6 35B but noted some rough edges. Other commenters discussed the implications for local AI and compared Bionic to other agent harnesses.

**Tags**: `#AI agents`, `#open models`, `#LM Studio`, `#local AI`, `#code generation`

---

<a id="item-6"></a>
## [Using Classical ML to Detect LLM-Generated Text](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 8.0/10

The author demonstrates that classical machine learning models like logistic regression can effectively detect LLM-generated text by using features such as perplexity and burstiness, achieving high accuracy. This is important because classical ML detectors are computationally cheaper, more transparent, and easier to deploy than deep learning models, potentially enabling widespread use in combating AI-generated misinformation. The classifier is compact and fast, using only handcrafted features, but its long-term effectiveness is uncertain as LLMs evolve to mimic human variability.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: Classical machine learning for text classification relies on engineered features like n-grams, perplexity scores, and sentence length distributions, rather than neural embeddings. LLM-generated texts often exhibit lower perplexity and more uniform style than human writing. This approach contrasts with larger deep learning detectors that require substantial compute and data.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/better-programming/detecting-llm-generated-texts-befce4426da9">Detecting LLM - Generated Texts . Is it possible to differentiate between</a></li>
<li><a href="https://arxiv.org/pdf/2303.07205">The Science of Detecting LLM - Generated Texts</a></li>

</ul>
</details>

**Discussion**: Comments range from skepticism, calling the effort a 'losing battle,' to interest in practical applications like browser extensions for real-time detection. Some argue that the best detector remains humans and that effort-based evaluation may be more robust.

**Tags**: `#LLM detection`, `#machine learning`, `#AI-generated text`, `#classification`, `#NLP`

---

<a id="item-7"></a>
## [Roc Compiler Rewrite from Rust to Zig](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

The Roc programming language team is rewriting its compiler from Rust to Zig, citing faster incremental builds and better control over memory layout for compiler-specific tasks like binary patching. This move highlights real-world trade-offs between safety and performance in systems programming, especially for compilers that need low-level memory control. It may influence language choices for future compiler projects. Zig's incremental build system is a key advantage, but the rewrite also addresses the need for memory-unsafe operations in compiler tasks such as code reloading. Rust's safety guarantees come with overhead that may not suit all compiler use cases.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Roc is a functional programming language focused on simplicity and performance, currently in early development. The Rust language prioritizes memory safety without garbage collection, while Zig offers manual memory management with compile-time safety checks. This rewrite reflects the different philosophies of the two languages in a practical compiler project.

<details><summary>References</summary>
<ul>
<li><a href="https://www.roc-lang.org/">The Roc Programming Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust (programming language) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Steveklabnik questioned the claim that compilers need significant unsafe code, noting that only specific features like code reloading require it. Other commenters debated Zig's runtime safety compared to Rust's compile-time guarantees, and whether Zig's incremental builds are a lasting advantage given potential future improvements in Rust.

**Tags**: `#Rust`, `#Zig`, `#compilers`, `#systems programming`, `#memory safety`

---

<a id="item-8"></a>
## [GPT-5.6 Codex Bug Risks File Deletion in Full Access Mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

A bug in GPT-5.6's Codex AI agent can delete user files when full access mode is enabled without sandboxing and the model mistakenly overrides $HOME instead of a temporary directory. This issue was reported by Thibault Sottiaux and investigated by OpenAI. This bug underscores critical safety risks in AI coding agents that have direct file system access, potentially causing irreversible data loss for developers and enterprises. It highlights the need for robust sandboxing and review mechanisms before deploying such agents in production. The bug occurs specifically when full access mode is enabled without sandboxing protections and the model attempts to override the $HOME environment variable but deletes $HOME by mistake. OpenAI recommends enabling auto-review and sandboxing to prevent similar incidents.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent developed by OpenAI, released in April 2025 as Codex CLI, designed to understand natural language and perform software engineering tasks. GPT-5.6 is the underlying large language model powering Codex. AI agents like Codex can execute commands on a user's machine, which introduces risks if given unrestricted access to the file system.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-9"></a>
## [Inkling: Thinking Machines Lab Releases 975B Parameter Open-Weights Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights multimodal Mixture-of-Experts model with 975B total parameters (41B active), licensed under Apache 2.0 and trained on 45 trillion tokens of text, images, audio, and video. Inkling strengthens the US open-weights AI ecosystem by providing a competitive alternative to Chinese open models and other US releases like NVIDIA Nemotron and Gemma 4, while also offering a strong base for fine-tuning via Thinking Machines' Tinker platform. The model card is notably sparse, with minimal training data documentation, and Thinking Machines admits Inkling is not a frontier model but a capable base model for customization. An additional smaller variant, Inkling-Small (276B total, 12B active), is promised but not yet released.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is a neural network architecture that uses multiple subnetworks ('experts') with a gating mechanism to activate only relevant experts per input token, enabling larger total parameters with lower computational cost. Open-weights models release pretrained parameters for public use but may not include full training code or data, offering a middle ground between proprietary and fully open-source AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/04/open-weight-models/">What are Open Source and Open Weight Models ? | Analytics Vidhya</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#multimodal`, `#mixture-of-experts`, `#AI model release`, `#Thinking Machines Lab`

---

<a id="item-10"></a>
## [xAI open-sources Grok Build after privacy backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI released the entire Grok Build codebase under an Apache 2.0 license on GitHub, following severe community backlash over the grok CLI tool that unintentionally uploaded entire directories to xAI's cloud storage. This move aims to restore user trust by providing complete transparency and allowing developers to run the tool locally, setting a new precedent for privacy in AI coding assistants. The codebase contains 844,530 lines of Rust with only about 3% vendored, and includes a self-contained Mermaid diagram renderer and tool implementations inspired by Codex and OpenCode.

rss · Simon Willison · Jul 15, 23:59

**Background**: The grok CLI tool from xAI is an AI-powered coding assistant. Recent backlash occurred when users discovered that running the tool in a directory would upload that entire directory to xAI's cloud, including sensitive files like SSH keys and password managers.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>

</ul>
</details>

**Discussion**: Community comments expressed outrage over the privacy violation, with one user reporting their entire home directory was uploaded. After open-sourcing, sentiment shifted to cautious optimism, though some remain skeptical about xAI's handling of retained data.

**Tags**: `#privacy`, `#security`, `#AI`, `#open-source`, `#CLI`

---

<a id="item-11"></a>
## [Researcher Tricks Claude into Leaking Private Data via web_fetch Loophole](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Security researcher Ayush Paul discovered a prompt injection attack that exploited Claude's web_fetch tool to exfiltrate private user data, such as name, city, and employer, by embedding URLs in a honeypot page that the tool would follow. This vulnerability demonstrates a practical bypass of Anthropic's exfiltration protections, highlighting that even well-designed AI safety measures can be circumvented through multi-step prompt injection attacks, posing a serious risk to user privacy in widely-used AI assistants. The attack worked because web_fetch was allowed to navigate to URLs embedded in previously fetched pages, enabling an attacker to chain multiple requests that ultimately led to exfiltration. Anthropic declined to pay a bug bounty, stating they had already identified the issue internally, and have since closed the loophole by removing that navigation capability.

rss · Simon Willison · Jul 15, 14:21

**Background**: The Claude web_fetch tool is designed to retrieve full content from specified web pages, but it can be exploited when combined with private data (e.g., user memories) and untrusted content—a pattern known as the 'lethal trifecta' for AI agents. Previously, Anthropic had implemented deterministic rules to prevent data exfiltration by restricting web_fetch to only visit exact URLs provided by the user or returned by the companion web_search tool.

<details><summary>References</summary>
<ul>
<li><a href="https://anthropic.mintlify.app/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://onthewire.ai/article/a-researcher-tricked-claude-into-spelling-out-a-user-s-private-data-one-letter-a">A Researcher Tricked Claude Into Spelling Out a User's Private Data ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#prompt injection`, `#data exfiltration`, `#Claude`, `#security`

---

<a id="item-12"></a>
## [QLoRA Default LR 2e-4 Overfits on Small Datasets, says Reddit](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 8.0/10

A Reddit user argues that the commonly recommended 2e-4 learning rate for QLoRA fine-tuning causes overfitting on datasets under 10k samples, and suggests using 1e-4 instead, backed by personal experiments. This challenges a widely adopted default across tutorials and documentation, potentially saving many practitioners weeks of wasted effort when fine-tuning on small custom datasets. The author reports that reducing the learning rate from 2e-4 to 1e-4 and increasing epochs from 3 to 5 led to significant evaluation improvement, and recommends tuning for datasets between 10k and 30k samples.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA is a parameter-efficient fine-tuning method for large language models that uses quantization and low-rank adapters. The default learning rate of 2e-4 originates from the Alpaca dataset of 52k samples, which is much larger than many custom datasets.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2305.14314">QL O RA: Efficient Finetuning of Quantized LLMs</a></li>
<li><a href="https://oryndex.co/tools/unsloth">Unsloth | Oryndex</a></li>

</ul>
</details>

**Tags**: `#QLoRA`, `#fine-tuning`, `#hyperparameters`, `#learning rate`, `#overfitting`

---

<a id="item-13"></a>
## [ExTernD: Ternary Decomposition for LLM Quantization with Arbitrary Accuracy](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

A new post-training quantization method called ExTernD decomposes each LLM weight matrix into two ternary matrices and a diagonal scaling matrix, enabling variable inner rank to achieve arbitrary accuracy while using only slightly more VRAM than current quantization methods. This approach could significantly improve LLM compression by allowing flexible trade-offs between model size and accuracy, potentially making ternary quantization practical for deployment without severe performance loss. The inner rank in ExTernD can be arbitrarily large to achieve desired accuracy, and the method reportedly uses only slightly more VRAM than standard quantization methods, making the trade-off worthwhile when leveraging ternary arithmetic.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Large language models (LLMs) are often compressed via post-training quantization (PTQ), which converts high-precision weights to lower precision after training. Ternary quantization uses values -1, 0, +1, which enables efficient hardware acceleration but typically suffers from accuracy loss. Matrix decomposition techniques like ExTernD aim to represent a full matrix as a product of smaller matrices to improve representational capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ...</a></li>
<li><a href="https://github.com/phiennd/td">GitHub - phiennd/td: A complete stack to run AI models in ternary ...</a></li>
<li><a href="https://medium.com/data-science-at-microsoft/exploring-quantization-in-large-language-models-llms-concepts-and-techniques-4e513ebf50ee">Exploring quantization in Large Language Models... | Medium</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#ternary`, `#PTQ`, `#model compression`

---

<a id="item-14"></a>
## [Microsoft Comic Chat open-sourced, sparking nostalgia](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

On July 16, 2026, Microsoft released Comic Chat (later known as Microsoft Chat) as open-source software, making the classic graphical IRC client freely available under an open-source license. This open-sourcing preserves a unique piece of internet history and allows developers to study, modify, and potentially revive a nostalgic chat client that was bundled with Windows 98. It also highlights Microsoft's growing engagement with the open-source community. Comic Chat was developed by Microsoft researcher David Kurlander and first released with Internet Explorer 3.0 in 1996. The open-source release was facilitated by Robert Standefer and Scott Hanselman, not the original developer.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: Microsoft Comic Chat was a graphical IRC client that automatically turned text conversations into comic strip panels with characters and emotions. It was an experimental feature of the early web, localized into 24 languages, and bundled with Windows 98, but it extended the IRC protocol in a way that was controversial in the IRC community.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>

</ul>
</details>

**Discussion**: The community comments show strong nostalgia and appreciation, with users sharing personal stories about how Comic Chat inspired their projects. Some technical discussion notes the protocol extension controversy, but overall sentiment is positive about preserving internet history.

**Tags**: `#open source`, `#IRC`, `#Microsoft`, `#history`, `#retro computing`

---

<a id="item-15"></a>
## [Decoy Font: A Font That Fools AI by Hiding Text in Plain Sight](https://www.mixfont.com/experiments/decoy-font) ⭐️ 7.0/10

A designer created 'Decoy Font', a TrueType font that exploits visual multistability to present different text to human viewers and AI vision systems, with the sharp text readable by AI and a blurred hidden message visible to humans. This font demonstrates a novel adversarial attack on AI vision, potentially impacting OCR and AI safety by highlighting vulnerabilities in how models interpret visual data at different spatial frequencies. The font encodes two letters per character using separate spatial frequencies: high-frequency details for one letter and low-frequency shading for another, causing AI models to read the sharp text while humans perceive the blurred message.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Visual multistability is a perceptual phenomenon where an ambiguous stimulus can be interpreted in multiple ways, such as the Necker cube. Decoy Font applies this concept by superimposing two letterforms at different spatial frequencies, exploiting the fact that AI models often focus on high-frequency details and miss low-frequency patterns that humans integrate.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font : A TTF font that hides what you type</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multistable_perception">Multistable perception - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted mixed results: some found that large language models like GPT and Claude could identify the hidden text with prompts, while others pointed out that simple image resizing could break the effect. One commenter claimed a PIL script could fix the font for OCR.

**Tags**: `#font`, `#AI`, `#adversarial examples`, `#OCR`, `#visual perception`

---

<a id="item-16"></a>
## [Book on Mathematics of Data Science Hits arXiv](https://arxiv.org/abs/2607.11938) ⭐️ 7.0/10

A new book titled 'Mathematics of Data Science' has been posted on arXiv, focusing on the mathematical foundations of data science with an emphasis on high-dimensional intuition and statistical thinking. This book provides a rigorous yet accessible foundation for modern data science, helping practitioners and students build the essential mathematical intuition needed for high-dimensional models and statistical reasoning. The book starts with explaining how human intuition fails in high dimensions, covering concepts like spikiness and volume, and connects these to practical topics such as stochastic gradient descent and optimization in high-dimensional spaces.

hackernews · Anon84 · Jul 16, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48939896)

**Background**: Data science is a broad and often overloaded term, encompassing everything from data wrangling to machine learning. A strong mathematical foundation, particularly in statistics and high-dimensional geometry, is critical for making sound decisions and avoiding common pitfalls in data analysis.

**Discussion**: Commenters praised the book's focus on high-dimensional intuition, with one noting it explains why human intuition fails in high dimensions and how that relates to stochastic gradient descent. Another emphasized that statistics remains the top priority skill for data scientists, while a third highlighted that strong basic understanding and good judgment are more important than ever.

**Tags**: `#data-science`, `#mathematics`, `#statistics`, `#high-dimensional`, `#machine-learning`

---

<a id="item-17"></a>
## [Interactive Linear Algebra Book with Dynamic Figures](https://immersivemath.com/ila/) ⭐️ 7.0/10

The book "Immersive Linear Algebra" by J. Ström, K. Åström, and T. Akenine-Möller, published in 2015, is the world's first linear algebra textbook featuring fully interactive figures that readers can manipulate in real time. This interactive approach makes abstract linear algebra concepts intuitive and engaging, potentially improving learning outcomes for students and inspiring similar innovations in other STEM textbooks. The book is freely available online at immersivemath.com and covers standard linear algebra topics with dynamic 3D visualizations; it remains a valuable educational resource despite being published nearly a decade ago.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is foundational in fields like computer science, engineering, and data science, but traditional textbooks rely on static diagrams that can make concepts like vector spaces and transformations hard to grasp. Interactive figures allow learners to rotate, zoom, and adjust parameters, building deeper understanding through exploration.

<details><summary>References</summary>
<ul>
<li><a href="http://immersivemath.com/ila/">Immersive Math</a></li>
<li><a href="https://immersivemath.com/ila/index.html?ref=brainarchives.com">Immersive Math</a></li>

</ul>
</details>

**Discussion**: Commenters are overwhelmingly positive, praising the book's clarity and interactivity, with many wishing it had been available during their own studies. Some suggest that modern AI tools like LLMs could now make creating similar interactive content easier, potentially leading to a new generation of educational resources.

**Tags**: `#linear algebra`, `#education`, `#interactive`, `#mathematics`, `#visualization`

---

<a id="item-18"></a>
## [Seeking Collaborators for Scaling and Evaluation of DABSN Recurrent LM Architecture](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

The author released a preprint and code for DABSN (Dynamic Adaptive Bias State Network), a novel recurrent language model architecture, and is seeking collaborators to scale it further and independently evaluate its performance on language modeling and long-context tasks. If DABSN achieves competitive results at scale, it could offer a more efficient alternative to transformer-based LMs, especially for long sequences, potentially reducing computational costs and enabling new applications in AI. The 24M parameter model was trained on 1B tokens using the GPT-2 tokenizer, and the code is available in PyTorch, C++, and Triton for reproducibility. The preprint covers benchmarks like MQAR, Copy, Key-Value retrieval, and A5/60.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent neural networks (RNNs) process sequences sequentially, which can be more memory-efficient than transformers' attention mechanism for long contexts. DABSN introduces a novel adaptive bias mechanism to improve long-range dependency handling. MQAR (Multi-Query Associative Recall) tests a model's ability to perform associative lookups from multiple cues. Triton is a GPU programming language for writing high-performance kernels.

<details><summary>References</summary>
<ul>
<li><a href="https://triton-lang.org/main/">Welcome to Triton ’s documentation! — Triton documentation</a></li>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR: Multi-Query Associative Recall - Emergent Mind</a></li>

</ul>
</details>

**Tags**: `#recurrent neural networks`, `#language model architecture`, `#open source`, `#collaboration`, `#machine learning research`

---

<a id="item-19"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 7.0/10

A Reddit post questions whether current AI memory architectures should evolve from storing descriptive facts to inferring higher-level reasoning patterns like explanatory frameworks and reasoning styles. This discussion challenges the conventional approach to AI persistent context, potentially leading to more personalized and adaptive AI assistants that understand users' reasoning styles. The post is speculative without concrete examples or empirical data, but it highlights a potential shift from descriptive memory systems (e.g., Mem0) to reasoning-pattern inference, requiring fundamentally different architectures.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Persistent context in AI refers to memory that persists across sessions, such as user preferences or conversation history. Current systems like Mem0 store descriptive facts. Cognitive architectures are blueprints for intelligent agents that model reasoning processes. The post suggests integrating such architectures into memory systems to infer higher-level patterns.

<details><summary>References</summary>
<ul>
<li><a href="https://mem0.ai/">Mem0 - AI Memory Layer for your Agents & Apps | Persistent Context</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cognitive_architecture">Cognitive architecture - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#persistent context`, `#machine learning`, `#cognitive architectures`, `#reasoning patterns`

---

<a id="item-20"></a>
## [Reddit User Seeks Devil's Advocates on JEPA Models](https://www.reddit.com/r/MachineLearning/comments/1uxcryc/looking_for_jepa_devil_advocates_r/) ⭐️ 7.0/10

A Reddit user in the Machine Learning community is actively soliciting critiques and downsides of JEPA-like models for world models in robot learning, noting that Yann LeCun promotes them as the next big thing. This discussion highlights growing skepticism and need for balanced evaluation of JEPA, a promising but still relatively untested architecture, especially as LeCun dismisses other approaches like LLMs and RL. JEPA (Joint Embedding Predictive Architecture) aims to learn abstract representations by predicting in embedding space rather than pixel space, but it faces limitations such as being untested in language modeling and lacking explicit causal modeling.

reddit · r/MachineLearning · /u/Amazing-Coat5160 · Jul 15, 17:34

**Background**: JEPA is a family of self-supervised learning architectures proposed by Yann LeCun, designed to learn world models by predicting masked parts of input in a latent space. World models in robot learning aim to enable robots to simulate and reason about their environment. The user is researching world models and wants to hear counterarguments to LeCun's highly optimistic presentations.

<details><summary>References</summary>
<ul>
<li><a href="https://rohitbandaru.github.io/blog/JEPA-Deep-Dive/">Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru</a></li>
<li><a href="https://www.emergentmind.com/topics/causal-jepa">Causal- JEPA : Causal World Modeling</a></li>
<li><a href="https://www.thesingularityproject.ai/p/yann-lecuns-joint-embedding-predictive">Yann LeCun’s Joint Embedding Predictive Architecture ( JEPA ) and the...</a></li>

</ul>
</details>

**Tags**: `#JEPA`, `#world models`, `#robot learning`, `#Yann LeCun`, `#machine learning`

---

<a id="item-21"></a>
## [PnP-CoSMo: Content/Style Modeling for Multi-Contrast MRI Reconstruction](https://www.reddit.com/r/MachineLearning/comments/1uy2h66/pnpcosmo_a_multicontrast_mri_reconstruction/) ⭐️ 7.0/10

PnP-CoSMo is a plug-and-play framework for multi-contrast MRI reconstruction that learns a content/style model from pure image-domain data, enabling reconstruction without raw k-space data. This work addresses the major bottleneck of requiring raw k-space data for training, which is often unavailable in clinical practice, potentially democratizing advanced MRI reconstruction across different contrasts and scanners. The framework consists of two stages: first, learning a contrast-invariant content and contrast-specific style model from image data; second, using the learned model as a prior in iterative reconstruction. It achieves competitive performance with state-of-the-art unrolled networks without needing k-space data.

reddit · r/MachineLearning · /u/void_gear · Jul 16, 13:10

**Background**: Multi-contrast MRI provides complementary information by acquiring images with different tissue contrasts. Traditional machine learning methods for reconstruction often require raw k-space data, which is not always available. K-space is the Fourier transform space where MRI raw data is stored, and unrolled networks are a common deep learning approach that unrolls an iterative optimization algorithm into a neural network. Content/style modeling separates shared structure (content) from contrast-specific appearance (style).

<details><summary>References</summary>
<ul>
<li><a href="https://www.wikiwand.com/en/articles/K-space_(MRI)">K - space in magnetic resonance imaging - Wikiwand</a></li>
<li><a href="https://www.emergentmind.com/topics/unrolled-networks">Unrolled Networks in Deep Learning</a></li>

</ul>
</details>

**Tags**: `#MRI reconstruction`, `#machine learning`, `#plug-and-play`, `#content modeling`, `#medical imaging`

---

<a id="item-22"></a>
## [MOSBO tools for heterogeneous meta-analysis data](https://www.reddit.com/r/MachineLearning/comments/1uxty9v/best_current_tools_for_multiobjective/) ⭐️ 7.0/10

A Reddit user is seeking recommendations for the best Python stack in 2026 for multi-objective surrogate-based optimization (MOSBO) on heterogeneous meta-analysis data, considering PyMC, pymoo, pysamoo, SMT, and MATLAB. This query highlights the growing need for accessible, efficient MOSBO workflows that combine hierarchical modeling with surrogate-assisted optimization, which is crucial for domains like meta-analysis in sports science or clinical research where multiple objectives and constraints must be balanced. The user requires fine-grained continuous outputs (not grid search) and domain-specific physiological constraints, and prefers Colab-friendly solutions due to using a Chromebook with limited Python experience.

reddit · r/MachineLearning · /u/BleakReason · Jul 16, 05:43

**Background**: Multi-objective surrogate-based optimization (MOSBO) uses surrogate models like Kriging or radial basis functions to approximate expensive objective functions and guide evolutionary algorithms. Python libraries such as pysamoo (surrogate-assisted multi-objective optimization) and SMT (surrogate modeling toolbox) provide ready-to-use implementations. Hierarchical modeling with PyMC can separate protocol effects from baseline effects in meta-analysis, enabling a continuous response surface for optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://pypi.org/project/pysamoo/">pysamoo · PyPI</a></li>
<li><a href="https://smt.readthedocs.io/">SMT : Surrogate Modeling Toolbox — SMT 2.14.2.dev1+g0d3602a74...</a></li>
<li><a href="https://github.com/SMTorg/smt">GitHub - SMTorg/ smt : SMT : The Surrogate Modeling Toolbox · GitHub</a></li>

</ul>
</details>

**Tags**: `#multi-objective optimization`, `#surrogate-based optimization`, `#meta-analysis`, `#hierarchical modeling`, `#Python`

---

<a id="item-23"></a>
## [170x PyTorch slowdown on T4 vs A100: extreme bottleneck explained](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 7.0/10

A user reports a 170x performance drop for a PyTorch point-tracking model on an NVIDIA T4 GPU compared to an A100, despite similar configuration and 99% GPU utilization on the T4. This highlights a critical architectural mismatch: the T4's lack of Tensor Cores for FP32 and drastically lower memory bandwidth (300 GB/s vs 2 TB/s) can cause disproportionate slowdowns for compute-intensive operations like 4D correlation volumes and transformer layers. The model uses pure FP32 precision and builds dense 4D correlation volumes followed by transformer layers, which heavily rely on Tensor Cores and memory bandwidth—both far weaker on T4. The 170x gap far exceeds the typical 6-10x generational difference, indicating a pathological case for T4's architecture.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 (Turing) and A100 (Ampere) are data center GPUs with stark differences: A100 has 312 TFLOPS FP16 (with Tensor Cores) and 2 TB/s memory bandwidth, while T4 has 8.1 TFLOPS FP16 and 300 GB/s. For FP32, A100's Tensor Cores can accelerate matrix operations, but T4 must rely on shader cores, making it much slower for transformer and correlation operations. The 4D correlation volume operation involves extensive matrix multiplications and memory accesses that amplify these architectural differences.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/">PyTorch model running 170x slower on T4 vs A100. What could cause a bottleneck this extreme? [D] : r/MachineLearning - Reddit</a></li>
<li><a href="https://gpuperhour.com/compare/t4-vs-a100">T4 vs A100: 38.5x FP16 Gap, 80GB vs 16GB | GPUPerHour</a></li>

</ul>
</details>

**Tags**: `#PyTorch`, `#GPU performance`, `#T4 vs A100`, `#deep learning optimization`, `#bottleneck`

---

<a id="item-24"></a>
## [Go Library Turns Mermaid Diagrams into Colorful ASCII Art via WebAssembly](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison used Claude Fable 5 to compile the Go library AlexanderGrooff/mermaid-ascii to WebAssembly, enabling browser-based conversion of Mermaid diagrams into ASCII art with color support. This complements an earlier Rust-based tool from Grok Build. This makes Mermaid diagram rendering accessible in text-only environments like terminals and text editors, with color support improving readability. It demonstrates the growing trend of compiling existing libraries to WebAssembly for client-side execution without server dependencies. The tool supports flowcharts, subgraphs, multi-line labels, sequence diagrams, and more, with adjustable padding and box padding. It uses Unicode box-drawing characters and ANSI color codes for rendering.

rss · Simon Willison · Jul 16, 14:57

**Background**: Mermaid is a JavaScript-based diagramming tool that uses text-based definitions to generate diagrams. ASCII art is a graphic design technique that uses characters from the ASCII standard to create images. WebAssembly (Wasm) is a binary instruction format that allows code written in languages like Go to run in web browsers at near-native speed.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/AlexanderGrooff/mermaid-ascii">GitHub - AlexanderGrooff/ mermaid - ascii : Render Mermaid graphs...</a></li>
<li><a href="https://tools.simonwillison.net/mermaid-ascii">Mermaid to ASCII art ( mermaid - ascii )</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#ascii`, `#webassembly`, `#visualization`, `#go`

---

<a id="item-25"></a>
## [Mermaid Diagrams Converted to Unicode Box Art via Rust+WASM](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 6.0/10

Simon Willison built a web tool that compiles a Rust terminal renderer for Mermaid diagrams to WebAssembly, enabling real-time conversion of Mermaid code into Unicode box art in the browser. This tool demonstrates a practical use of WebAssembly to bring a CLI-oriented Rust library to the web, offering a lightweight, dependency-free way to render Mermaid diagrams in text-only environments. It could be useful for developers working in terminals or for embedding diagrams in plain-text documents. The tool is based on the xai-grok-markdown crate from xAI's open-sourced Grok CLI, and was built with assistance from Claude Code (Fable 5). Users can input Mermaid code, see the rendered Unicode art in real time, and copy the result as text or a shareable link.

rss · Simon Willison · Jul 16, 00:33

**Background**: Mermaid is a text-based diagramming tool that allows users to create flowcharts, sequence diagrams, and more using Markdown-like syntax. Unicode box-drawing characters are standard symbols used in terminals to draw lines and boxes. WebAssembly is a binary instruction format that enables high-performance code to run in web browsers.

<details><summary>References</summary>
<ul>
<li><a href="https://mermaid.js.org/">Mermaid | Diagramming and charting tool</a></li>
<li><a href="https://en.wikipedia.org/wiki/Box-drawing_characters">Box -drawing characters - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#unicode`, `#webassembly`, `#rust`, `#tool`

---

<a id="item-26"></a>
## [First RTCA Workshop at NeurIPS 2026 Calls for Papers](https://www.reddit.com/r/MachineLearning/comments/1uy8e0v/cfp_rtca_neurips_2026_r/) ⭐️ 6.0/10

The first Real-Time Conversational Agents (RTCA) Workshop at NeurIPS 2026 has been announced, with a call for papers and demos focusing on real-time multimodal interaction. The workshop will take place on December 11 or 12, 2026 in Sydney, Australia. This workshop addresses the growing need for real-time capabilities in conversational AI, moving beyond offline generation to handle latency, turn-taking, and cross-modal alignment. It will help establish shared benchmarks and methodologies for evaluating naturalness in interactive systems, which is critical for advancing voice assistants, embodied avatars, and live multimodal agents. The workshop accepts full papers (up to 8 pages), short papers (up to 4 pages), and demo papers (up to 2 pages), all using the NeurIPS 2026 style file for double-blind review. It is non-archival, so authors retain the right to publish elsewhere; submission deadline is August 29, 2026.

reddit · r/MachineLearning · /u/Few-Ferret9700 · Jul 16, 16:51

**Background**: Real-time conversational agents aim to interact with humans naturally by streaming speech, video, and language while continuously listening and adapting. This is fundamentally harder than offline generation because it requires low latency, handling turn-taking, backchannels, interruptions, and cross-modal alignment between audio, video, and text. Recent advances like full-duplex models (e.g., NVIDIA PersonaPlex, Meta's synchronous LLMs) and streaming architectures have made this feasible, but the field lacks shared benchmarks and evaluation methods. The RTCA workshop brings together researchers from speech, vision, language, HCI, and ML systems to address these challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://research.nvidia.com/labs/adlr/personaplex/">NVIDIA PersonaPlex: Natural Conversational AI With Any Role and Voice</a></li>
<li><a href="https://ai.meta.com/research/publications/beyond-turn-based-interfaces-synchronous-llms-as-full-duplex-dialogue-agents/">Beyond Turn-Based Interfaces: Synchronous LLMs as Full-Duplex Dialogue Agents | Research - AI at Meta</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#conversational AI`, `#multimodal`, `#workshop`, `#CfP`

---

<a id="item-27"></a>
## [Disentangling Convolutional Neurons with Hadamard Product Clustering](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 6.0/10

A research post introduces a novel method using the Hadamard product of a neuron's receptive field and weights to identify what the neuron detects, then clusters these products to reveal monosemantic clusters (e.g., cars, cats, dogs) and additional low-activation clusters (e.g., letters, human faces). This work provides a new technique for fine-grained analysis of convolutional neurons, potentially improving interpretability of vision models and offering insights into how gradient descent distributes concepts across dependent neurons. The method was applied to a 1x1 convolution layer in InceptionV1, and notably, low-valued activation clusters (like letters) had all their dependent neurons also firing on the same concept, with positive and negative weights balanced to reduce the overall sum.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by understanding individual neurons and circuits. The Hadamard product is an element-wise matrix multiplication that can highlight the alignment between input and weights. In convolutional networks, neurons detect patterns in their receptive field; clustering the Hadamard product reveals distinct patterns the neuron responds to.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://transformer-circuits.pub/2024/scaling-monosemanticity/">Scaling Monosemanticity: Extracting Interpretable Features from...</a></li>
<li><a href="https://www.lesswrong.com/posts/tSNygWGHdpiBvzp4D/rational-animations-intro-to-mechanistic-interpretability">Rational Animations' intro to mechanistic interpretability — LessWrong</a></li>

</ul>
</details>

**Discussion**: The post author notes that starting with convolutions may not attract much attention, and they plan to move to language models. The community may discuss the novelty and utility of the method.

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#interpretability`, `#deep learning`

---