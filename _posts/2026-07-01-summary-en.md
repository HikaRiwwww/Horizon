---
layout: default
title: "Horizon Summary: 2026-07-01 (EN)"
date: 2026-07-01
lang: en
---

> From 35 items, 23 important content pieces were selected

---

1. [Claude Code embeds steganographic markers in requests](#item-1) ⭐️ 9.0/10
2. [Google's Agentic AI Peer-Reviewer Handles ~10K Papers, Catches 34% More Errors](#item-2) ⭐️ 9.0/10
3. [Anthropic Releases Claude Sonnet 5 with Mixed Community Reception](#item-3) ⭐️ 8.0/10
4. [US lifts export controls on Anthropic's Claude Fable 5 and Mythos 5](#item-4) ⭐️ 8.0/10
5. [Anthropic launches Claude Science for secure data science](#item-5) ⭐️ 8.0/10
6. [CERN enters Long Shutdown 3 to upgrade LHC for high luminosity](#item-6) ⭐️ 8.0/10
7. [Ngrok ports Kubernetes to the browser](#item-7) ⭐️ 8.0/10
8. [DIY mmWave Radar for Material Classification Faces Challenges](#item-8) ⭐️ 8.0/10
9. [Interactive map of 11M scientific papers using SPECTER2 and UMAP](#item-9) ⭐️ 8.0/10
10. [EML Trees Proven Universal Approximators](#item-10) ⭐️ 8.0/10
11. [DeepMind Releases Nano Banana 2 Lite, Faster and Cheaper Image Generator](#item-11) ⭐️ 7.0/10
12. [Mistral Releases Leanstral 1.5 for Lean 4 Theorem Proving](#item-12) ⭐️ 7.0/10
13. [shot-scraper video: New tool records agent demos automatically](#item-13) ⭐️ 7.0/10
14. [Ornith-1.0: Open-Weight Agentic Coding Model Delivers SOTA Performance](#item-14) ⭐️ 7.0/10
15. [REAP: Automatically Curating Coding Agent Benchmarks from Production Data](#item-15) ⭐️ 7.0/10
16. [Cerebras-OpenAI Deal Eats Inference Capacity, Stranding Startups](#item-16) ⭐️ 7.0/10
17. [HEMA Practitioner Builds Open Dataset for AI Swordfighting Tracking](#item-17) ⭐️ 7.0/10
18. [uv 0.11.26 released with performance boosts](#item-18) ⭐️ 6.0/10
19. [Google Copybara: Moving Code Between Repositories](#item-19) ⭐️ 6.0/10
20. [Brain2Qwerty: Non-Invasive Brain-to-Text AI](#item-20) ⭐️ 6.0/10
21. [MARS2 Workshop on Multimodal Reasoning at ECCV 2026](#item-21) ⭐️ 6.0/10
22. [Improving 5-Class Diabetic Retinopathy Model on APTOS 2019](#item-22) ⭐️ 6.0/10
23. [Why NCE over MLE for Instance Representation Learning?](#item-23) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Claude Code embeds steganographic markers in requests](https://thereallo.dev/blog/claude-code-prompt-steganography) ⭐️ 9.0/10

A discovery reveals that Anthropic's Claude Code tool uses steganography to embed tracking information in the AI requests it sends, potentially to monitor unauthorized usage or model distillation. This raises serious concerns about transparency and trust for developers using AI coding tools, and could impact adoption of Claude Code while fueling broader debate on ethical monitoring practices in the industry. The steganographic markers are hidden within the text of requests sent to Anthropic's servers, making them invisible to normal inspection; the technique was reverse-engineered and publicly disclosed by a third party.

hackernews · kirushik · Jun 30, 15:44 · [Discussion](https://news.ycombinator.com/item?id=48734373)

**Background**: Steganography is the practice of concealing messages within other data, unlike cryptography which makes messages unreadable. Claude Code is an agentic coding tool from Anthropic that runs in the terminal and helps developers edit files, run commands, and understand codebases, all while communicating with Anthropic's cloud servers.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Steganography">Steganography - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community is divided: some criticize Anthropic for lack of transparency and deceptive practices, while others see the intent (e.g., preventing model distillation) as understandable. A few recommend open-source alternatives like Codex CLI to avoid such issues.

**Tags**: `#steganography`, `#AI`, `#Anthropic`, `#security`, `#ethics`

---

<a id="item-2"></a>
## [Google's Agentic AI Peer-Reviewer Handles ~10K Papers, Catches 34% More Errors](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

Google deployed an agentic AI peer-reviewer at ICML and STOC that reviewed approximately 10,000 papers with a 30-minute turnaround, and the formal research paper reveals it catches 34% more mathematical errors than zero-shot prompting. This sets a precedent for AI-assisted peer review at conference scale, potentially reducing reviewer workload and improving review quality, especially for mathematical correctness. The agentic system operates autonomously within defined constraints, using tools and multi-step reasoning. It was tested on real submissions to top computer science conferences, demonstrating practical feasibility and significant improvement over baseline methods.

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Jun 29, 10:05

**Background**: Agentic AI refers to AI systems that can pursue goals, use tools, and take actions with varying degrees of autonomy, unlike simple prompting. Peer review is a critical but time-consuming process in academic publishing. This work shows that AI can assist at scale, catching errors that human reviewers might miss.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://paperreview.ai/">Stanford Agentic Reviewer - Submit Paper</a></li>
<li><a href="https://github.com/debashis1983/agentic-paper-review">GitHub - debashis1983/agentic-paper-review: Agentic Paper Reviewer ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#peer review`, `#machine learning`, `#research automation`

---

<a id="item-3"></a>
## [Anthropic Releases Claude Sonnet 5 with Mixed Community Reception](https://www.anthropic.com/news/claude-sonnet-5) ⭐️ 8.0/10

Anthropic has released Claude Sonnet 5, positioned as the most agentic Sonnet model yet, with enhanced tool use and autonomous planning capabilities. This release underscores the industry shift toward agentic AI, where models take autonomous actions, but the community debate over cost-performance versus the more powerful Opus model could influence developer adoption. According to community benchmarks, Sonnet 5's cost per task at high effort levels exceeds that of Opus, and it shows regression in vulnerability discovery tasks (scoring 0 with default safeguards).

hackernews · marinesebastian · Jun 30, 17:59 · [Discussion](https://news.ycombinator.com/item?id=48736605)

**Background**: Claude models are named after literary genres: Haiku, Sonnet, Opus, and Fable. Sonnet is typically a mid-range model balancing speed and capability, while Opus is Anthropic's most powerful model. Agentic AI refers to systems that pursue goals autonomously over multiple steps without per-step human approval.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://claude-manual.com/en/getting-started/model-comparison">Claude Model Comparison — Opus , Sonnet, or... | Claude Manual</a></li>

</ul>
</details>

**Discussion**: Community comments are critical: several users note that Sonnet 5's cost-performance is worse than Opus at medium and high effort levels, and some benchmarks show regressions compared to previous versions. One user describes Sonnet 5 as 'GLM-5.2 level' but at 2x cost, while another finds it worse on price/performance than GLM 5.2.

**Tags**: `#Anthropic`, `#Claude Sonnet 5`, `#AI model release`, `#agentic AI`, `#LLM`

---

<a id="item-4"></a>
## [US lifts export controls on Anthropic's Claude Fable 5 and Mythos 5](https://twitter.com/AnthropicAI/status/2072106151890809341) ⭐️ 8.0/10

The US Department of Commerce lifted export controls on Anthropic's Claude Fable 5 and Mythos 5 models on June 30, 2026, following safety improvements. Claude Fable 5 is now generally available, while Mythos 5 is restricted to select businesses and cybersecurity experts. This policy change signals a shift in US AI regulation, potentially enabling broader access to advanced models while raising concerns about predictability and security for businesses. It may affect trust in American frontier AI models and influence global AI development. Claude Fable 5, a Mythos-class model made safe for general use, cannot initially be used for coding tasks such as debugging, which fall back to Opus 4.8. Claude Mythos 5, designed to find software vulnerabilities, remains restricted to authorized users.

hackernews · Pragmata · Jun 30, 23:55 · [Discussion](https://news.ycombinator.com/item?id=48740771)

**Background**: Export controls restrict the transfer of dual-use AI technologies to foreign entities. Anthropic had initially withheld Claude Mythos from public release due to misuse concerns. The lifting of controls follows Anthropic's coordination with the US government to mitigate risks, including deploying classifiers to block cybersecurity tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.bbc.com/news/articles/cdr42623e1do">Fable and Mythos : Anthropic says US lifts export ban on its advanced...</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration over lack of predictability in AI regulation, with users noting that businesses cannot rely on SOTA models due to shifting policies. Some highlight that Claude Fable 5 cannot be used for coding, and a letter from Commerce reveals the controls were lifted after Anthropic addressed risks, but the process remains opaque.

**Tags**: `#AI regulation`, `#export controls`, `#Anthropic`, `#policy`

---

<a id="item-5"></a>
## [Anthropic launches Claude Science for secure data science](https://claude.com/product/claude-science) ⭐️ 8.0/10

Anthropic launched Claude Science, a web-based workbench for data science and research computing that runs a local server on the user's machine and integrates with HPC clusters and databases. This provides a secure environment for processing sensitive data, especially in regulated industries like pharmaceuticals, and streamlines research workflows by consolidating multiple tools into one platform. Claude Science uses a local server architecture with a web UI, enabling it to run entirely on the user's hardware and connect to institutional clusters and databases without sending data to the cloud.

hackernews · lebovic · Jun 30, 17:07 · [Discussion](https://news.ycombinator.com/item?id=48735770)

**Background**: Traditional data science platforms often rely on cloud-based processing, which can raise data privacy issues in fields like life sciences. Claude Science addresses this by keeping computation local while still providing a modern, AI-assisted interface. It is not a new AI model but a workflow platform that integrates existing scientific tools and packages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-science-ai-workbench">Claude Science, an AI workbench for scientists, is now available</a></li>
<li><a href="https://techcrunch.com/2026/06/30/anthropics-claude-science-bets-on-workflow-not-a-new-model-to-win-over-scientists/">Anthropic’s Claude Science bets on workflow, not a new model, to win over scientists | TechCrunch</a></li>

</ul>
</details>

**Discussion**: Community members appreciated the local server architecture for secure environments, with one user highlighting integrations with institutional HPC. However, there were criticisms about scientific accuracy, such as a test in RNAi biopesticide design yielding only basic results and a concern that the AI might 'degenerate' in bioscience contexts.

**Tags**: `#Anthropic`, `#Claude`, `#data science`, `#HPC`, `#scientific computing`

---

<a id="item-6"></a>
## [CERN enters Long Shutdown 3 to upgrade LHC for high luminosity](https://home.cern/cern-bids-farewell-to-the-lhc-and-enters-long-shutdown-3/) ⭐️ 8.0/10

CERN has officially begun Long Shutdown 3 (LS3) of the Large Hadron Collider (LHC), which will last until 2030 and involve a major upgrade to the High-Luminosity LHC (HL-LHC), aiming to increase collision rates tenfold. This upgrade will dramatically increase the number of collisions, allowing physicists to study rare processes and the Higgs boson in unprecedented detail, potentially leading to new discoveries in fundamental physics. During LS3, thousands of specialists from CERN and partner institutes will transform the LHC, its injectors, and experiments into their HiLumi versions, while also renovating the entire accelerator complex. The HL-LHC is expected to produce up to 380 million Higgs bosons over its lifetime.

hackernews · HelloUsername · Jun 29, 18:52 · [Discussion](https://news.ycombinator.com/item?id=48723484)

**Background**: The Large Hadron Collider (LHC) is the world's largest and most powerful particle accelerator, located at CERN near Geneva. It operates in runs interspersed with long shutdowns for maintenance and upgrades. Long Shutdown 3 (LS3) is the third such shutdown, following Run 3 which ended in 2026. The HL-LHC upgrade will increase the integrated luminosity by a factor of 10 beyond the LHC's design value, enabling studies of rare processes and precise measurements of known particles.

<details><summary>References</summary>
<ul>
<li><a href="https://home.cern/cern-bids-farewell-to-the-lhc-and-enters-long-shutdown-3/">CERN bids farewell to the LHC and enters Long Shutdown 3 – Home | CERN</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Luminosity_Large_Hadron_Collider">High Luminosity Large Hadron Collider</a></li>
<li><a href="https://home.cern/science/accelerators/hilumi-lhc/">HiLumi LHC – Home | CERN</a></li>

</ul>
</details>

**Discussion**: Commenters expressed both excitement and technical curiosity about the upgrade. One noted the scale of the ATLAS Inner Tracker (ITk) upgrade with 5 billion channels, while another highlighted that CERN now stores over 1 exabyte of collision data. A few debated the historical cancellation of the Superconducting Super Collider (SSC), and one suggested the title was overly dramatic since the LHC is not being retired, just upgraded.

**Tags**: `#physics`, `#CERN`, `#LHC`, `#particle accelerators`, `#high-energy physics`

---

<a id="item-7"></a>
## [Ngrok ports Kubernetes to the browser](https://ngrok.com/blog/i-ported-kubernetes-to-the-browser) ⭐️ 8.0/10

Ngrok released 'Wébernetes', a project that runs a full Kubernetes cluster inside the browser using WebAssembly containers, enabling interactive learning and AI-driven development testing. This lowers the barrier for learning Kubernetes and allows developers to test AI-generated code against a real K8s environment without provisioning infrastructure, potentially improving code quality and educational accessibility. The project simulates core Kubernetes components (API server, controller manager, scheduler) as WebAssembly modules, each running in separate browser workers. It does not run actual containers but emulates their behavior for educational purposes.

hackernews · peterdemin · Jun 30, 20:48 · [Discussion](https://news.ycombinator.com/item?id=48738985)

**Background**: Kubernetes (K8s) is an open-source container orchestration platform that automates deployment, scaling, and management of containerized applications. WebAssembly (Wasm) is a binary instruction format designed to run high-performance applications in browsers and other environments. By combining these, Wébernetes makes K8s concepts accessible without requiring a cloud cluster.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cncf.io/blog/2024/03/12/webassembly-on-kubernetes-from-containers-to-wasm-part-01/">WebAssembly on Kubernetes: from containers to Wasm (part 01) | CNCF</a></li>
<li><a href="https://www.nops.io/blog/how-to-run-webassembly-on-kubernetes/">How to Run WebAssembly on Kubernetes - nOps</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kubernetes">Kubernetes - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community praised the project for its educational potential, especially for hands-on K8s learning. Some questioned whether it actually runs containers in the browser, with replies clarifying it emulates container behavior via Wasm. The workflow of testing AI-generated code against a real cluster was highlighted as a novel use case.

**Tags**: `#kubernetes`, `#browser`, `#education`, `#ai-assisted`, `#ngrok`

---

<a id="item-8"></a>
## [DIY mmWave Radar for Material Classification Faces Challenges](https://gauthier-lechevalier.com/radar) ⭐️ 8.0/10

A developer built a mmWave radar prototype for material classification, aiming to detect asbestos but finding limited sensitivity and consistency in distinguishing materials. This project highlights the potential of low-cost mmWave radar for material identification, which could impact safety inspections (e.g., asbestos) if sensitivity challenges are overcome. The radar uses 60-64 GHz frequency and relies on signal reflection patterns; however, the prototype has not yet demonstrated reliable detection of asbestos at low concentrations.

hackernews · GL26 · Jun 30, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48736137)

**Background**: mmWave radar operates at millimeter wavelengths (30-300 GHz), offering high precision for short-range sensing. Previous research has used 60-GHz radar combined with deep learning to classify materials (e.g., wood, plastic, metal) based on reflected signal patterns. This project extends that concept to asbestos detection but requires higher sensitivity for practical use.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Radar">Radar - Wikipedia</a></li>
<li><a href="https://www.researchgate.net/publication/336086706_Material_Classification_using_60-GHz_Radar_and_Deep_Convolutional_Neural_Network">(PDF) Material Classification using 60-GHz Radar and Deep...</a></li>
<li><a href="https://sesamedisk.com/mmwave-radar-material-classification-industrial/">Millimeter-Wave Radar for Material - Sesame Disk</a></li>

</ul>
</details>

**Discussion**: Commenters debated the actual risk of asbestos in sealed walls (deepsun), praised the learning value of publishing failures (tim-tday), and suggested alternative approaches like discontinuity detection (jcims). Some questioned whether the core challenge of asbestos detection was addressed (ghostly_s).

**Tags**: `#mmWave`, `#radar`, `#material classification`, `#hardware`, `#DIY`

---

<a id="item-9"></a>
## [Interactive map of 11M scientific papers using SPECTER2 and UMAP](https://www.reddit.com/r/MachineLearning/comments/1ujn3u5/a_map_of_the_latest_11_million_papers_split_by/) ⭐️ 8.0/10

A free interactive map of 11 million scientific papers has been created, using SPECTER2 embeddings and UMAP dimensionality reduction to visualize research fields and trends over time. This tool enables researchers to quickly grasp the macroscopic landscape of scientific literature, identify emerging trends, and explore related work through semantic similarity, which is especially valuable given the rapid growth of publications. The map is built from titles and abstracts of papers sourced from OpenAlex and Arxiv, encoded with SPECTER2, projected to 2D via UMAP, with Voronoi labels around high-density peaks. It supports keyword and semantic searches, institutional/author/topic analytics, and a time slider for temporal exploration.

reddit · r/MachineLearning · /u/icannotchangethename · Jun 30, 11:55

**Background**: SPECTER2 is a state-of-the-art model for generating scientific document embeddings, trained on diverse tasks and fields. UMAP is a dimensionality reduction technique that preserves local and global structure, often used for visualizing high-dimensional data. Combining these allows semantic relationships between papers to be mapped in a 2D space.

<details><summary>References</summary>
<ul>
<li><a href="https://allenai.org/blog/specter2-adapting-scientific-document-embeddings-to-multiple-fields-and-task-formats-c95686c06567">SPECTER2: Adapting scientific document embeddings to multiple fields and task formats | Ai2</a></li>
<li><a href="https://umap-learn.readthedocs.io/">UMAP: Uniform Manifold Approximation and Projection for Dimension Reduction — umap 0.5.8 documentation</a></li>

</ul>
</details>

**Tags**: `#scientific literature`, `#visualization`, `#NLP`, `#machine learning`, `#open science`

---

<a id="item-10"></a>
## [EML Trees Proven Universal Approximators](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 8.0/10

A paper proves a universal approximation theorem for EML trees, showing they can approximate a wide class of functions using a constructive LEGO-block approach. This is a significant theoretical contribution that extends universal approximation results to a new class of models, potentially impacting function approximation and machine learning by providing a novel framework. The proof includes explicit constructions of binary operations, polynomials, hyperbolic tangent, and approximate partitions of unity, and addresses technical difficulties like the ill-definedness of natural logarithm for nonpositive inputs using sign-based decompositions.

reddit · r/MachineLearning · /u/JoeGermany · Jun 29, 11:16

**Background**: The EML function represents elementary functions through composition. This paper generalizes it to EML trees with learnable parameters and proves universal approximation. Universal approximation theorems are fundamental in machine learning, showing that certain models can approximate any function arbitrarily well.

**Tags**: `#machine learning`, `#approximation theory`, `#universal approximation`, `#EML trees`

---

<a id="item-11"></a>
## [DeepMind Releases Nano Banana 2 Lite, Faster and Cheaper Image Generator](https://deepmind.google/models/gemini-image/flash-lite/) ⭐️ 7.0/10

Google DeepMind has released Nano Banana 2 Lite, a distilled version of its image generation model that is significantly faster and cheaper than the base Nano Banana 2 model. This release makes advanced image generation more accessible for developers and hobbyists due to lower cost and faster inference, while also sparking discussions about ethical use in real estate listings and other applications. The model generates images in under 5 seconds compared to 30 seconds for the base Nano Banana 2, but it lacks some capabilities like programmatic aspect ratio control and performs worse on highly nuanced prompts.

hackernews · minimaxir · Jun 30, 16:48 · [Discussion](https://news.ycombinator.com/item?id=48735444)

**Background**: Nano Banana 2 Lite is a distilled version of Google's Nano Banana 2 image generation model, which was made generally available in May 2026 alongside Nano Banana Pro. Distillation reduces model size and computational requirements, enabling faster and cheaper inference at the cost of some quality and flexibility.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/30/google-introduces-a-faster-cheaper-image-generator-with-nano-banana-2-lite/">Google introduces a faster, cheaper image generator with Nano Banana 2 Lite | TechCrunch</a></li>
<li><a href="https://cloud.google.com/blog/products/ai-machine-learning/nano-banana-2-and-nano-banana-pro-are-generally-available">Nano Banana 2 and Nano Banana Pro available for everyone | Google Cloud Blog</a></li>

</ul>
</details>

**Discussion**: The community reception is mixed: developers praise the speed and text rendering, but criticize the requirement for a Google One account, limitations on aspect ratio control, and concerns about misuse in real estate listings. Some users also noted the omission of ChatGPT in comparison charts.

**Tags**: `#AI`, `#image generation`, `#DeepMind`, `#model release`, `#machine learning`

---

<a id="item-12"></a>
## [Mistral Releases Leanstral 1.5 for Lean 4 Theorem Proving](https://docs.mistral.ai/models/model-cards/leanstral-1-5-26-06) ⭐️ 7.0/10

Mistral AI released Leanstral 1.5, an updated specialized language model designed to assist with theorem proving in the Lean 4 proof assistant. This release strengthens the tooling for formal verification and mathematical reasoning, enabling more reliable AI-assisted programming and proof development. It particularly benefits researchers and developers working with Lean 4, which is gaining traction in both academia and industry. Leanstral 1.5 is a specialized model that likely improves upon the previous Leanstral-2603, which was a Mixture-of-Experts model. It is available on Hugging Face and can be used with the Vibe harness, as noted by a community member who released an updated OpenATP package.

hackernews · vetronauta · Jun 30, 20:44 · [Discussion](https://news.ycombinator.com/item?id=48738938)

**Background**: Lean 4 is a proof assistant and functional programming language used for formal mathematics. Leanstral is an open-weight LLM from Mistral fine-tuned to generate Lean 4 code and proofs, aiming to bridge LLMs and formal verification. The first version, Leanstral, was released in March 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://huggingface.co/mistralai/Leanstral-2603">mistralai/Leanstral-2603 · Hugging Face</a></li>
<li><a href="https://webkul.com/blog/mistrals-leanstral/">Leanstral: Mistral's Open-Source AI for Trustworthy Coding - Webkul Blog</a></li>

</ul>
</details>

**Discussion**: Community members responded positively, with one promptly releasing an OpenATP Python package supporting Leanstral 1.5. Others noted the model's specialization for Lean 4 rather than similar provers like Coq, and some debated Mistral's general performance compared to other models.

**Tags**: `#Mistral`, `#Lean 4`, `#theorem proving`, `#LLM`

---

<a id="item-13"></a>
## [shot-scraper video: New tool records agent demos automatically](https://simonwillison.net/2026/Jun/30/shot-scraper-video/#atom-everything) ⭐️ 7.0/10

Simon Willison released shot-scraper 1.10 with a new `shot-scraper video` command that records video demos of web application interactions using Playwright, driven by a `storyboard.yml` file. This tool enables AI coding agents to automatically produce video demos of their work, helping developers verify and showcase agent-created features efficiently. The command accepts a `storyboard.yml` file defining server setup, URL, viewport, cursor visibility, wait conditions, custom JavaScript, and a series of scenes with actions like pause, click, and text input.

rss · Simon Willison · Jun 30, 16:54

**Background**: shot-scraper is a command-line tool built on Playwright for taking automated screenshots and scraping web pages. The new video feature extends it to record full interactions, allowing agents to create demos that prove their code works.

<details><summary>References</summary>
<ul>
<li><a href="https://shot-scraper.datasette.io/">shot-scraper</a></li>
<li><a href="https://simonwillison.net/2022/Mar/10/shot-scraper/">shot-scraper: automated screenshots for documentation, built on Playwright</a></li>

</ul>
</details>

**Tags**: `#developer-tools`, `#video-demos`, `#shot-scraper`, `#playwright`, `#agents`

---

<a id="item-14"></a>
## [Ornith-1.0: Open-Weight Agentic Coding Model Delivers SOTA Performance](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 7.0/10

DeepReinforce released Ornith-1.0, a family of open-weight LLMs (MIT licensed) for agentic coding, achieving state-of-the-art results on coding benchmarks. It includes variants from 9B to 397B parameters, built on Gemma 4 and Qwen 3.5. This is significant because it is the first model to use self-scaffolding, learning to generate both solutions and task-specific harnesses, potentially advancing autonomous coding agents. Its open weights and MIT license make it accessible for the open-source community. The model uses a self-improving training framework that jointly optimizes the scaffold and solution, discovering better search trajectories. The 35B MoE variant can run on consumer hardware with GGUF quantization (20GB).

rss · Simon Willison · Jun 29, 16:17

**Background**: Self-scaffolding means the model learns to create its own code-generation harnesses instead of relying on human-designed ones. Agentic coding refers to AI agents that autonomously plan, write, test, and modify code with minimal human intervention. This model builds on two existing open-weight base models, Gemma 4 and Qwen 3.5, both Apache 2.0 licensed.

<details><summary>References</summary>
<ul>
<li><a href="https://deep-reinforce.com/ornith_1_0.html">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding | DeepReinforce Blog | Jun. 2026</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-source`, `#coding`, `#agentic AI`

---

<a id="item-15"></a>
## [REAP: Automatically Curating Coding Agent Benchmarks from Production Data](https://www.reddit.com/r/MachineLearning/comments/1uk713d/reap_automatic_curation_of_coding_agent/) ⭐️ 7.0/10

REAP (Relevance and Execution-Audited Pipeline) introduces an automated pipeline that constructs production-derived benchmarks for coding agents from real developer-agent sessions without manual labeling. This addresses a critical need for realistic, continuously updated benchmarks to evaluate LLM-based coding agents, reducing the gap between lab tests and real-world performance. The pipeline automatically curates relevant tasks from interactive production usage logs and audits them through execution validation to ensure correctness and reproducibility.

reddit · r/MachineLearning · /u/julian88888888 · Jul 1, 00:50

**Background**: Coding agents are AI tools that assist developers by writing or editing code. Traditional benchmarks for these agents are often manually curated or static, limiting their relevance to real-world scenarios. REAP automates the curation using production data, enabling benchmarks that reflect actual developer workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.01527">[2604.01527] REAP : Automatic Curation of Coding Agent...</a></li>

</ul>
</details>

**Tags**: `#benchmark curation`, `#coding agents`, `#production data`, `#LLM evaluation`, `#machine learning`

---

<a id="item-16"></a>
## [Cerebras-OpenAI Deal Eats Inference Capacity, Stranding Startups](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 7.0/10

A small AI startup revealed that Cerebras' exclusive deal with OpenAI to supply $20 billion worth of chips has pre-allocated the vast majority of its near-term inference capacity, effectively making its API waitlist indefinite for smaller companies. This deal highlights how large-scale hardware agreements can crowd out startups relying on specialized AI inference hardware, potentially stifling innovation in real-time AI applications and deepening the concentration of AI compute power among hyperscalers. The deal reportedly involves Cerebras supplying its wafer-scale chips to OpenAI, leaving minimal capacity for other customers, and startups needing high-throughput, low-latency inference for production workloads are most impacted.

reddit · r/MachineLearning · /u/Kortopi-98 · Jun 29, 12:00

**Background**: Cerebras builds wafer-scale engines (WSE), which are massive single chips designed for AI training and inference, offering high throughput and low latency compared to traditional GPUs. However, production capacity is limited, and major deals can consume most available output. This deal with OpenAI reportedly amounts to $20 billion, effectively locking up Cerebras' near-term capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion reflects widespread frustration among startups, with many expressing concern that exclusive deals with hyperscalers will make it nearly impossible for smaller players to access cutting-edge hardware. Some commenters suggest diversifying hardware options or seeking alternatives like Groq or specialized clouds.

**Tags**: `#AI inference`, `#Cerebras`, `#OpenAI`, `#hardware shortage`, `#startup challenges`

---

<a id="item-17"></a>
## [HEMA Practitioner Builds Open Dataset for AI Swordfighting Tracking](https://www.reddit.com/r/MachineLearning/comments/1uivddx/i_do_historical_swordfighting_and_noticed_ai/) ⭐️ 7.0/10

A historical swordfighter (HEMA practitioner) is creating an open multi-view dataset with synchronized high-speed cameras (120/240fps) to help AI track fast-moving, occluded swordfighting. They shared a proposed annotation schema on Hugging Face and are requesting community feedback. This dataset could help bridge the Sim2Real gap for embodied AI by providing extreme real-world motion scenarios. It may improve AI tracking of fast, occluded objects in sports, robotics, and other domains. The dataset will include 100 hyper-trimmed clips annotated with biomechanics, frame-level keypoints, segmentation masks, and computer vision hazards such as occlusion ratings. The schema includes weapon type, historical source, footwork, and strike trajectory.

reddit · r/MachineLearning · /u/fonssagrives · Jun 29, 15:16

**Background**: HEMA (Historical European Martial Arts) involves fencers wearing heavy jackets and using steel blades that can move at 80 mph, causing severe motion blur and occlusion. The Sim2Real gap refers to the differences between simulated training environments and messy real-world conditions. Thin-object tracking is a known challenge in computer vision because narrow features like sword blades are difficult to detect, especially with motion blur.

<details><summary>References</summary>
<ul>
<li><a href="https://saipien.org/meta-partnr-embodied-ai-benchmark-teaching-robots-to-partner-with-humans-in-home-and-business/">Meta PARTNR: Embodied AI Benchmark Teaching Robots To Partner...</a></li>
<li><a href="https://www.ultralytics.com/glossary/object-tracking">What is Object Tracking? Computer Vision Guide | Ultralytics</a></li>

</ul>
</details>

**Tags**: `#computer vision`, `#dataset`, `#embodied AI`, `#motion tracking`, `#HEMA`

---

<a id="item-18"></a>
## [uv 0.11.26 released with performance boosts](https://github.com/astral-sh/uv/releases/tag/0.11.26) ⭐️ 6.0/10

uv 0.11.26 was released on June 30, 2026, featuring performance improvements to the PubGrub dependency resolver and a bug fix for build cache warnings. These optimizations make uv faster for resolving complex dependency trees, directly benefiting Python developers who use uv as a package manager. The focus on resolver performance is critical for large projects with many dependencies. The update adapts uv to IDs-only PubGrub dependencies, reduces allocations in ForkMap::contains, reuses resolver work across iterations, and speeds up candidate selection for disjoint ranges. The only bug fix warns when the build cache is inside the source directory.

github · github-actions[bot] · Jun 30, 14:53

**Background**: uv is a fast Python package manager written in Rust. PubGrub is a conflict-driven dependency resolution algorithm that uses clause learning to efficiently solve version constraints. ForkMap is a data structure used internally by uv; disjoint ranges are version ranges that do not overlap, which can be resolved more quickly.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vector-of-bool/pubgrub">GitHub - vector-of-bool/pubgrub: Pubgrub dependency resolution algorithm for C++</a></li>
<li><a href="https://docs.astral.sh/uv/concepts/resolution/">Resolution | uv</a></li>
<li><a href="https://nesbitt.io/2026/02/06/dependency-resolution-methods.html">Dependency Resolution Methods | Andrew Nesbitt</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#uv`, `#release-notes`

---

<a id="item-19"></a>
## [Google Copybara: Moving Code Between Repositories](https://github.com/google/copybara) ⭐️ 6.0/10

Google's open-source tool Copybara automates transforming and moving code between repositories while preserving history. It enables efficient syncing between monorepos and external repos, simplifying workflows for teams that need to share code across projects without the overhead of separate libraries. Copybara uses a Skylark DSL for defining workflows and supports integrations with Git and GitHub. It originated from Google's internal monorepo needs.

hackernews · reconnecting · Jun 30, 23:45 · [Discussion](https://news.ycombinator.com/item?id=48740698)

**Background**: In version control, a monorepo is a single repository containing multiple projects. Google, Meta, and others use large monorepos. Copybara helps manage code that needs to exist in both internal and external repositories.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/google/copybara">GitHub - google/copybara: Copybara: A tool for transforming and moving code between repositories. · GitHub</a></li>
<li><a href="https://stackfoss.medium.com/copybara-a-tool-for-transforming-and-moving-code-between-repositories-315a75502f6d">Copybara: A Tool for Transforming and Moving Code between Repositories | by StackFoss | Medium</a></li>
<li><a href="https://www.webpronews.com/googles-copybara-open-source-tool-for-code-migration-and-syncing/">Google’s Copybara: Open-Source Tool for Code Migration and Syncing</a></li>

</ul>
</details>

**Discussion**: Users praise Copybara for simplifying code export workflows, with one noting it's 'something you should have set up yesterday.' Some mention alternatives like Josh for Rust or Jujutsu workflows, but overall sentiment is positive for specific use cases.

**Tags**: `#code migration`, `#monorepo`, `#version control`, `#Google`

---

<a id="item-20"></a>
## [Brain2Qwerty: Non-Invasive Brain-to-Text AI](https://ai.meta.com/blog/brain2qwerty-brain-ai-human-communication/?_fb_noscript=1) ⭐️ 6.0/10

Meta AI researchers introduced Brain2Qwerty, a non-invasive system that uses AI to decode brain activity into text with a small but statistically significant improvement over previous methods. This work advances non-invasive brain-computer interfaces, potentially enabling communication for paralyzed individuals without the risks of surgery, while also shedding light on how the brain processes language. The system relies on magnetoencephalography (MEG) and electroencephalography (EEG) recordings, and the researchers released the code and dataset to foster reproducibility and further research.

hackernews · alok-g · Jun 30, 21:29 · [Discussion](https://news.ycombinator.com/item?id=48739466)

**Background**: Brain-computer interfaces (BCIs) can be invasive (requiring surgery) or non-invasive (using external sensors like EEG). Non-invasive BCIs are safer but typically yield lower signal quality. Brain2Qwerty combines advanced AI with non-invasive recording to improve decoding accuracy, though it still lags behind invasive methods.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/brain2qwerty-brain-ai-human-communication/">From Brain Waves to Words: Brain2Qwerty Offers a New Path to Communication Without Surgery</a></li>
<li><a href="https://www.deeplearning.ai/the-batch/brain2qwerty-a-system-that-decodes-thoughts-using-brain-waves-without-surgery">Brain2Qwerty, A System That Decodes Thoughts Using Brain Waves Without Surgery</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the improvement is incremental rather than revolutionary, but praised the release of code and dataset. Ethical concerns about neural privacy were raised, and some discussed the potential of combining EEG with LLMs for better decoding.

**Tags**: `#brain-computer interface`, `#EEG`, `#speech decoding`, `#AI`, `#Meta`

---

<a id="item-21"></a>
## [MARS2 Workshop on Multimodal Reasoning at ECCV 2026](https://www.reddit.com/r/MachineLearning/comments/1uka1r6/anyone_looking_into_the_new_mars2/) ⭐️ 6.0/10

The MARS2 Workshop and Competition on multimodal reasoning and test-time reasoning for video temporal grounding has been announced for ECCV 2026, with speakers from MIT, Cambridge, Oxford, CMU, and NTU, and organizers including Tec-Do and MiniMax. This workshop could establish a benchmark for evaluating multimodal reasoning in real-world scenarios like advertising understanding, potentially advancing video understanding and test-time compute scaling. The competition emphasizes 'slow thinking' (test-time reasoning) applied to video temporal grounding, and features organizers Tec-Do and MiniMax, with speakers from top universities.

reddit · r/MachineLearning · /u/Glass-Childhood-4971 · Jul 1, 03:15

**Background**: Video temporal grounding is the task of locating the start and end timestamps in an untrimmed video that correspond to a natural language query. Test-time reasoning (or test-time compute) enables models to perform additional inference steps to improve reasoning accuracy. The MARS2 Workshop combines these concepts to evaluate models that can reason step-by-step about video content in realistic applications.

<details><summary>References</summary>
<ul>
<li><a href="https://minghangz.github.io/uploads/TFVTG/TFVTG_paper.pdf">Training-free Video Temporal Grounding using</a></li>
<li><a href="https://huggingface.co/blog/Kseniase/testtimecompute">What is test-time compute and how to scale it?</a></li>

</ul>
</details>

**Tags**: `#multimodal reasoning`, `#ECCV`, `#video temporal grounding`, `#competition`, `#workshop`

---

<a id="item-22"></a>
## [Improving 5-Class Diabetic Retinopathy Model on APTOS 2019](https://www.reddit.com/r/MachineLearning/comments/1ujztdd/how_to_improve_a_5class_diabetic_retinopathy/) ⭐️ 6.0/10

A final-year student reports persistent misclassification in a 5-class diabetic retinopathy classifier trained on the APTOS 2019 dataset, seeking advice on improving model consistency. Medical AI models for diabetic retinopathy are critical for early diagnosis, but class confusion can undermine clinical trust; addressing this issue may improve real-world deployment. The model confuses Moderate with Severe or Proliferative, and Severe is often misclassified; high confidence even when wrong suggests overconfidence. The student has tried preprocessing, TTA, and different architectures (ResNet50, ResNet152) but still faces issues.

reddit · r/MachineLearning · /u/Delicious_Corner_754 · Jun 30, 19:58

**Background**: Diabetic retinopathy (DR) is a diabetes complication affecting eyes. The APTOS 2019 dataset contains 3662 fundus images with 5 severity classes: No DR, Mild, Moderate, Severe, Proliferative DR. Transfer learning with pretrained models like ResNet is common, but domain shift and class imbalance can degrade performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kaggle.com/datasets/mariaherrerot/aptos2019">APTOS-2019 dataset | Kaggle</a></li>
<li><a href="https://academictorrents.com/details/d8653db45e7f111dc2c1b595bdac7ccf695efcfd">APTOS 2019 diabetic retinopathy dataset - Academic Torrents</a></li>
<li><a href="https://www.vizuaranewsletter.com/p/resnet-the-architecture-that-changed">ResNet: The architecture that changed ML forever</a></li>

</ul>
</details>

**Tags**: `#diabetic retinopathy`, `#transfer learning`, `#classification`, `#APTOS 2019`, `#medical AI`

---

<a id="item-23"></a>
## [Why NCE over MLE for Instance Representation Learning?](https://www.reddit.com/r/MachineLearning/comments/1uj8nse/loss_functions_in_instance_representation/) ⭐️ 6.0/10

A Reddit user questions why Noise Contrastive Estimation (NCE) is used instead of Maximum Likelihood Estimation (MLE) for instance representation learning, specifically regarding the non-parametric softmax in Wu et al.'s paper. This question addresses a core design choice in self-supervised learning, clarifying the computational and statistical trade-offs between NCE and MLE, which is essential for understanding popular objectives like InfoNCE. The user is confused about why NCE is computationally advantageous when the partition function approximation seems similar to direct approximation in MLE, and about the biased estimation concern raised by Claude.

reddit · r/MachineLearning · /u/No_Balance_9777 · Jun 29, 23:34

**Background**: In instance representation learning, maximizing the likelihood under a non-parametric softmax requires computing a normalization term over all instances, which is computationally prohibitive for large datasets. NCE avoids this by transforming the problem into a binary classification task that discriminates between real data and noise samples. As the number of noise samples increases, the NCE gradient converges to the gradient of the true log-likelihood, making it a practical approximation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/noise-contrastive-estimation-loss">What Is Noise Contrastive Estimation Loss ?</a></li>
<li><a href="https://arxiv.org/pdf/1805.01978">Unsupervised Feature Learning via Non - Parametric Instance...</a></li>
<li><a href="https://wandb.ai/self-supervised-learning/index/reports/What-Is-Noise-Contrastive-Estimation-Loss-A-Tutorial-With-Code--Vmlldzo2NzY2OTY2">What Is Noise Contrastive Estimation Loss ? A Tutorial With Code</a></li>

</ul>
</details>

**Tags**: `#representation learning`, `#noise contrastive estimation`, `#loss functions`, `#machine learning`

---