---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 37 items, 18 important content pieces were selected

---

1. [JWST detects atmosphere on rocky exoplanet LHS 1140b](#item-1) ⭐️ 8.0/10
2. [Julia Evans shares SQLite tips: .expert, backups, credentials](#item-2) ⭐️ 8.0/10
3. [Kimi K3: 2.8T Parameter Open-Weight Model Analyzed via Pelican Benchmark](#item-3) ⭐️ 8.0/10
4. [Firefox Runs Inside Browser via WebAssembly Compilation](#item-4) ⭐️ 8.0/10
5. [GPT-5.6 Codex bug deletes user files when $HOME is overridden](#item-5) ⭐️ 8.0/10
6. [Inkling: Open-weights MoE multimodal model from Thinking Machines Lab](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds: AI Is Welcome in Linux Kernel Development](#item-7) ⭐️ 8.0/10
8. [EU AI Act OpenRAG: Legal Chunk Dataset with BGE-M3 Embeddings](#item-8) ⭐️ 8.0/10
9. [New Recurrent Architecture DABSN Seeks Collaborators for Scaling](#item-9) ⭐️ 8.0/10
10. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-10) ⭐️ 8.0/10
11. [ExTernD: Expanded-Rank Ternary Decomposition for LLM Quantization](#item-11) ⭐️ 8.0/10
12. [Kaiser nurses say AI, surveillance harm jobs and care](#item-12) ⭐️ 7.0/10
13. [Zilog Z80 Turns 50: A Retrospective](#item-13) ⭐️ 7.0/10
14. [Stereo2Spatial Converts Stereo Music to Immersive Binaural Mixes](#item-14) ⭐️ 7.0/10
15. [Recurse Center Founder Thanks HN After 15 Years](#item-15) ⭐️ 6.0/10
16. [LLM Cliché Highlighter Tool Launched](#item-16) ⭐️ 6.0/10
17. [Spot birds not golf](#item-17) ⭐️ 6.0/10
18. [Mermaid to ASCII art with color via WebAssembly](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [JWST detects atmosphere on rocky exoplanet LHS 1140b](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

JWST has detected an atmosphere on LHS 1140b, a rocky exoplanet in the habitable zone of a red dwarf star 48 light-years away, ruling out the possibility that it is a mini-Neptune. This marks the first confirmed atmosphere on a potentially habitable rocky exoplanet, offering a prime target for studying habitability beyond our solar system and advancing the search for life. LHS 1140b has a mass 5.6 times Earth's and orbits its M-dwarf star every 24.7 days. The atmosphere detection, made via emission spectroscopy during secondary eclipse, shows signs of a possible nitrogen-rich or water-dominated atmosphere, but further observations are needed to confirm composition.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: LHS 1140b is a super-Earth discovered in 2017, located in the habitable zone of a red dwarf. Red dwarfs are cooler and more active than Sun-like stars, making their inner planets vulnerable to atmospheric stripping. JWST's sensitivity allows detection of thin atmospheres around rocky worlds, a critical step toward assessing habitability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b - Wikipedia</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.theguardian.com/science/2026/jul/16/atmosphere-lhs-1140b-exoplanet-could-water-scientists">Earth-like exoplanet found to have an atmosphere | Space | The Guardian</a></li>

</ul>
</details>

**Discussion**: Commenters noted that red dwarfs' intense stellar activity usually strips atmospheres, making this detection surprising and significant. One expert, citing an arXiv preprint, confirmed that the emission spectroscopy rules out a mini-Neptune classification, validating the rocky nature. Others discussed propulsion for interstellar probes and the Fermi paradox related to communication windows.

**Tags**: `#exoplanets`, `#astronomy`, `#JWST`, `#atmosphere detection`, `#habitable zone`

---

<a id="item-2"></a>
## [Julia Evans shares SQLite tips: .expert, backups, credentials](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 8.0/10

Julia Evans published a blog post with practical tips for running SQLite, including using the .expert command for automatic index recommendations, backup strategies with .dump and compression, and credential management for cloud backups. These tips help developers optimize SQLite performance, avoid common pitfalls like blocking writes during backups, and simplify cloud backup workflows, making SQLite more practical for production use. The .expert command analyzes queries and suggests relevant indexes, which can be created with a single command. Backup tips include using .dump with zstd compression and WAL mode to avoid locking writers. For AWS backups, Simon Willison's s3-credentials tool generates scoped read-only or write-only credentials for a specific S3 bucket.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a lightweight embedded database commonly used in applications and on servers. Its command-line shell provides powerful features like .expert for index recommendations and .dump for backups. WAL (Write-Ahead Logging) mode allows concurrent reads while a writer is active. Managing cloud credentials securely for backups is often cumbersome, hence tools like s3-credentials simplify the process.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/cli.html">Command Line Shell For SQLite</a></li>
<li><a href="https://sqlite.org/backup.html">SQLite Backup API</a></li>
<li><a href="https://sqlite.org/src/file?name=ext/expert/README.md&ci=tip">SQLite: README.md at tip</a></li>

</ul>
</details>

**Discussion**: Commenters shared their own backup scripts, such as using .dump piped to zstd with --rsyncable for efficient syncing, and discussed best practices for large DELETEs like batching and preloading rowids. Simon Willison promoted his s3-credentials tool, receiving positive feedback for solving credential management pain points.

**Tags**: `#SQLite`, `#databases`, `#backups`, `#tools`, `#practical tips`

---

<a id="item-3"></a>
## [Kimi K3: 2.8T Parameter Open-Weight Model Analyzed via Pelican Benchmark](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter open-weight model, with promises of open weights by July 27, 2026. Simon Willison tested it using the pelican benchmark (generating an SVG of a pelican on a bicycle) to probe training data contamination. This is one of the largest open-weight models to date, surpassing DeepSeek's 1.6T model, and its high pricing ($3/$15 per million tokens) marks a shift for Chinese AI labs. The pelican benchmark analysis highlights ongoing concerns about training data contamination in LLM evaluations. Kimi K3 uses 95 input tokens and 16,658 output tokens for the pelican prompt, costing $0.25 per task. Community members noted that the token count discrepancy (95 vs typical 10) suggests an 85-token hidden system prompt, possibly for reasoning effort.

rss · Simon Willison · Jul 16, 20:19 · [Discussion](https://news.ycombinator.com/item?id=48947717)

**Background**: The pelican benchmark is an informal test created by Simon Willison to evaluate LLMs' ability to generate SVG code from a simple prompt. It gained attention as a quick and qualitative way to compare models, but critics argue it may be contaminated since many pelican-on-bicycle SVGs exist online.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/kimi-k3/">Kimi K3, and what we can still learn from the pelican benchmark</a></li>

</ul>
</details>

**Discussion**: Commenters questioned the validity of the pelican benchmark, with OsrsNeedsf2P arguing that pelican SVGs are likely in the training set due to Simon's own blog traffic. devttyeu discovered a possible hidden system prompt from token count anomalies, while btown suggested a more adversarial benchmark combining SWE-bench with SVG generation.

**Tags**: `#AI`, `#LLMs`, `#open-weight models`, `#benchmarks`, `#training data contamination`

---

<a id="item-4"></a>
## [Firefox Runs Inside Browser via WebAssembly Compilation](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 8.0/10

Puter compiled the full Firefox browser to WebAssembly, allowing it to run inside another browser like Chrome. This demonstrates the feasibility of running complex native applications in the browser, with potential implications for sandboxing, cross-platform execution, and browser-in-browser scenarios. The project used the Gecko engine due to its strong single-process support and proxied all network traffic through a WebSocket-based Wisp protocol to satisfy browser security restrictions.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format that enables running compiled code in web browsers at near-native speed. The Wisp protocol is designed to proxy multiple TCP/UDP sockets over a single WebSocket connection, which is necessary because WebAssembly code in a browser cannot open arbitrary network connections directly.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>

</ul>
</details>

**Tags**: `#webassembly`, `#firefox`, `#browser`, `#compilation`, `#web`

---

<a id="item-5"></a>
## [GPT-5.6 Codex bug deletes user files when $HOME is overridden](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

Thibault Sottiaux reported that GPT-5.6 Codex has a bug where, when full access mode is enabled without sandboxing, the model can mistakenly delete the $HOME directory instead of a temporary directory when attempting to override $HOME. This bug poses a serious data loss risk for developers using Codex with full system access, highlighting the dangers of trusting AI coding agents without proper sandboxing and review safeguards. The bug occurs specifically when Codex runs with full access mode enabled and sandboxing protections disabled, including auto-review. The model attempts to set a temporary directory by overriding $HOME but may accidentally delete $HOME.

rss · Simon Willison · Jul 16, 17:45

**Background**: GPT-5.6 Codex is OpenAI's AI coding agent that can autonomously write and execute code. Full access mode allows Codex to interact with the file system without restrictions, while sandboxing provides a security boundary. When sandboxing is bypassed, the model has the same permissions as the user, making such bugs potentially catastrophic.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software... | OpenAI</a></li>
<li><a href="https://www.vincentschmalbach.com/how-codex-cli-flags-actually-work-full-auto-sandbox-and-bypass/">How Codex CLI Flags Actually Work (Full-Auto, Sandbox, and ...</a></li>
<li><a href="https://learn.chatgpt.com/docs/sandboxing?surface=app">Sandbox | ChatGPT Learn</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#GPT-5.6`, `#codex`, `#coding-agents`, `#generative AI`

---

<a id="item-6"></a>
## [Inkling: Open-weights MoE multimodal model from Thinking Machines Lab](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights multimodal Mixture-of-Experts model with 975B total parameters and 41B active, licensed under Apache-2.0. This release strengthens the US open-weights ecosystem, providing a competitive alternative to Chinese open-weight models and offering a strong base for customization via the Tinker training platform. The model is multimodal, trained on 45 trillion tokens of text, images, audio, and video. The model card is relatively brief, and Thinking Machines admits Inkling is not a frontier model but a strong base for fine-tuning.

rss · Simon Willison · Jul 16, 15:35

**Background**: A Mixture-of-Experts (MoE) transformer uses multiple specialized sub-networks ('experts') and a router to activate only a subset per input, enabling high total parameters with low computational cost. Open-weights models make trained parameters publicly available but do not include full training code or data, differing from open-source.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://neysa.ai/blog/open-weights-open-source/">Open Weights vs Open Source : What’s the Real Difference?</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#Mixture-of-Experts`, `#multimodal`, `#large language model`

---

<a id="item-7"></a>
## [Linus Torvalds: AI Is Welcome in Linux Kernel Development](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator of Linux, explicitly stated on the Linux Media mailing list that the Linux project is not anti-AI and considers AI a useful tool. This sets a clear direction for the Linux kernel community, countering growing anti-AI sentiment among some open-source developers. It encourages integration of AI tools into kernel development. Torvalds emphasized that AI is a tool like any other and called for acceptance, threatening a fork if necessary. The statement was made in a July 2026 email on the linux-media mailing list.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds is the creator and maintainer of the Linux kernel, the core of the Linux operating system used worldwide. There has been debate in open-source communities about the role of AI, with some projects rejecting AI-generated contributions. Torvalds' authoritative stance clarifies the kernel's policy.

**Tags**: `#Linux`, `#Linus Torvalds`, `#AI`, `#open source`, `#kernel`

---

<a id="item-8"></a>
## [EU AI Act OpenRAG: Legal Chunk Dataset with BGE-M3 Embeddings](https://www.reddit.com/r/MachineLearning/comments/1uytlac/eu_ai_act_openrag_933_legally_structured_chunks/) ⭐️ 8.0/10

A Reddit user released EU AI Act OpenRAG, a SQLite corpus containing 933 legally structured chunks of the EU AI Act Regulation, each embedded with 1024-dimensional BGE-M3 embeddings, designed for RAG and legal-NLP experimentation. This resource provides a high-quality, structurally chunked legal dataset with precomputed embeddings, enabling more effective retrieval-augmented generation for legal documents, and demonstrates improved retrieval performance over sliding window baselines. The corpus chunks based on legal structure (articles, recitals, definitions, annexes) rather than character windows, includes exact EUR-Lex links and application-date metadata, and the evaluation shows structural chunking achieves recall@20 of 0.541 versus 0.449 for baseline.

reddit · r/MachineLearning · /u/Automatic-Forever-63 · Jul 17, 08:18

**Background**: RAG (Retrieval-Augmented Generation) enhances language models by retrieving relevant document chunks before generating answers. BGE-M3 is a multilingual embedding model from BAAI that supports dense, sparse, and multi-vector retrieval. Legal documents like the EU AI Act require careful chunking to preserve meaning, and this dataset offers a novel structure-based approach.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/BAAI/bge-m3?ref=blog-ko.allganize.ai">BAAI/ bge - m 3 · Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/bge-m3-embedding">BGE M 3 - Embedding : Multilingual Retrieval Model</a></li>

</ul>
</details>

**Tags**: `#RAG`, `#NLP`, `#legal`, `#embeddings`, `#EU AI Act`

---

<a id="item-9"></a>
## [New Recurrent Architecture DABSN Seeks Collaborators for Scaling](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 8.0/10

A novel recurrent architecture called DABSN (Dynamic Adaptive Bias State Network) has been released with preprint and open-source code, and its creator is seeking collaborators for scaling and independent evaluation. If validated, DABSN could offer a competitive alternative to transformers for long-context language modeling, potentially improving efficiency and reasoning capabilities. The open and collaborative approach accelerates research and reproducibility. The architecture has been tested on reasoning, memory, and long-sequence benchmarks (MQAR, Copy, Key-Value retrieval, A5/60), and a 24M-parameter language model was trained on 1B tokens with a GPT-2 tokenizer. Implementations in PyTorch, C++, and Triton are provided.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent neural networks (RNNs) process sequences step-by-step, but often struggle with long-range dependencies. Transformer models excel at long-context tasks but are computationally expensive. DABSN is a new recurrent architecture that aims to combine the efficiency of RNNs with strong long-context performance, as measured by benchmarks like MQAR (Multi-Query Associative Recall).

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR: Multi-Query Associative Recall</a></li>

</ul>
</details>

**Tags**: `#recurrent-neural-networks`, `#architecture`, `#language-modeling`, `#open-source`, `#collaboration`

---

<a id="item-10"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 8.0/10

The post proposes that future AI memory systems should infer and store high-level reasoning patterns and abstractions, such as explanatory frameworks and characteristic reasoning styles, rather than merely descriptive facts about users. If adopted, this shift could lead to AI systems that better understand users' cognitive models, enabling more personalized and adaptive interactions. It challenges current industry focus on vector embeddings and factual retrieval, potentially steering research toward architectures that model human-like abstraction. The post distinguishes between storing descriptive facts (e.g., 'user likes economics') and inferring reasoning styles (e.g., 'user explains economics via incentives and institutions'). It questions whether such representations can emerge naturally from current models or require fundamentally different architectures.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI memory systems typically store persistent context via conversation summaries, user preferences, and vector databases, focusing on factual recall. However, true understanding may require capturing how users reason—patterns of abstraction and explanation. This aligns with ongoing challenges in AI of modeling human-like abstraction and reasoning, as noted in recent research.

<details><summary>References</summary>
<ul>
<li><a href="https://redis.io/blog/ai-agent-memory-stateful-systems/">AI agent memory: types, architecture & implementation</a></li>
<li><a href="https://zylos.ai/research/2026-04-05-ai-agent-memory-architectures-persistent-knowledge/">AI Agent Memory Architectures: From Context Windows to ...</a></li>
<li><a href="https://www.cognee.ai/academy/chapter-1/what-is-ai-memory">What is AI Memory? | Cognee Academy</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#persistent context`, `#machine learning`, `#reasoning styles`, `#abstraction`

---

<a id="item-11"></a>
## [ExTernD: Expanded-Rank Ternary Decomposition for LLM Quantization](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD introduces an expanded-rank ternary decomposition for post-training quantization of large language models, decomposing each weight matrix into two ternary matrices and a diagonal scaling matrix to achieve accuracy approaching any quantization level. This method overcomes the fixed-matrix-size limitation of ternary quantization and offers a practical way to achieve near-full-precision accuracy with only modest additional VRAM, potentially advancing efficient LLM deployment. The inner rank can be arbitrarily large, allowing accuracy to approach any desired level, and the VRAM increase is only slightly more than current quantization methods, making it worth exploiting ternary math.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization reduces the memory footprint of large language models by converting full-precision weights to lower-bit representations. Ternary quantization uses values -1, 0, and +1, but previous methods were limited by fixed matrix size. ExTernD addresses this by decomposing the weight matrix into two ternary matrices and a diagonal scaling matrix, effectively increasing the representational capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD: Expanded - Rank Ternary Decomposition ...</a></li>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded - Rank Ternary Decomposition Ternary LLM...</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#LLM`, `#PTQ`, `#ternary`, `#deep learning`

---

<a id="item-12"></a>
## [Kaiser nurses say AI, surveillance harm jobs and care](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Nurses at Kaiser Permanente report that workplace AI tools, including surveillance and empathy evaluation systems, are increasing pressure and worsening patient care, though some clinicians find value in AI-assisted documentation. This highlights growing tensions between AI-driven efficiency metrics and quality patient care in healthcare, affecting nurse well-being and trust in technology. Complaints center on call center metrics and pressure to ration care, with a 2024 empathy AI pilot since discontinued; however, some clinicians praise LLM tools for live translation and note summarization.

hackernews · gnabgib · Jul 17, 22:26 · [Discussion](https://news.ycombinator.com/item?id=48952880)

**Background**: AI in healthcare includes tools for documentation, diagnosis, and patient interaction, but also surveillance for productivity metrics. Kaiser Permanente is a large managed care consortium that has integrated digital tools, leading to staff concerns about privacy and autonomy.

**Discussion**: Commenters are divided: some criticize the misuse of metrics and empathy evaluations, while others report positive experiences with AI note-taking tools that reduce stress. One commenter noted similar issues at UHC, indicating broader industry trends.

**Tags**: `#AI in healthcare`, `#workplace surveillance`, `#nursing`, `#Kaiser Permanente`, `#ethics`

---

<a id="item-13"></a>
## [Zilog Z80 Turns 50: A Retrospective](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

The Zilog Z80 microprocessor, first launched in July 1976, celebrated its 50th anniversary in 2026, prompting retrospectives on its legacy and impact on early computing. The Z80 was a cornerstone of the microcomputer revolution, powering iconic systems like the TRS-80 and ZX Spectrum, and its longevity in embedded systems underscores its enduring design. The Z80 is binary compatible with the Intel 8080, but with differences in flag register behavior; it also introduced new instructions and registers, making it popular for hobbyists and commercial products.

hackernews · st_goliath · Jul 17, 19:41 · [Discussion](https://news.ycombinator.com/item?id=48951461)

**Background**: The Z80 is an 8-bit microprocessor designed by Zilog and released in 1976. It became widely used in home computers, game consoles, and embedded systems due to its low cost and powerful instruction set. Its influence extended into the 1980s and beyond, with variants still produced for industrial applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zilog">Zilog - Wikipedia</a></li>
<li><a href="https://www.computinghistory.org.uk/det/12157/Zilog-Z-80-Microcomputer-System/">Zilog Z - 80 Microcomputer System - Computer - Computing History</a></li>

</ul>
</details>

**Discussion**: Community comments are nostalgic and appreciative, with users sharing personal stories of learning assembly and building systems around the Z80. Some technical clarifications were noted, such as the flag register incompatibility with the 8080.

**Tags**: `#Z80`, `#CPU`, `#Retrocomputing`, `#History`, `#Hardware`

---

<a id="item-14"></a>
## [Stereo2Spatial Converts Stereo Music to Immersive Binaural Mixes](https://www.reddit.com/r/MachineLearning/comments/1uzevbg/stereo2spatial_convert_stereo_music_tracks_to/) ⭐️ 7.0/10

The author released Stereo2Spatial, a flow-matching diffusion model with memory tokens that converts stereo music tracks into spatialized binaural mixes, available under Apache 2.0 license. This project enables anyone to create high-quality spatial audio from existing stereo recordings, democratizing access to immersive listening experiences without requiring expensive studio equipment. The model initially used a latent VAE (EAR-VAE) but switched to raw waveform modeling with amplitude lifting from WavFlow to stabilize training; it was trained on 7,669 tracks for 20 days on two A6000 GPUs.

reddit · r/MachineLearning · /u/kittenkrazy · Jul 17, 22:55

**Background**: Spatial audio recreates a three-dimensional sound field, making listeners feel sounds come from all around. Binaural audio uses two channels to simulate this effect over headphones. Flow-matching diffusion models generate high-quality audio by gradually converting noise into a target signal, and memory tokens help maintain long-term consistency across audio segments.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/earlab/EAR_VAE">earlab/EAR_VAE · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2601.12950">[2601.12950] ImmersiveFlow: Stereo-to-7.1.4 spatial audio ... Flow — Turn Data Into an Experience Over Your Table www.immersiveflow.com GitHub - immersiveflow/immersiveflow.github.io Packages · immersiveflow · GitHub ImmersiveFlow: Stereo-to-7.1.4 spatial audio generation with ...</a></li>

</ul>
</details>

**Tags**: `#audio processing`, `#diffusion models`, `#spatial audio`, `#machine learning`, `#VAE`

---

<a id="item-15"></a>
## [Recurse Center Founder Thanks HN After 15 Years](https://news.ycombinator.com/item?id=48949551) ⭐️ 6.0/10

The founder of Recurse Center, a free self-directed programming retreat, publicly thanked Hacker News for its crucial role in the organization's founding and 15-year success, sharing that HN has remained the second-largest source of applicants. This milestone underscores the power of online communities like HN in launching and sustaining educational initiatives that prioritize learning over profit, and highlights a sustainable nonprofit model funded by recruiting services. The Recurse Center remains free for all participants, funded by a built-in recruiting agency that charges companies but never deducts from participant salaries. Paul Graham's prescient comment from the original 2011 HN launch noted the 'right sort of crazy' in running free retreats.

hackernews · nicholasjbs · Jul 17, 16:57

**Background**: The Recurse Center (originally Hacker School) was founded in 2010 after a failed startup idea. It runs self-directed programming retreats where participants work on projects, contribute to open source, and learn collaboratively. It has impacted over 3,000 people and is known for its supportive community and social rules.

**Discussion**: Community comments express deep gratitude and nostalgia, with alumni sharing personal transformations and fond memories. One commenter noted the cleverness of hiding the free pricing in the FAQ to filter out those focused solely on cost.

**Tags**: `#Recurse Center`, `#community`, `#programming retreat`, `#startup`, `#YC`

---

<a id="item-16"></a>
## [LLM Cliché Highlighter Tool Launched](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison launched a web tool that detects and highlights common clichés in LLM-generated writing, built using Claude Fable 5 and vibe coding. This tool addresses a growing annoyance among readers of AI-generated content, helping users quickly identify formulaic phrasing. It also demonstrates a practical application of 'vibe coding' with a cutting-edge model. The tool uses the r.jina.ai service to fetch article content from URLs, highlights patterns like 'is real and' and 'worth naming', and offers a 'Show just the highlights' mode. It was created via vibe coding with Anthropic's Claude Fable 5 model.

rss · Simon Willison · Jul 17, 12:11

**Background**: Vibe coding is an AI-assisted development approach where the developer describes the task in a prompt and accepts generated code without thorough review. The tool leverages the r.jina.ai reader API to convert web pages to LLM-friendly markdown. Claude Fable 5, released in June 2026, is Anthropic's most capable model for ambitious coding projects.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_code">Vibe code</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://github.com/jina-ai/reader">GitHub - jina-ai/reader: Convert any URL to an LLM-friendly ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI writing`, `#cliché detection`, `#tools`, `#Simon Willison`

---

<a id="item-17"></a>
## [Spot birds not golf](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 6.0/10

Simon Willison proposes that hyperscalers like Google offset data center water consumption by purchasing golf courses and converting them into public parks for birdwatching. This creative idea highlights a tangible way to address the growing water footprint of AI and cloud computing, sparking discussion on sustainable offsets for data center resource use. Google used 10.9 billion gallons of water in 2025 (~30 million gallons/day), while a single Coachella Valley golf course uses about 750,000 gallons/day; acquiring 40 of the 120 courses could offset Google's daily usage.

rss · Simon Willison · Jul 17, 02:58

**Background**: Hyperscalers are large cloud providers like Google, Amazon, and Microsoft that operate massive data centers requiring vast amounts of water for cooling. An acre-foot is a common water measurement unit equal to about 325,851 gallons. Golf courses in arid regions consume significant water, making them a potential target for water conservation offsets.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperscale_computing">Hyperscale computing - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Acre-foot">Acre-foot - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ai-energy-usage`, `#water conservation`, `#data centers`, `#sustainability`

---

<a id="item-18"></a>
## [Mermaid to ASCII art with color via WebAssembly](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison compiled the Go library mermaid-ascii to WebAssembly, enabling Mermaid diagram conversion to ASCII art with color support directly in the browser. This tool allows developers to embed Mermaid diagrams in text-based environments like terminals or code comments without losing color information, bridging visualization and plain-text workflows. The WebAssembly binary is about 3.7 MB (1.1 MB gzipped) and includes a standard Go runtime; it supports multiple diagram types including flowcharts, sequence diagrams, and subgraphs with customizable padding and box sizes.

rss · Simon Willison · Jul 16, 14:57

**Background**: Mermaid is a popular JavaScript-based diagramming tool that renders Markdown-like text into diagrams. ASCII art conversion translates those diagrams into text characters, useful for environments that cannot display SVG or images. WebAssembly allows Go code to run in the browser at near-native speed.

<details><summary>References</summary>
<ul>
<li><a href="https://tools.simonwillison.net/mermaid-ascii">Mermaid to ASCII art (mermaid-ascii) - tools.simonwillison.net</a></li>
<li><a href="https://github.com/simonw/tools/tree/main/mermaid-ascii">tools/mermaid-ascii at main · simonw/tools · GitHub</a></li>
<li><a href="https://pypi.org/project/mermaid-ascii/">mermaid-ascii · PyPI</a></li>

</ul>
</details>

**Tags**: `#Mermaid`, `#ASCII art`, `#WebAssembly`, `#Go`, `#tool`

---