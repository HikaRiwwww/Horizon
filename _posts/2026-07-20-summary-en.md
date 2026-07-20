---
layout: default
title: "Horizon Summary: 2026-07-20 (EN)"
date: 2026-07-20
lang: en
---

> From 27 items, 15 important content pieces were selected

---

1. [Anthropic Makes Claude Fable 5 Permanent in Max Plans](#item-1) ⭐️ 9.0/10
2. [Blatant AI Slop Wins $25K DeepMind/Kaggle Prize?](#item-2) ⭐️ 9.0/10
3. [Bowling center SRE replaces $120k system with ESP32s](#item-3) ⭐️ 8.0/10
4. [Claude Code Adopts Rust-Based Bun Runtime](#item-4) ⭐️ 8.0/10
5. [Minecraft: Java Edition Adopts SDL3 for Input and Windowing](#item-5) ⭐️ 8.0/10
6. [Alibaba announces Qwen 3.8 open-weights LLM](#item-6) ⭐️ 8.0/10
7. [AI Mania Is Eviscerating Global Decision-Making](#item-7) ⭐️ 8.0/10
8. [Interactive Poincaré ball visualization of GPT-2's token embeddings](#item-8) ⭐️ 8.0/10
9. [Survey of 25 Deep Learning Methods for scRNA-seq](#item-9) ⭐️ 8.0/10
10. [Selling 2,500 MIDI Recorders: Hardware Is Not So Hard](#item-10) ⭐️ 7.0/10
11. [Study: AI advice boosts confidence, hurts accuracy – but flawed](#item-11) ⭐️ 7.0/10
12. [Interactive t-SNE map of GPT-2 token embeddings](#item-12) ⭐️ 7.0/10
13. [SQLite Query Explainer: Interactive Tool via WASM](#item-13) ⭐️ 6.0/10
14. [GPT-2 Small Embedding Geometry Around 'Trump'](#item-14) ⭐️ 6.0/10
15. [TabFM Studio: point-and-click local predictions with tabular AI](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic Makes Claude Fable 5 Permanent in Max Plans](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 9.0/10

Anthropic reversed its plan to remove Claude Fable 5 from subscriptions, instead making it permanent in Max and Team Premium plans beginning July 20, 2026, at 50% of usage limits. This decision shows fierce competition in frontier AI models, as Anthropic responded to pressure from OpenAI's GPT-5.6 Sol and Moonshot AI's Kimi 3, ensuring subscribers retain access to their best model. Fable 5 is now included in the $100/month and $200/month Max plans and Team Premium, but not in the $20/month plan; Pro and Team Standard users receive a one-time $100 credit for API access.

rss · Simon Willison · Jul 18, 06:00

**Background**: Claude Fable 5 is Anthropic's flagship model, excelling in long-horizon reasoning and coding tasks, scoring highest on FrontierBench. Originally planned for API-only access due to compute constraints, the reversal was driven by competition from GPT-5.6 Sol, which outperforms Fable 5 on coding benchmarks at lower cost, and Kimi K3, a 2.8 trillion-parameter model achieving top-three ranking.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>

</ul>
</details>

**Discussion**: The article notes users were previously anxious about losing access to Fable 5, and the permanent inclusion is a relief; the author questions whether Anthropic will need to scale back training to free up GPUs for serving the model.

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#Fable 5`, `#GPT-5.6`

---

<a id="item-2"></a>
## [Blatant AI Slop Wins $25K DeepMind/Kaggle Prize?](https://www.reddit.com/r/MachineLearning/comments/1uzyf66/did_blatant_ai_slop_just_win_a_25k_usd_deepmind/) ⭐️ 9.0/10

A Reddit user claims that a nonsensical submission won the $25,000 grand prize in the Google DeepMind-sponsored Kaggle competition 'Measuring Progress Toward AGI - Cognitive Abilities', alleging failures in the review process. This incident undermines trust in high-profile AI competitions and raises serious questions about peer review and research integrity in the AI community. The user's analysis in two posts highlights that the winning submission was rambling, over ten times the required length, and contained nonsensical methodology; the organizers maintain that the review was proper and the outcome subjective.

reddit · r/MachineLearning · /u/TheWerkmeister · Jul 18, 15:10

**Background**: Kaggle is a platform for data science competitions, often sponsored by companies like DeepMind to crowdsource solutions. This particular competition aimed to design new cognitive-science-based benchmarks for measuring progress toward artificial general intelligence (AGI). The post claims the winning entry lacked coherent arguments and valid code, yet still received the top prize.

**Tags**: `#Kaggle`, `#DeepMind`, `#AI ethics`, `#research integrity`, `#competition`

---

<a id="item-3"></a>
## [Bowling center SRE replaces $120k system with ESP32s](https://news.ycombinator.com/item?id=48968606) ⭐️ 8.0/10

A site reliability engineer replaced a proprietary $120k bowling scoring system with a custom-built solution using ESP32 microcontrollers, costing only $1,600 for 8 lanes. The prototype uses an ESPNow mesh network, Raspberry Pi, and open-source software to handle pin detection, scoring, and animations. This demonstrates that modern embedded systems can replace expensive legacy equipment at a fraction of the cost, reducing vendor lock-in and enabling customization. Small bowling centers and similar venues could affordably modernize and retain control of their data and features. The system uses an ESPNow star-topology mesh with an RS485 wired fallback, communicating with a Raspberry Pi that runs Redis and a state machine. Each lane pair costs about $200 in off-the-shelf parts, and repairs can be done in under 10 minutes by swapping modules.

hackernews · section33 · Jul 19, 14:41

**Background**: Bowling scoring systems are specialized, often costing $80k-$120k for a replacement, using camera-based pin detection and proprietary hardware. ESP32 is a low-cost microcontroller with integrated Wi-Fi and Bluetooth, widely used in IoT projects. The author's project, called OpenLaneLink, is planned to be open-sourced, allowing others to build their own scoring systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digikey.com/es/maker/blogs/2024/a-guide-for-the-esp32-microcontroller-series">A Guide for the ESP 32 Microcontroller Series</a></li>
<li><a href="https://mitsi.com/case-studies/bowling-pin-fall-tracker/">Pinspotters: The Bowling Tracker - Micro Technology Services, Inc.</a></li>

</ul>
</details>

**Discussion**: Commenters shared similar experiences retrofitting old equipment, validating the approach. One commenter noted owning a fully mechanical mini bowling lane and appreciated the relay triggering detail. Another discussed opportunities for retrofitting old machine tools with modern controls. Enthusiastic comments mentioned adding LED lighting and kiosk payment integration.

**Tags**: `#ESP32`, `#embedded systems`, `#bowling`, `#cost optimization`, `#retrofit`

---

<a id="item-4"></a>
## [Claude Code Adopts Rust-Based Bun Runtime](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 8.0/10

Claude Code v2.1.181, released June 17, 2026, now uses the Rust port of Bun, achieving a 10% faster startup on Linux. The Rust version corresponds to Bun v1.4.0 canary, which has not yet been officially released. This change demonstrates a major AI coding tool adopting a runtime rewrite for performance gains, fueling broader discussions about language migration and engineering trade-offs. It also highlights the increasing role of AI in software development, as the rewrite was largely done with AI assistance. Evidence includes binary strings showing 'Bun v1.4.0' and hundreds of Rust source filenames embedded in Claude Code. The Rust rewrite of Bun's 500k-line codebase was completed in 11 days using AI, with the original Zig version still shipping as stable.

rss · Simon Willison · Jul 19, 03:54 · [Discussion](https://news.ycombinator.com/item?id=48966569)

**Background**: Bun is a fast all-in-one JavaScript runtime originally written in Zig. The Rust rewrite aims for improved memory safety and automatic memory management, reducing manual lifecycle tracking bugs. Claude Code is an agentic AI coding tool by Anthropic that works in the terminal, IDE, and desktop app.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/blog/bun-in-rust">Rewriting Bun in Rust | Bun Blog</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/ bun : Incredibly fast JavaScript runtime , bundler...</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**Discussion**: Community reactions are divided: some praise the technical improvements and pragmatic decision, while others criticize the lack of transparent communication and question the necessity of running a TUI over JavaScript. Concerns about Bun's governance and the rapid AI-assisted rewrite also surface.

**Tags**: `#bun`, `#rust`, `#claude-code`, `#runtime`, `#ai-tools`

---

<a id="item-5"></a>
## [Minecraft: Java Edition Adopts SDL3 for Input and Windowing](https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4) ⭐️ 8.0/10

Minecraft: Java Edition's latest snapshot (25w03a) replaces LWJGL's GLFW backend with SDL3 for input and windowing, marking a major shift in the game's cross-platform stack. This move improves input handling, multi-monitor support, and Wayland compatibility, while also simplifying future platform updates. It demonstrates Mojang's commitment to modernizing the game's codebase and engaging with the modding community. The LWJGL SDL3 bindings were contributed by a member of the GTNH modpack team, later merged into LWJGL. Known issues include crashes in exclusive fullscreen on Windows with multiple monitors and on Wayland.

hackernews · ObviouslyFlamer · Jul 19, 11:48 · [Discussion](https://news.ycombinator.com/item?id=48967256)

**Background**: SDL (Simple DirectMedia Layer) is a cross-platform library that abstracts audio, input, and graphics hardware. LWJGL (Lightweight Java Game Library) provides Java bindings for native libraries like GLFW (which Minecraft previously used). SDL3 was released in January 2025 and offers improved performance and features.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SDL3">SDL3</a></li>
<li><a href="https://wiki.libsdl.org/SDL3/FrontPage">SDL3/FrontPage - SDL Wiki</a></li>
<li><a href="https://en.wikipedia.org/wiki/LWJGL">LWJGL</a></li>

</ul>
</details>

**Discussion**: The community praised the contribution from the GTNH modpack team, completing a 'vanilla→modded→vanilla' cycle. Some expressed concern about stability, noting that exclusive fullscreen crashes on Wayland and multi-monitor Windows could block the snapshot. Others saw it as a sign of Minecraft evolving into a game engine.

**Tags**: `#minecraft`, `#sdl3`, `#game-development`, `#cross-platform`, `#lwjgl`

---

<a id="item-6"></a>
## [Alibaba announces Qwen 3.8 open-weights LLM](https://twitter.com/Alibaba_Qwen/status/2078759124914098291) ⭐️ 8.0/10

Alibaba has announced Qwen 3.8, an open-weights large language model with 2.4 trillion parameters, set to be released soon. This announcement follows Moonshot AI's recent reveal of their 2.8T parameter Kimi K3 model, intensifying competition in open-source AI. This marks a significant escalation in the open-weights LLM arms race, offering developers and researchers access to extremely large models. The competition between Alibaba and Moonshot AI is likely to accelerate innovation and lower costs for users. The model has 2.4 trillion parameters and will be released as open-weights, though a specific launch date has not been confirmed. The announcement came via a link to Alibaba Cloud's token pricing page, suggesting a cloud offering may precede the open release.

hackernews · nh43215rgb · Jul 19, 08:44 · [Discussion](https://news.ycombinator.com/item?id=48966120)

**Background**: Open-weights models are large language models whose trained parameters are publicly available for use and modification, though they may not be fully open-source. The race to release ever-larger open models has been heating up, with companies like Alibaba and Moonshot AI pushing boundaries to attract developers and enterprise customers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open-Weights Model? | AI21</a></li>
<li><a href="https://huggingface.co/collections/Qwen/qwen3">Qwen 3 - a Qwen Collection</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed but engaged. Many users are excited about the competition, expecting better models and lower prices. However, one user reported a poor experience with a previous Qwen model for software engineering tasks, while others praised local performance with smaller Qwen variants.

**Tags**: `#LLM`, `#open-weights`, `#Alibaba`, `#Qwen`, `#AI competition`

---

<a id="item-7"></a>
## [AI Mania Is Eviscerating Global Decision-Making](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 8.0/10

Nik Suresh's article exposes how AI hype is causing irrational decisions in large companies, with anonymous anecdotes including executives crafting AI strategies without ever using ChatGPT. This critique highlights the dangerous disconnect between AI enthusiasm and actual competence, potentially leading to wasted resources and misguided priorities across industries. Specific anecdotes include an engineer rewriting a Go repository in Zig solely to appear AI-proficient and keep their job, and a dialogue revealing that enterprise vendors self-censor to avoid undermining customers' AI claims.

rss · Simon Willison · Jul 19, 05:06

**Background**: AI mania refers to the excessive hype surrounding artificial intelligence, where companies rush to adopt AI without understanding it. This can lead to poor decision-making, as executives prioritize appearing AI-savvy over making sound business choices. Zig is a system programming language designed as an alternative to C, known for its focus on robustness and performance. The article provides a behind-the-scenes look at how this dynamic plays out in large organizations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Tags**: `#AI hype`, `#decision-making`, `#technology critique`, `#industry trends`

---

<a id="item-8"></a>
## [Interactive Poincaré ball visualization of GPT-2's token embeddings](https://www.reddit.com/r/MachineLearning/comments/1v0pv45/follow_up_gpt2s_vocabulary_as_a_hyperbolic_tree/) ⭐️ 8.0/10

A user created an interactive 3D visualization of GPT-2's 32,070 token embeddings in a Poincaré ball model of hyperbolic space, allowing exploration by dragging, zooming, and tapping tokens. This layout reveals the hierarchical structure of the vocabulary without any optimization or training. This visualization provides a novel, intuitive way to understand the inherent hierarchy in language model embeddings, which could improve interpretability. It demonstrates the practical application of hyperbolic geometry for representing complex data structures in AI. The visualization uses GPT-2-small's raw token embeddings laid out in hyperbolic space, with Möbius translation for navigation. The vocabulary's similarity structure forms a forest: one giant tree of ~2,300 tokens, hundreds of smaller trees, and ~6,700 isolated tokens.

reddit · r/MachineLearning · /u/Limp-Contest-7309 · Jul 19, 12:54

**Background**: Hyperbolic geometry, specifically the Poincaré ball model, is a non-Euclidean geometry where space expands exponentially from the center, making it ideal for embedding tree-like structures. Poincaré embeddings have been used to learn hierarchical representations of symbolic data. Möbius transformations are isometric motions in hyperbolic space that preserve angles.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1705.08039">[1705.08039] Poincaré Embeddings for Learning Hierarchical Representations</a></li>
<li><a href="https://bjlkeng.io/posts/hyperbolic-geometry-and-poincare-embeddings/">Hyperbolic Geometry and Poincaré Embeddings | Bounded Rationality</a></li>
<li><a href="https://en.wikipedia.org/wiki/Möbius_transformation">Möbius transformation - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#GPT-2`, `#hyperbolic embeddings`, `#visualization`, `#token embeddings`, `#interactive`

---

<a id="item-9"></a>
## [Survey of 25 Deep Learning Methods for scRNA-seq](https://www.reddit.com/r/MachineLearning/comments/1v06nc1/deep_learning_tackles_singlecell_analysis_a/) ⭐️ 8.0/10

A recent survey paper summarizes 25 deep learning methods for single-cell RNA sequencing (scRNA-seq) analysis, categorizing them into six subcategories with detailed comparisons. This structured overview helps researchers select appropriate deep learning tools for scRNA-seq data, advancing cell biology and disease research by improving accuracy in cell classification, trajectory inference, and gene expression analysis. The 25 methods cover tasks such as clustering, imputation, cell type annotation, and gene regulatory network inference, with architectures ranging from autoencoders to graph neural networks.

reddit · r/MachineLearning · /u/teraRockstar · Jul 18, 20:35

**Background**: Single-cell RNA sequencing (scRNA-seq) measures gene expression at the individual cell level, revealing cellular heterogeneity crucial for understanding development and disease. However, scRNA-seq data is high-dimensional, sparse, and noisy, making traditional analysis challenging. Deep learning methods excel at extracting patterns from complex data, offering powerful alternatives for tasks like dimensionality reduction and clustering.

<details><summary>References</summary>
<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/37393865/">Deep learning applications in single-cell genomics and transcriptomics data analysis - PubMed</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11211037/">Highlights of how single - cell analyses are illuminating differentiation...</a></li>

</ul>
</details>

**Tags**: `#deep learning`, `#single-cell RNA-seq`, `#bioinformatics`, `#survey`, `#methods`

---

<a id="item-10"></a>
## [Selling 2,500 MIDI Recorders: Hardware Is Not So Hard](https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard) ⭐️ 7.0/10

Chip Weinberger shares lessons from selling 2,500 JamCorder MIDI recorders, arguing that hardware development can be simpler than perceived with the right approach. This story provides practical insights for software engineers transitioning to hardware, challenging the notion that hardware is inherently difficult and highlighting the feasibility of small-scale hardware entrepreneurship. The JamCorder is a simple device with only 25 components and an injection-molded clamshell case; Weinberger emphasizes that making hardware simple is a design choice, and that scaling concerns can be deferred.

hackernews · chipweinberger · Jul 19, 10:34 · [Discussion](https://news.ycombinator.com/item?id=48966713)

**Background**: MIDI (Musical Instrument Digital Interface) is a technical standard for connecting electronic musical instruments and computers. A MIDI recorder captures performance data (like note on/off, velocity) rather than audio, making it easy to edit and integrate with other gear. The JamCorder is a portable MIDI recorder that stores recordings as MIDI files on a memory card, freeing users from needing a computer or app to work with MIDI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MIDI">MIDI - Wikipedia</a></li>
<li><a href="https://www.homebrewaudio.com/12101/midi-recording-what-is-it-and-why-is-it-awesome/">MIDI Recording - What Is It And Why Is It Awesome? - Home Brew Audio – Home Recording Studio</a></li>

</ul>
</details>

**Discussion**: Commenters generally praise the JamCorder as a well-designed product, with one long-time customer calling it 'basically a perfect product.' However, some push back on the 'hardware is as hard as you make it' statement, arguing that complexity depends on the product requirements, not just design choices. There is also curiosity about anti-counterfeit strategies and the simplicity of the website.

**Tags**: `#hardware`, `#entrepreneurship`, `#product design`, `#lessons learned`

---

<a id="item-11"></a>
## [Study: AI advice boosts confidence, hurts accuracy – but flawed](https://thenextweb.com/news/ai-advice-suppresses-critical-thinking-wrong-answers-study) ⭐️ 7.0/10

A new study claims that receiving advice from AI systems reduces users' accuracy on factual questions while increasing their confidence in wrong answers, but the study's methodology has been heavily criticized. This study touches on the critical question of how AI affects human reasoning and decision-making, but its flawed design may obscure real insights into human-AI interaction. The study used an LLM known to give incorrect answers to certain questions and allowed participants to skip questions if unsure, which critics argue tests only the effect of deliberately bad advice, not typical AI usage.

hackernews · rbanffy · Jul 19, 21:18 · [Discussion](https://news.ycombinator.com/item?id=48971738)

**Background**: Many AI systems, like large language models, can produce confident-sounding but incorrect answers. Studies on AI's impact on human reasoning are becoming common as AI tools are integrated into daily tasks. However, designing rigorous experiments to isolate AI's influence is challenging.

**Discussion**: Commenters criticized the study's methodology, arguing it tests the effect of intentionally bad AI advice rather than typical AI usage. Others noted real-world examples of people uncritically repeating AI-generated answers, highlighting concerns about over-reliance on AI.

**Tags**: `#AI`, `#critical thinking`, `#study`, `#human-AI interaction`, `#methodology`

---

<a id="item-12"></a>
## [Interactive t-SNE map of GPT-2 token embeddings](https://www.reddit.com/r/MachineLearning/comments/1v09muj/interactive_map_of_gpt2s_token_embedding_space/) ⭐️ 7.0/10

A developer released an interactive t-SNE map visualizing the token embedding space of GPT-2 Small, containing 32,070 tokens. Users can tap any token to explore its nearest neighbors via a minimum spanning tree graph. This tool provides an intuitive, visual way to understand how GPT-2 organizes tokens semantically in its embedding space. It is valuable for education and debugging, making abstract NLP concepts accessible to a wider audience. The map uses t-SNE on a compressed representation of the embedding table, with edges representing a minimum spanning tree to show real nearest-kin relationships. No forward pass or context is needed; it works on mobile with pinch-to-zoom and search.

reddit · r/MachineLearning · /u/Limp-Contest-7309 · Jul 18, 22:42

**Background**: Token embeddings are vector representations of tokens learned by language models like GPT-2. t-SNE is a dimensionality reduction technique commonly used to visualize high-dimensional data in 2D. A minimum spanning tree connects all points with the minimum total edge weight, preserving local structure. This interactive map combines these techniques to explore the embedding space.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=JiJYWydfOEk">Input Embedings in GPT 2 , Weight Tying , Demystifying the... - YouTube</a></li>
<li><a href="https://stats.stackexchange.com/questions/587801/embedded-minimum-spanning-trees-for-visualizing-effects-of-dimensionality-reduct">data visualization - Embedded minimum spanning trees for ...</a></li>
<li><a href="https://huggingface.co/transformers/v2.9.1/model_doc/gpt2.html">OpenAI GPT 2 — transformers 2.9.1 documentation</a></li>

</ul>
</details>

**Tags**: `#token embeddings`, `#GPT-2`, `#visualization`, `#t-SNE`, `#NLP`

---

<a id="item-13"></a>
## [SQLite Query Explainer: Interactive Tool via WASM](https://simonwillison.net/2026/Jul/18/sqlite-query-explainer/#atom-everything) ⭐️ 6.0/10

Simon Willison released an interactive web tool that explains SQLite query plans by running SQLite inside Pyodide, a Python runtime compiled to WebAssembly, directly in the browser. The tool adds plain-English explanations to the output of EXPLAIN and EXPLAIN QUERY PLAN commands. This tool addresses a common pain point for developers who find SQLite query plans cryptic and hard to read. By providing explanations in plain language, it lowers the barrier for understanding query optimization and helps users write more efficient SQL queries. The tool runs entirely in the browser using WebAssembly, requiring no server-side processing. However, the author notes that they are not an expert in SQLite query plans and advises users to verify the explanations with official documentation or experimentation.

rss · Simon Willison · Jul 18, 17:19

**Background**: SQLite's EXPLAIN QUERY PLAN command outputs a high-level description of how a query is executed, but the output can be terse and technical. WebAssembly enables running compiled code in browsers at near-native speed, and Pyodide ports CPython to WebAssembly, allowing Python code to run client-side. This tool stacks SQLite, Python, and Pyodide on top of WebAssembly to bring interactive query plan analysis to the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sqlite.org/eqp.html">Explain query plan</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.2</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**Tags**: `#sql`, `#sqlite`, `#webassembly`, `#query-plan`, `#tools`

---

<a id="item-14"></a>
## [GPT-2 Small Embedding Geometry Around 'Trump'](https://www.reddit.com/r/MachineLearning/comments/1v07xai/gpt2_smalls_embedding_geometry_around_trump/) ⭐️ 6.0/10

A visualization compares discretized vs continuous nearest neighbors of the token 'Trump' in GPT-2 Small's static embedding table, showing that discretization leads to generic political terms while continuous embeddings reveal more specific personal and presidential names. This work highlights how quantization in token embeddings can alter semantic relationships, which is crucial for understanding model interpretability and robustness in NLP systems. The analysis projects 32,070 alphabetic tokens via t-SNE and compares nearest neighbors from discretized (coordinate thresholding) vs continuous embeddings; discretized neighbors include Mitt, Hillary, Pelosi, Blair, while continuous neighbors include Obama, Clinton, Bush, Eisenhower.

reddit · r/MachineLearning · /u/Limp-Contest-7309 · Jul 18, 21:29

**Background**: GPT-2 Small uses a static token embedding table learned during training, where each token is represented as a fixed vector in a high-dimensional space. Discretization thresholds each coordinate to 0 or 1 before computing nearest neighbors, while continuous embeddings retain the original float values. This distinction reveals how representation precision affects semantic similarity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.alignmentforum.org/posts/BMghmAxYxeSdAteDc/an-exploration-of-gpt-2-s-embedding-weights">An exploration of GPT-2's embedding weights</a></li>
<li><a href="https://airbyte.com/data-engineering-resources/tokenization-vs-embeddings">Tokenization vs Embedding - How are they Different? | Airbyte</a></li>

</ul>
</details>

**Tags**: `#GPT-2`, `#embeddings`, `#t-SNE`, `#NLP`, `#token analysis`

---

<a id="item-15"></a>
## [TabFM Studio: point-and-click local predictions with tabular AI](https://www.reddit.com/r/MachineLearning/comments/1uzx1el/tabfm_studio_pointandclick_predictions_on/) ⭐️ 6.0/10

TabFM Studio is a new open-source web app that lets users run Google's TabFM tabular foundation model on spreadsheets using a point-and-click interface, without writing any code. This tool greatly lowers the barrier for non-programmers to leverage state-of-the-art tabular foundation models for prediction tasks, potentially enabling wider adoption of AI in data analysis workflows. The app currently supports only Google's TabFM model, but is designed to be extensible. Users upload a CSV or Excel file, select the target column, and the app uses filled rows as in-context examples to predict empty cells.

reddit · r/MachineLearning · /u/Lckylke · Jul 18, 14:15

**Background**: Tabular foundation models like TabFM are AI models trained on large amounts of structured data to perform classification and regression tasks with zero or few examples, similar to how large language models work. In-context learning (ICE) allows the model to use a few labeled examples from the spreadsheet to make predictions on unseen rows without fine-tuning. However, using these models typically requires programming skills, which TabFM Studio aims to eliminate.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>

</ul>
</details>

**Tags**: `#tabular data`, `#foundation models`, `#no-code`, `#machine learning`, `#open source`

---