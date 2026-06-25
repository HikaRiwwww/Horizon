---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 35 items, 20 important content pieces were selected

---

1. [OpenAI Unveils First Custom AI Inference Chip, Jalapeno](#item-1) ⭐️ 9.0/10
2. [Qualcomm Acquires AI Startup Modular](#item-2) ⭐️ 9.0/10
3. [Self-Play RL Agent with ViT and JAX Reaches #1 in Generals.io](#item-3) ⭐️ 9.0/10
4. [Anthropic Accuses Alibaba of Illicit Claude AI Distillation](#item-4) ⭐️ 8.0/10
5. [NVIDIA's 45°C Cooling Cuts Data Center Water Use to Near Zero](#item-5) ⭐️ 8.0/10
6. [Papers with Code Revives OCR Benchmarks Page](#item-6) ⭐️ 8.0/10
7. [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](#item-7) ⭐️ 8.0/10
8. [PR spam on GitHub mirrors early 2000s email spam](#item-8) ⭐️ 7.0/10
9. [Google Introduces Computer Use in Gemini 3.5 Flash](#item-9) ⭐️ 7.0/10
10. [Converting MDN browser compatibility data into a SQLite database](#item-10) ⭐️ 7.0/10
11. [LLM-generated job applications reveal only tool use, not identity](#item-11) ⭐️ 7.0/10
12. [Datasette 1.0a35 Adds JSON APIs for Table Management](#item-12) ⭐️ 7.0/10
13. [MuJoFil: GPU-Accelerated Vision RL Simulator](#item-13) ⭐️ 7.0/10
14. [DeepSWE: Contamination-Free Benchmark for Coding Agents](#item-14) ⭐️ 7.0/10
15. [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](#item-15) ⭐️ 7.0/10
16. [Are ML teams testing model security risks in production?](#item-16) ⭐️ 7.0/10
17. [uv 0.11.24 adds CPython 3.15 beta support and relocatable environments](#item-17) ⭐️ 6.0/10
18. [Blogging Can Be Stating the Obvious](#item-18) ⭐️ 6.0/10
19. [RubyLLM: Unified AI Framework for Ruby](#item-19) ⭐️ 6.0/10
20. [OPFS + Pyodide Test Harness for Datasette Lite](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI Unveils First Custom AI Inference Chip, Jalapeno](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI unveiled its first custom AI inference chip, named Jalapeno, developed in collaboration with Broadcom and manufactured by TSMC, with the design completed in nine months using OpenAI's own AI models. This marks OpenAI's transition from relying on third-party GPUs to designing its own silicon, potentially reducing inference costs and energy consumption while improving performance. It also signals a broader industry trend where AI companies develop custom hardware to optimize for their specific workloads. Jalapeno is an inference-specific chip, meaning it is optimized for running trained models rather than training them. The chip was designed with assistance from OpenAI's own AI models, raising questions about the actual impact of AI-assisted chip design.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI inference chips are specialized processors designed to execute trained AI models efficiently, as opposed to training chips which handle the computationally intensive model training process. Custom application-specific integrated circuits (ASICs) can offer significant performance and efficiency gains over general-purpose GPUs for specific tasks. OpenAI's move into custom chip design mirrors efforts by other tech giants like Google (TPU) and Amazon (Inferentia).

<details><summary>References</summary>
<ul>
<li><a href="https://www.granitefirm.com/blog/us/2025/08/24/ai-inference-chips/">AI inference chips vs. training chips - Andy Lin's Long-term Stock Investment Blog</a></li>
<li><a href="https://www.datacenterknowledge.com/data-center-chips/inference-becomes-the-next-ai-chip-battleground">Inference Becomes the Next AI Chip Battleground</a></li>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community showed mixed reactions: some doubted the significance of AI-assisted design, calling it 'meaningless marketing' without further details, while others raised technical details like TSMC manufacturing and speculated about future chip architectures that embed weights directly into silicon for extreme efficiency.

**Tags**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#semiconductors`

---

<a id="item-2"></a>
## [Qualcomm Acquires AI Startup Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

On June 24, 2026, Qualcomm announced the acquisition of Modular, the company behind the Mojo programming language and the MAX compiler framework, for approximately $4 billion. The deal aims to enhance Qualcomm's AI inference capabilities across edge and cloud devices. This acquisition positions Qualcomm to challenge Nvidia's dominance in AI inference by integrating Modular's compiler technology with Qualcomm's hardware, potentially enabling more efficient AI deployment on ARM and future RISC-V chips. It also signals a strategic shift toward building a software stack that rivals CUDA. The deal is valued at $4 billion according to Reuters. Modular's Mojo language is built on MLIR and targets multiple hardware types including CPUs, GPUs, and ASICs, while the MAX compiler framework focuses on high-performance AI inference.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Modular was founded by Chris Lattner, the original architect of LLVM and Swift, and Tim Davis. Mojo is a programming language that combines Python-like syntax with systems-level performance, leveraging MLIR for multi-target compilation. The MAX compiler provides tools for deploying large language models efficiently across heterogeneous hardware. Qualcomm is a leading chipmaker in mobile and edge AI, currently reliant on ARM architecture but actively exploring RISC-V.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed reactions: some see the acquisition as a strategic move toward RISC-V and AI inference, potentially enabling low-cost inference with Qualcomm's ARM chips. Others question whether it was always the plan to exit or an admission of failure, while Chris Lattner's shift away from making Mojo more Python-like is noted with some disappointment.

**Tags**: `#Qualcomm`, `#Modular`, `#AI`, `#Mojo`, `#acquisition`

---

<a id="item-3"></a>
## [Self-Play RL Agent with ViT and JAX Reaches #1 in Generals.io](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

A self-play reinforcement learning agent using a Vision Transformer architecture and JAX framework achieved superhuman performance in the real-time strategy game Generals.io, ranking #1 on the human 1v1 leaderboard. The project is fully open source, including a fast JAX-based game simulator. This demonstrates that scaling modern architectures like Vision Transformers with JAX can outperform hand-crafted heuristics and prior game-specific algorithms, providing a strong baseline for imperfect-information RTS games. The open-sourced tools lower the barrier for further research in game AI and self-play methods. The agent was trained using self-play reinforcement learning with behavior cloning and reward shaping, but the key improvements were switching from NumPy/Torch to JAX for full pipeline acceleration and replacing CNNs with Vision Transformers. The final agent surpasses the previous best algorithmic agent and consistently beats top human players.

reddit · r/MachineLearning · /u/shrekofspeed · Jun 24, 16:18

**Background**: Generals.io is a fast-paced multiplayer strategy game where players control armies, capture territory, and protect their general. Self-play reinforcement learning involves an agent training by playing against itself to iteratively improve. Vision Transformers apply the transformer self-attention mechanism to image patches, enabling global feature extraction, while JAX is a high-performance Python library for accelerated computation on GPUs/TPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://generals.io/">generals.io</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision_transformer">Vision transformer - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/JAX_(software)">JAX (software) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#reinforcement-learning`, `#self-play`, `#game-ai`, `#vision-transformer`, `#jax`

---

<a id="item-4"></a>
## [Anthropic Accuses Alibaba of Illicit Claude AI Distillation](https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/) ⭐️ 8.0/10

On June 24, 2026, Anthropic publicly accused Alibaba of illicitly extracting capabilities from its Claude AI model through a process called model distillation, allegedly to gain a competitive advantage. This accusation highlights growing tensions over intellectual property in the AI industry, particularly around model distillation as a shortcut for competitors. It raises questions about how to protect proprietary AI models while balancing open innovation. Model distillation involves training a smaller model on the outputs of a larger model to replicate its performance at lower cost. Anonymous commenters suggest that Chinese resellers may have been offering discounted Claude tokens and using user interactions to gather training data.

hackernews · htrp · Jun 24, 19:48 · [Discussion](https://news.ycombinator.com/item?id=48664814)

**Background**: Model distillation is a machine learning technique where knowledge is transferred from a large, complex model to a smaller, more efficient one, often used to deploy AI on resource-limited devices. Claude is a family of large language models developed by Anthropic, known for its focus on safety and ethical guidelines. Anthropic has previously trained Claude on vast amounts of web text, raising questions about the consistency of its position on data usage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Many commenters express irony, noting that Anthropic itself trained Claude on billions of words without compensating copyright holders, and that copying competitors' products is standard industry practice. Others discuss the practical details of how Chinese resellers might be distilling the model via cheap API access.

**Tags**: `#AI ethics`, `#model distillation`, `#IP theft`, `#AI competition`, `#industry news`

---

<a id="item-5"></a>
## [NVIDIA's 45°C Cooling Cuts Data Center Water Use to Near Zero](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA has introduced a 45°C liquid cooling architecture for AI data centers that uses a 75% water and 25% propylene glycol coolant, nearly eliminating water consumption and allowing operation without chillers. This innovation significantly reduces the environmental impact of AI workloads, which are water-intensive, and opens up opportunities for waste heat reuse in district heating systems, lowering operational costs. The coolant runs at 45°C, much warmer than traditional 21-30°C loops, enabling heat rejection to ambient air without chillers. Direct-to-chip cooling is used, and the architecture is designed for NVIDIA's next-generation Rubin GPUs.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Traditional data center cooling uses chillers to drop coolant to 21-30°C, consuming large amounts of electricity and water. Direct-to-chip liquid cooling circulates coolant directly over processors, offering higher efficiency but typically still requires low temperatures. NVIDIA's approach raises the coolant temperature to 45°C, making it viable for heat reuse and reducing water loss from evaporation.

<details><summary>References</summary>
<ul>
<li><a href="https://beyondtmrw.org/article/45c-breakthrough-to-cool-ai-data-center-machines">AI Data Center Liquid Cooling 45C: Hotter Than a Hot Tub</a></li>
<li><a href="https://techstory.in/the-45c-breakthrough-nvidias-liquid-cooling-architecture-solves-data-center-water-crisis/">NVIDIA Liquid Cooling Design Cuts Water to Near Zero - TechStory</a></li>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45°C Liquid Cooling Design for AI Data Centers</a></li>

</ul>
</details>

**Discussion**: The community is largely positive, highlighting the potential for district heating synergies and reduced water usage. Some commenters question the novelty, noting that similar high-temperature cooling has been used before, and others ask for more details on climate dependencies and pump limits.

**Tags**: `#data center cooling`, `#liquid cooling`, `#NVIDIA`, `#energy efficiency`, `#sustainability`

---

<a id="item-6"></a>
## [Papers with Code Revives OCR Benchmarks Page](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 8.0/10

The maintainer of Papers with Code has created a curated page listing top open-source OCR models and benchmarks, including recent releases from Baidu (Unlimited OCR with R-SWA) and Mistral (OCR 4 via API). This centralized resource helps AI practitioners easily find and compare state-of-the-art OCR models, which is crucial for digitizing documents and enabling agentic RAG applications. The page features benchmarks like OlmOCRBench and OmniDocBench, with top models including Chandra OCR 2 and Mistral OCR v4; Baidu's Unlimited OCR uses only 500M activated parameters out of 3B total.

reddit · r/MachineLearning · /u/NielsRogge · Jun 24, 16:26

**Background**: OCR (Optical Character Recognition) converts scanned documents and PDFs into machine-readable text. Recent advances in large language models have spurred new OCR architectures like Baidu's R-SWA (Reference Sliding Window Attention) and DeepSeek OCR, which inspired Unlimited OCR. Sliding window attention reduces computational cost by limiting each token's context window, enabling efficient processing of long documents.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/BaiduAI_News/status/2069322806748410291">Baidu AI on X: "We’re open-sourcing Unlimited OCR — built to read long documents in one pass. With 3B total parameters and only 500M activated, Unlimited OCR sets new end-to-end SOTA results on OmniDocBench v1.5 and v1.6. The key innovation is Reference Sliding Window Attention (R-SWA), https://t.co/cBRqmyRUKN" / X</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>

</ul>
</details>

**Tags**: `#OCR`, `#Open-Source`, `#Benchmarks`, `#AI Agents`, `#RAG`

---

<a id="item-7"></a>
## [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 8.0/10

The author introduces HDD-RoPE, a novel positional embedding that uses cumulative matrix products and data-dependent rotation, achieving faster convergence on the TinyStories dataset compared to the xPos baseline. This work challenges the traditional pair-wise rotation in rotary position embeddings by enabling multi-dimensional position representations, potentially improving transformers' ability to model hierarchical structures like paragraphs or sentences. HDD-RoPE breaks query and key vectors into chunks of arbitrary size (e.g., 4) and applies data-dependent rotations along multiple axes, effectively representing position in a multi-dimensional space. The implementation is available in an open-source repository with code and mathematical details.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 24, 18:16

**Background**: Rotary Position Embedding (RoPE) encodes relative position by rotating pairs of dimensions in queries and keys at fixed frequencies, limiting position to a one-dimensional linear sequence. HDD-RoPE generalizes this by allowing arbitrary chunk sizes and dynamic rotation rates based on the data, enabling the model to learn position within higher-level structures.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2305.07759">[2305.07759] TinyStories: How Small Can Language Models Be ... TinyStories · Datasets roneneldan/TinyStories at main - Hugging Face TinyStories Dataset | vizuaraai/nano-gpt-oss | DeepWiki GitHub - raymond-van/gpt-tinystories: Reproducing GPT on the ... GitHub - xingvu/TinyStories: Creating a mini GPT-2 model from ...</a></li>

</ul>
</details>

**Tags**: `#positional embedding`, `#rotary position encoding`, `#transformer`, `#machine learning research`, `#deep learning`

---

<a id="item-8"></a>
## [PR spam on GitHub mirrors early 2000s email spam](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

The article draws a parallel between the rise of spam pull requests on GitHub and the early 2000s email spam epidemic, prompting community discussion on reputation systems and maintainer controls. This issue directly affects open source maintainers by wasting their time and degrading project quality. Understanding the historical analogy may help the community adopt effective anti-spam mechanisms before the problem escalates. GitHub recently added configurable pull request limits for maintainers, but community members point out that unlike email spam, GitHub spam cannot be traced to individual users via server reputation. Some suggest building reputation infrastructure similar to email, while others question the motivation behind PR spam.

hackernews · dakshgupta · Jun 24, 14:32 · [Discussion](https://news.ycombinator.com/item?id=48660579)

**Background**: A Pull Request (PR) is a request to contribute code changes to an open source project. Spam PRs are meaningless or malicious submissions that burden maintainers. In the early 2000s, email spam overwhelmed users until reputation systems (e.g., sender scores), blacklists, and filtering tools brought it under control. This news argues that open source communities may need similar defenses against PR spam.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/marketplace/spampr">Spampr · GitHub Marketplace</a></li>
<li><a href="https://github.com/marketplace/actions/check-and-reject-spam-prs">Check and reject spam PRs - GitHub Marketplace</a></li>
<li><a href="https://github.com/orgs/community/discussions/53233">What should I do about spam issues or pull requests? · community · Discussion #53233</a></li>

</ul>
</details>

**Discussion**: Commenters noted that GitHub already introduced PR limits, but one argued that email spam control relied on server-level reputation which doesn't apply to individual GitHub users. Another user questioned the motivation (e.g., karma farming). Some called for unsubscribe lists akin to uBlock Origin, and a former anti-spam worker shared historical insights.

**Tags**: `#open source`, `#GitHub`, `#spam`, `#maintainers`, `#community`

---

<a id="item-9"></a>
## [Google Introduces Computer Use in Gemini 3.5 Flash](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 7.0/10

Google has announced that Gemini 3.5 Flash now includes a computer use capability, allowing the AI to autonomously operate a computer by mimicking mouse and keyboard actions. However, user reports indicate frequent task failures and unpredictable behavior. This feature positions Gemini among other AI models like Anthropic's Claude and OpenAI's GPT that are competing in autonomous computer interaction. The reported reliability issues could undermine user trust and adoption for real-world automation tasks. The computer use capability in Gemini 3.5 Flash is designed for tasks like form filling and file management. Users have reported that the model aborts tasks after exceeding error thresholds, executes dangerous commands like 'git reset --hard' without confirmation, and lacks support for Model Context Protocol (MCP) in the app.

hackernews · swolpers · Jun 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48662999)

**Background**: Computer use is a capability that allows AI models to interact with a computer's graphical user interface as a human would, by clicking buttons, typing, and navigating between applications. Google's Gemini 3.5 Flash is a lightweight model that balances speed and performance, positioning it for developer workflows. Similar features have been introduced by Anthropic for Claude and by OpenAI for GPT-5.4.

<details><summary>References</summary>
<ul>
<li><a href="https://theoutpost.ai/news-story/anthropic-unveils-groundbreaking-computer-use-ai-for-autonomous-task-performance-7482/">Anthropic Unveils Groundbreaking ' Computer Use ' AI for Autonomous...</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.5 Flash — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: Community comments reveal significant frustration: one user reported Gemini gave up after many iterations and explicitly said it invents data. Another user experienced Gemini running 'git reset --hard' unexpectedly. Some users are skeptical about benchmark graphs and request features like MCP support or a coding agent comparable to Codex.

**Tags**: `#Gemini`, `#AI`, `#LLM`, `#computer use`, `#Google`

---

<a id="item-10"></a>
## [Converting MDN browser compatibility data into a SQLite database](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 7.0/10

Simon Willison used AI-assisted coding tools (Claude Code Opus 4.8 and Codex Desktop GPT-5.5) to create a script that converts MDN's browser-compat-data into a SQLite database, and hosted it on GitHub with open CORS headers for easy access. This tool provides developers with offline and fast queryable access to browser compatibility data, simplifying web development workflows. It also demonstrates a practical use of AI-generated code for automating data conversion and hosting. The resulting database is about 66MB and is stored in a GitHub orphan branch named 'db' to leverage GitHub's CORS headers. It can be explored interactively using Datasette Lite.

rss · Simon Willison · Jun 24, 23:59

**Background**: MDN (Mozilla Developer Network) provides a comprehensive browser-compat-data repository that tracks which web features are supported by different browsers. However, querying this data traditionally requires parsing JSON files. Simon Willison's tool converts it into a SQLite database, enabling SQL queries. The MDN MCP service was recently introduced, which also provides access to this data via the Model Context Protocol.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/blog/introducing-mdn-mcp-server/">Introducing the MDN MCP server - MDN Web Docs</a></li>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ...</a></li>

</ul>
</details>

**Tags**: `#browser-compatibility`, `#sqlite`, `#AI-tools`, `#web-development`, `#data-tools`

---

<a id="item-11"></a>
## [LLM-generated job applications reveal only tool use, not identity](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright observed that many recent job applications are co-written by LLMs, featuring LLM-generated portfolios, projects, and commit messages, resulting in generic and impersonal submissions. This highlights a growing challenge for hiring managers to assess candidates' true skills and authenticity, as LLMs enable applicants to mask their identity behind polished but hollow content. MacWright notes that these applications tell him nothing about the person except which tools they use, leading to a sense of 'accidental anonymity' where candidates disappear behind the AI.

rss · Simon Willison · Jun 24, 18:13

**Background**: Large language models (LLMs) like GPT-4 are increasingly used to generate text for resumes, cover letters, and even code. This trend raises concerns about authenticity in hiring, as perfect but impersonal submissions become common. MacWright's commentary reflects a broader anxiety in tech communities about AI eroding personal expression and merit evaluation.

**Tags**: `#careers`, `#AI`, `#hiring`, `#authenticity`, `#LLM`

---

<a id="item-12"></a>
## [Datasette 1.0a35 Adds JSON APIs for Table Management](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 introduces new 'Create table' and 'Alter table' interfaces backed by JSON APIs, allowing users to manage database schemas programmatically. This release significantly enhances Datasette's capability as a data publishing tool by enabling schema modifications through a web interface and API, making it more flexible for dynamic data management. The new JSON APIs at '/<database>/-/create' and '/<database>/<table>/-/alter' support defining columns, primary keys, constraints, defaults, foreign keys, and table renames. Additionally, the template context documentation is now stabilized as a stable API for custom templates.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing data, created by Simon Willison. It turns any SQLite database into an instant web interface with powerful exploration features and JSON APIs, without requiring code. This alpha release continues to expand its schema management capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette : An open source multi- tool for exploring and publishing data</a></li>
<li><a href="https://tds.s-anand.net/2025-09/data-analysis-with-datasette/">Data Analysis With Datasette • Tools in Data Science</a></li>
<li><a href="https://www.toolmage.com/en/tool/datasette/">Datasette : Open-Source Tool for Data Exploration and API Publishing</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#JSON API`, `#database`, `#alpha`

---

<a id="item-13"></a>
## [MuJoFil: GPU-Accelerated Vision RL Simulator](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 7.0/10

MuJoFil, a new open-source simulator, combines Nvidia's Newton physics engine (GPU-native MuJoCo) with Google's Filament renderer to enable high-fidelity, parallelized vision-based reinforcement learning training directly on GPU. This addresses the limitations of existing simulators: MuJoCo's CPU-bound physics, MJX's lack of vision support, and Isaac's accessibility issues. MuJoFil offers an accessible, open-source alternative for training vision-based policies at scale. MuJoFil uses Nvidia's Newton (built on Warp) for GPU-accelerated physics, and a heavily modified Filament for parallel rendering with PBR texture support. It supports importing environments in GLB, OpenUSD, etc., and is available via pip as 'mujofil' (CPU) and 'mujofil-warp' (GPU/CUDA).

reddit · r/MachineLearning · /u/MT1699 · Jun 24, 19:07

**Background**: MuJoCo is a popular physics simulator for robotics, but its CPU-based computation limits parallelism. MJX, a GPU-accelerated variant, lacks rendering for vision RL. Nvidia's Newton (open-source, GPU-native MuJoCo) and Google's Filament (PBR renderer) provide the building blocks. MuJoFil integrates both to create a complete vision RL training pipeline.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://google.github.io/filament/dup/intro.html?trk=article-ssr-frontend-pulse_little-text-block">Introduction - Filament</a></li>
<li><a href="https://github.com/newton-physics/newton">GitHub - newton-physics/newton: An open-source, GPU ...</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#simulation`, `#MuJoCo`, `#GPU`, `#vision`

---

<a id="item-14"></a>
## [DeepSWE: Contamination-Free Benchmark for Coding Agents](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 7.0/10

A new benchmark called DeepSWE has been released that evaluates frontier models on code writing tasks using contamination-free, original prompts spanning 91 repositories across 5 languages. DeepSWE addresses critical flaws in existing benchmarks like data contamination and lack of real-world complexity, providing a more reliable evaluation of how well AI coding agents perform in actual software engineering tasks. Prompts are roughly half the length of SWE-bench Pro's but require 5.5 times more code and about twice as many output tokens; verifiers are hand-written to test software behavior rather than implementation details.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Benchmarks for AI code generation often suffer from data contamination, where models have seen solutions during pretraining, leading to inflated performance. SWE-bench and its variants are popular but have limitations in diversity and contamination. DeepSWE aims to fix these issues by creating original tasks from scratch and hand-writing verifiers to ensure robust evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.net/">DeepSWE Benchmark : GPT vs Claude for Agentic Coding</a></li>
<li><a href="https://www.swebench.com/original.html">SWE-bench</a></li>

</ul>
</details>

**Discussion**: No comments were available for analysis in the provided data.

**Tags**: `#benchmark`, `#LLM`, `#code generation`, `#software engineering`, `#evaluation`

---

<a id="item-15"></a>
## [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 7.0/10

A Reddit user compiled a spreadsheet comparing LLM inference pricing across 7 providers, including OpenRouter, DeepSeek, Together AI, Fireworks, and Groq, revealing that cached input pricing can be tens of times cheaper than uncached input. This matters because developers running workloads with reusable context—such as agents with large system prompts, RAG pipelines, or multi-turn conversations—can achieve significant cost savings by selecting providers with favorable caching policies, making caching a more important factor than headline token price. The spreadsheet tracks input/output token pricing, context windows, cached input pricing where available, and supported models. It does not include real throughput, cold-start times, precision variants (FP16/FP8), or egress costs.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 24, 11:28

**Background**: LLM inference pricing typically charges per token for input and output. Many providers offer a discount for cached input tokens that are reused across requests (cache hits). The depth of discount and transparency varies widely; this comparison highlights those differences and their practical impact on cost-sensitive applications.

<details><summary>References</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/deepseek-reasonix-cuts-inference-cost-5x-with-9982-cache-hit">DeepSeek Reasonix cuts inference cost 5x with 99.82% cache hit</a></li>
<li><a href="https://www.cloudzero.com/blog/deepseek-pricing/">DeepSeek pricing 2026: V4, R1, API costs, and how to optimize</a></li>
<li><a href="https://benchlm.ai/llm-pricing">LLM API Pricing Comparison 2026 — Cost Per Token for GPT ...</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#pricing`, `#caching`, `#cost optimization`, `#providers`

---

<a id="item-16"></a>
## [Are ML teams testing model security risks in production?](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

A Reddit user questions whether machine learning teams perform adversarial testing, such as model extraction and data poisoning, before deploying models in production, highlighting a perceived gap in security practices compared to traditional software. As ML models become prevalent in critical applications, failure to test for extraction and poisoning risks could lead to intellectual property theft, data breaches, and compromised model integrity. This discussion underscores the need for standardized security reviews in ML pipelines. Model extraction attacks aim to steal a model's functionality by querying its API, while data poisoning attacks corrupt training data to manipulate model behavior. The post notes that many ML teams skip adversarial testing before deployment.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Adversarial machine learning studies attacks like evasion, extraction, and poisoning that exploit vulnerabilities in ML models. Model extraction attacks allow adversaries to create a surrogate model by observing outputs, while data poisoning involves injecting malicious samples into training data. Traditional software security practices like penetration testing are well-established, but equivalent measures for ML models are less common. The Reddit post reflects a growing awareness of this gap.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_poisoning_attack">Data poisoning attack</a></li>
<li><a href="https://arxiv.org/html/2502.16065v1">A Survey of Model Extraction Attacks and Defenses in ...</a></li>
<li><a href="https://developers.google.com/machine-learning/guides/adv-testing">Adversarial Testing for Generative AI | Machine Learning ...</a></li>

</ul>
</details>

**Tags**: `#model security`, `#adversarial testing`, `#production ML`, `#ML pipelines`, `#extraction attacks`

---

<a id="item-17"></a>
## [uv 0.11.24 adds CPython 3.15 beta support and relocatable environments](https://github.com/astral-sh/uv/releases/tag/0.11.24) ⭐️ 6.0/10

uv 0.11.24 introduces support for CPython 3.15.0b3 and a preview feature that makes project environments relocatable. It also includes performance improvements like a compact index for lazy version maps and several bug fixes. This update keeps uv aligned with the latest Python beta releases, allowing early adopters to test upcoming Python versions. The relocatable environments feature, once stable, will simplify deployment by enabling users to move entire project environments without breaking paths. The relocatable environment feature is still in preview, meaning it may change in future releases. The compact index for lazy version maps optimizes memory usage when resolving dependencies, which is particularly beneficial for large projects.

github · github-actions[bot] · Jun 23, 21:16

**Background**: uv is a fast Python package and project manager created by Astral, written in Rust. It aims to be a drop-in replacement for pip and pip-tools, offering significantly faster dependency resolution and installation. The tool also supports project management features like lockfiles and workspaces, similar to Poetry or Rye.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/uv">GitHub - astral-sh/ uv : An extremely fast Python package and project ...</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release`, `#performance`

---

<a id="item-18"></a>
## [Blogging Can Be Stating the Obvious](https://blog.jim-nielsen.com/2026/blogging-stating-the-obvious/) ⭐️ 6.0/10

Jim Nielsen published a blog post arguing that stating the obvious in blogging is valuable because what seems obvious to one person may be new and insightful to others. This perspective encourages more people to share their knowledge without fear of being redundant, potentially enriching the overall quality of online discourse and knowledge sharing. The post is a reflection rather than a technical breakthrough, and it received 114 upvotes and 45 comments on a social news aggregator, indicating moderate engagement.

hackernews · Curiositry · Jun 24, 23:46 · [Discussion](https://news.ycombinator.com/item?id=48666927)

**Background**: Blogging as a form of knowledge sharing often faces the 'curse of knowledge,' where experts assume what they know is common. This post challenges that assumption by arguing that stating the obvious can be helpful.

**Discussion**: Commenters shared personal experiences: one noted that online studies stating the obvious spark 'well obviously' replies but can lead to deeper discussion; another mathematician recalled losing enthusiasm after becoming an expert; a user who had a popular post reported being told it was 'not new' but still received many upvotes and positive comments.

**Tags**: `#blogging`, `#knowledge sharing`, `#writing`, `#community`, `#philosophy`

---

<a id="item-19"></a>
## [RubyLLM: Unified AI Framework for Ruby](https://rubyllm.com/) ⭐️ 6.0/10

RubyLLM is a Ruby gem that provides a single, elegant interface for multiple major AI providers including OpenAI, Anthropic, Google, and Ollama. It aims to simplify AI integration for Ruby developers by abstracting away provider-specific API differences. For Ruby developers, RubyLLM reduces the complexity of working with multiple AI APIs, allowing easy provider switching and faster prototyping. Its clean design lowers the barrier to building AI-powered applications in the Ruby ecosystem. The gem has only three dependencies: Faraday, Zeitwerk, and Marcel. Community feedback highlights some pain points, such as incomplete cache support for xAI and the responses API not being natively supported until recent updates. Despite these, it is praised for usability and extensibility.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: Ruby developers historically lacked a unified tool for integrating with LLM providers, often having to write custom wrappers or use language-agnostic HTTP clients. RubyLLM fills this gap by offering a consistent API similar to Vercel's AI SDK for JavaScript, enabling seamless interaction with various models.

<details><summary>References</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers.</a></li>
<li><a href="https://medium.com/@raviskit2012/rubyllm-the-ruby-gem-that-makes-ai-feel-right-at-home-a34a1d18def4">RubyLLM : The Ruby Gem That Makes AI Feel Right at Home | Medium</a></li>

</ul>
</details>

**Discussion**: Community sentiment is generally positive, with users praising the framework's ease of use and design. However, concerns were raised about maintainer responsiveness to pull requests, merging of low-quality PRs ("vibe coded"), and specific technical issues like cache handling and observability instrumentation.

**Tags**: `#Ruby`, `#AI framework`, `#LLM`, `#developer tools`, `#open source`

---

<a id="item-20"></a>
## [OPFS + Pyodide Test Harness for Datasette Lite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison built a test harness to explore using the Origin Private File System (OPFS) with Pyodide, aiming to enable Datasette Lite to edit persistent SQLite files in the browser. This exploration could allow running Python-based data tools like Datasette entirely client-side with persistent storage, reducing server dependence and enabling offline data analysis. The test harness leverages OPFS, which provides a sandboxed filesystem per origin, and Pyodide's WebAssembly-based Python runtime to attempt SQLite file editing directly in the browser.

rss · Simon Willison · Jun 23, 18:58

**Background**: Datasette Lite is a version of the Datasette data exploration tool that runs entirely in the browser using Pyodide and WebAssembly. The Origin Private File System (OPFS) is a browser API that provides a private, origin-specific filesystem for persistent storage. Combining these could enable browser-based applications to save and edit files like SQLite databases without a server.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN - MDN Web Docs</a></li>
<li><a href="https://web.dev/articles/origin-private-file-system">The origin private file system | Articles | web.dev</a></li>
<li><a href="https://pyodide.com/">Home - Pyodide</a></li>

</ul>
</details>

**Tags**: `#browsers`, `#pyodide`, `#datasette-lite`, `#OPFS`, `#WebAssembly`

---