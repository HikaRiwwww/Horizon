---
layout: default
title: "Horizon Summary: 2026-06-24 (EN)"
date: 2026-06-24
lang: en
---

> From 34 items, 18 important content pieces were selected

---

1. [FUTO Swipe: New Model Boosts Accuracy on Privacy-Focused Keyboard](#item-1) ⭐️ 8.0/10
2. [Swift Package Index joins Apple](#item-2) ⭐️ 8.0/10
3. [The Coming Loop: AI Coding Risks Losing Human Taste](#item-3) ⭐️ 8.0/10
4. [Baidu Unlimited OCR: One-Shot Long Document Parsing](#item-4) ⭐️ 8.0/10
5. [Datasette 1.0a35: New Create/Alter Table Interfaces and JSON APIs](#item-5) ⭐️ 8.0/10
6. [LLMs Prioritize Style Over Role Tags, Enabling Jailbreaks](#item-6) ⭐️ 8.0/10
7. [Porting Moebius 0.2B Inpainting Model to Browser with WebGPU](#item-7) ⭐️ 8.0/10
8. [DeepSWE: New Open-Source Benchmark for Frontier Coding Models](#item-8) ⭐️ 8.0/10
9. [TikZ Editor – WYSIWYG for LaTeX Figures](#item-9) ⭐️ 7.0/10
10. [Vitamin D: Not Worthless, But Not Miraculous](#item-10) ⭐️ 7.0/10
11. [Are ML teams testing model security risks in production?](#item-11) ⭐️ 7.0/10
12. [Non-deterministic Benchmark Obfuscates Known Vulnerabilities to Test LLMs](#item-12) ⭐️ 7.0/10
13. [uv 0.11.24 adds CPython 3.15.0b3 support and relocatable environments](#item-13) ⭐️ 6.0/10
14. [Tribute to the inventor of red and green spell-check squiggles](#item-14) ⭐️ 6.0/10
15. [Extreme Heat Conference Canceled Due to Heat Warning](#item-15) ⭐️ 6.0/10
16. [OPFS + Pyodide Test Harness for Browser SQLite Editing](#item-16) ⭐️ 6.0/10
17. [Hugging Face Revives Papers with Code with New Features](#item-17) ⭐️ 6.0/10
18. [Niche request for syntax-robust NLI for diffusion LLMs](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [FUTO Swipe: New Model Boosts Accuracy on Privacy-Focused Keyboard](https://swipe.futo.tech/) ⭐️ 8.0/10

FUTO Keyboard now includes a new swipe typing model called FUTO Swipe that significantly improves accuracy, aiming to rival Gboard while keeping all processing offline. This matters because it brings high-quality swipe typing to privacy-conscious users who previously had to choose between accuracy and data privacy. It could shift the mobile input landscape by proving that offline, open-source keyboards can match proprietary ones. The swipe model is available now in the FUTO Keyboard app and was trained using user swipe data collected through an opt-in training program. Some users report it feels as good as Gboard, though it still lacks context-aware suggestions and occasionally capitalizes words incorrectly.

hackernews · futohq · Jun 23, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48648619)

**Background**: FUTO Keyboard is an open-source, fully offline Android keyboard that prioritizes user privacy by not sending any data to the cloud. Swipe typing (or gesture typing) allows users to input words by sliding their finger over letters, which is faster than tapping. Historically, open-source keyboards have struggled with swipe accuracy compared to proprietary ones like Gboard, which rely on cloud-based models.

<details><summary>References</summary>
<ul>
<li><a href="https://swipe.futo.tech/">FUTO Swipe</a></li>
<li><a href="https://swipe.futo.org/">FUTO Keyboard Swipe Training</a></li>

</ul>
</details>

**Discussion**: Users are generally positive, with many stating the new swipe model is a significant improvement and close to Gboard. Some note minor issues like random capitalization and lack of context awareness, but overall satisfaction is high. There is also a mention of licensing concerns: the swipe library is GPLv3 but the main app uses a different license.

**Tags**: `#keyboard`, `#swipe typing`, `#privacy`, `#open-source`, `#mobile input`

---

<a id="item-2"></a>
## [Swift Package Index joins Apple](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 8.0/10

Apple has acquired the Swift Package Index (SPI), a community-run search engine for Swift packages that support the Swift Package Manager. This acquisition could centralize Swift package discovery under Apple’s control, potentially affecting the openness of the ecosystem and raising concerns about future governance and restrictions. SPI currently indexes metadata from over 11,000 packages and is itself an open-source project. The acquisition explicitly mentions developer identity as a future direction, which has sparked debate among developers.

hackernews · JDevlieghere · Jun 23, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48648779)

**Background**: The Swift Package Index is a community-maintained tool that helps developers discover Swift packages compatible with the Swift Package Manager. It has been a key resource in the Swift ecosystem. Apple's move to acquire SPI raises questions about whether it will remain open and community-driven or become more restrictive under Apple's governance.

<details><summary>References</summary>
<ul>
<li><a href="https://swiftpackageindex.com/">Swift Package Index</a></li>
<li><a href="https://www.swift.org/packages/">Packages | Swift.org</a></li>
<li><a href="https://github.com/SwiftPackageIndex">Swift Package Index · GitHub</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some are happy for the SPI team, while others worry about Apple's track record with open source and developer services, especially given the mention of developer identity as a future direction. Another comment notes the potential for a competitor to emerge due to SPI's limitation to GitHub repos.

**Tags**: `#Swift`, `#Apple`, `#Package Management`, `#Open Source`

---

<a id="item-3"></a>
## [The Coming Loop: AI Coding Risks Losing Human Taste](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

Armin Ronacher's article 'The Coming Loop' argues that over-reliance on LLMs for code generation and summarization creates a feedback loop where humans gradually lose understanding and aesthetic judgment of code. This critique highlights a significant risk in current AI-assisted coding trends: as developers increasingly accept machine-generated code without full comprehension, codebases may become unmaintainable by humans alone, potentially degrading software quality and developer skill over time. The article emphasizes that the loop occurs when people merge code they cannot explain, rely on machines to summarize contexts, and lose the ability to create precise issue reports without AI augmentation. It also notes that aesthetics and taste are crucial aspects of coding that LLMs cannot replicate.

hackernews · ingve · Jun 23, 11:06 · [Discussion](https://news.ycombinator.com/item?id=48643180)

**Background**: LLMs (Large Language Models) like GPT-4 are widely used for generating code snippets, summarizing discussions, and automating programming tasks. The 'loop' refers to a dependency cycle where humans offload cognitive work to AI, thereby weakening their own skills and judgment. This article reflects growing concerns in the software community about the long-term impact of AI on developer expertise and code quality.

**Discussion**: Community comments largely agree with the critique, with users like mccoyb noting that loops require upfront clarity, and stillpointlab emphasizing the bottleneck of writing good specifications. Some commenters point out that LLMs excel at goal-driven tasks but fail at aesthetics, reinforcing the article's core argument.

**Tags**: `#AI`, `#software engineering`, `#code generation`, `#LLMs`, `#human-AI interaction`

---

<a id="item-4"></a>
## [Baidu Unlimited OCR: One-Shot Long Document Parsing](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

Baidu released Unlimited OCR, an open-source model that can parse entire multi-page documents in a single forward pass using a novel KV cache optimization to avoid memory overload. This addresses a major bottleneck in document AI: processing long PDFs without chunking, enabling efficient and accurate OCR for large documents, which benefits industries like finance, legal, and digitization. The model employs a sliding-window attention with always attending to the image prefix, and the KV cache optimization prevents linear memory growth. Quality degrades slightly with more pages, but the approach is single-pass.

hackernews · ingve · Jun 23, 11:35 · [Discussion](https://news.ycombinator.com/item?id=48643426)

**Background**: Vision-language models (VLMs) for OCR typically store a growing key-value cache as they process tokens, leading to VRAM exhaustion on long documents. Traditional solutions require chunking pages and stitching outputs, which can be error-prone. Unlimited OCR's KV cache hack allows for constant memory usage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.explainx.ai/blog/baidu-unlimited-ocr-one-shot-long-horizon-parsing-2026">Baidu Unlimited-OCR: One-Shot Long-Horizon Document Parsing ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48643426">Unlimited OCR: One-Shot Long-Horizon Parsing | Hacker News</a></li>
<li><a href="https://news.linxi.com.au/news/baidu-releases-open-source-unlimited-ocr-for-long-horizon-document-parsing">Baidu Unlimited OCR Open Source Release: One-Shot Long ...</a></li>

</ul>
</details>

**Discussion**: Commenters appreciate the clever KV cache hack and note that similar multi-page VLM OCR works like MinerU-Popo treat post-processing as a separate step. One user points out the name references 'Unlimited Blade Works' from Fate/stay night, and another highlights the team's acknowledgment of Deepseek-OCR and PaddleOCR.

**Tags**: `#OCR`, `#KV Cache`, `#Long Document Processing`, `#AI Efficiency`, `#VLM`

---

<a id="item-5"></a>
## [Datasette 1.0a35: New Create/Alter Table Interfaces and JSON APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a35 introduces a new create table interface and alter table interface, both backed by JSON APIs, allowing users to define columns, constraints, and foreign keys programmatically. These features mark a significant step towards the Datasette 1.0 release, enabling users to manage database schemas directly through the web UI or API without external tools. The create table API supports defining columns, primary keys, custom types, NOT NULL constraints, literal and expression defaults, and single-column foreign keys. The alter table API supports adding, renaming, reordering, and dropping columns, as well as changing types, defaults, constraints, primary keys, foreign keys, and renaming the table.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing structured data. It automatically creates a JSON API for any SQLite database. This release is part of the alpha series leading to Datasette 1.0, which aims to stabilize the core features.

**Tags**: `#datasette`, `#data exploration`, `#SQLite`, `#JSON API`, `#open source`

---

<a id="item-6"></a>
## [LLMs Prioritize Style Over Role Tags, Enabling Jailbreaks](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Research shows that LLMs cannot reliably distinguish system prompts from user input, as they prioritize writing style over literal role tags like <system> and <user>. A technique called 'destyling' — rewriting text to differ slightly in style — reduced attack success from 61% to 10%. This finding challenges current defenses against prompt injection, which rely on role tags and content filtering. It suggests that without genuine role perception, LLM security will remain a 'whack-a-mole game'. The researchers tested models like gpt-oss-20b and found that appending text matching the style of internal thinking blocks could override training. Role confusion is described as a continuous boundary, making subtle injections possible at scale.

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection is a security vulnerability where an attacker manipulates the input to an AI model to alter its behavior. Role tags like <system> and <user> are commonly used to separate instructions from user input in LLM applications. This research reveals that models rely more on stylistic cues than on these tags, undermining the fundamental trust in role-based separation.

<details><summary>References</summary>
<ul>
<li><a href="https://prompt-engineering-guide.vercel.app/prompts/adversarial-prompting/prompt-injection">Prompt Injection in LLMs | Prompt Engineering Guide</a></li>
<li><a href="https://letsdatascience.com/news/researchers-demonstrate-prompt-injection-as-role-confusion-40c29edb">Researchers Demonstrate Prompt Injection as Role Confusion | Let's Data Science</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_safety">AI safety - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#AI safety`, `#LLM`, `#role confusion`, `#jailbreak`

---

<a id="item-7"></a>
## [Porting Moebius 0.2B Inpainting Model to Browser with WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison ported the Moebius 0.2B image inpainting model from PyTorch/CUDA to run in the browser using WebGPU, achieving interactive performance. He used Claude Code as an agentic coding tool to accelerate the porting process. This demonstrates that lightweight state-of-the-art models can run efficiently at the edge (browser) without server-side compute, enabling privacy-preserving, low-latency AI tools. It also showcases the potential of WebGPU for real-time machine learning inference in web applications. The port used ONNX Runtime Web with the WebGPU backend, as suggested by Claude during initial research. The demo is available at simonw.github.io/moebius-web/, allowing users to upload images, mark regions to remove, and run inpainting directly in the browser.

rss · Simon Willison · Jun 22, 23:43

**Background**: Image inpainting is a computer vision task where missing or removed regions of an image are filled plausibly. Moebius is a 0.2B parameter model that achieves performance comparable to 10B+ models, making it suitable for lightweight deployment. WebGPU is a web standard providing low-level GPU access in browsers, superseding WebGL and enabling general-purpose GPU compute for tasks like ML inference.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebGPU">WebGPU</a></li>
<li><a href="https://huggingface.co/papers/2606.19195">Paper page - Moebius : 0 . 2 B Lightweight Image Inpainting Framework...</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**Discussion**: On Hacker News, commenters expressed excitement about running advanced AI models in the browser and praised the use of Claude Code for rapid prototyping. Some discussed the implications of WebGPU for democratizing AI and reducing reliance on cloud infrastructure.

**Tags**: `#machine learning`, `#webgpu`, `#image inpainting`, `#browser AI`, `#open source`

---

<a id="item-8"></a>
## [DeepSWE: New Open-Source Benchmark for Frontier Coding Models](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark that evaluates frontier coding models using contamination-free tasks written from scratch, spanning 91 repositories across 5 languages, with prompts half the length of SWE-bench Pro but requiring 5.5x more code. This benchmark addresses critical issues in current AI coding evaluations like data contamination and task simplicity, providing a more realistic measure of how well frontier coding agents perform in real-world software engineering. DeepSWE's verifiers are hand-written to test software behavior rather than implementation details, and all tasks are contamination-free as they are created from scratch rather than adapted from existing commits.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Existing benchmarks like SWE-bench evaluate AI models on real GitHub issues, but they may suffer from data contamination since models could have seen solutions during pretraining. Contamination-free benchmarks ensure test instances are strictly excluded from training data, providing a faithful measure of generalization. DeepSWE is a new effort in this direction, specifically for software engineering tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/contamination-free-benchmarking">Contamination-Free Benchmarking - emergentmind.com</a></li>
<li><a href="https://epoch.ai/benchmarks/swe-bench-verified">SWE-bench Verified | Epoch AI</a></li>
<li><a href="https://www.swebench.com/">SWE-bench Leaderboards</a></li>

</ul>
</details>

**Tags**: `#benchmark`, `#AI coding`, `#machine learning`, `#open source`

---

<a id="item-9"></a>
## [TikZ Editor – WYSIWYG for LaTeX Figures](https://tikz.dev/editor/) ⭐️ 7.0/10

A new open-source WYSIWYG editor for TikZ figures allows users to edit LaTeX source code visually by dragging and resizing elements, with source and rendered view staying in sync. This tool addresses a common pain point for academics who manually code TikZ figures, potentially saving significant time and reducing trial-and-error. Its open-source nature and AI-assisted development also demonstrate how coding agents can build complex software that was previously too tedious to implement. The editor parses TikZ code and tracks exact source locations for each object, enabling coordinate edits without changing code structure. It was built almost entirely using Codex, consuming about 700M tokens (approx. $15k API cost but only $500 in ChatGPT subscriptions). It also includes converters from SVG/pptx/ipe to TikZ.

hackernews · DominikPeters · Jun 23, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48645437)

**Background**: TikZ is a LaTeX package for creating vector graphics programmatically, widely used in academic papers for diagrams. Traditionally, users write TikZ commands like \draw (0,0) -- (1,2); and recompile to see results, which can be tedious. WYSIWYG editors exist for other graphics formats (e.g., SVG), but this tool uniquely combines source code editing with visual manipulation for TikZ.

<details><summary>References</summary>
<ul>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://tikzmaker.com/">TikzMaker</a></li>

</ul>
</details>

**Discussion**: Community feedback is generally positive but includes criticism about the generated TikZ code using absolute coordinates unnecessarily. Some users noted that AI tools can already generate TikZ code effectively. The developer shared that the project used about 700M tokens via Codex, costing around $500 in subscription fees.

**Tags**: `#LaTeX`, `#TikZ`, `#editor`, `#academic tools`, `#open-source`

---

<a id="item-10"></a>
## [Vitamin D: Not Worthless, But Not Miraculous](https://dynomight.net/vitamin-d/) ⭐️ 7.0/10

A nuanced analysis argues that while vitamin D benefits are often overstated for the general population, it remains important for those severely deficient. This balanced perspective counters the hype surrounding vitamin D, helping the public and health professionals make more evidence-based decisions about supplementation. The analysis highlights that many studies use flawed methodologies, such as inadequate control for seasonal and latitudinal variations, and that effects are most pronounced in those with baseline deficiency.

hackernews · surprisetalk · Jun 23, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48647486)

**Background**: Vitamin D is a fat-soluble nutrient essential for calcium absorption and bone health. While it is also implicated in immune function and other processes, large randomized trials have largely failed to show benefits for disease prevention in the general population, leading to debate about its actual value.

**Discussion**: Commenters generally praised the balanced analysis, with several noting that the strongest evidence supports vitamin D supplementation only for those with severe deficiency. Some discussed the need for co-factors like vitamin K2 and criticized common research pitfalls such as not measuring blood levels after supplementation.

**Tags**: `#vitamin D`, `#health research`, `#science communication`, `#critical analysis`

---

<a id="item-11"></a>
## [Are ML teams testing model security risks in production?](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

A Reddit post by user Xorphian highlights that many ML teams skip adversarial testing (e.g., model extraction, poisoning) before deploying models, contrasting with standard software security reviews. The discussion questions whether and how practitioners are addressing these risks in production. Model security risks like extraction and poisoning can lead to intellectual property theft, compromised model integrity, and unsafe AI behavior, yet they remain under-tested. This discussion underscores a critical gap in MLOps practices that could have serious consequences as ML adoption grows. Model extraction attacks involve stealing a model's functionality by querying its API, while poisoning attacks manipulate training data or model parameters to cause undesirable behavior. The post suggests that security review for models lags behind traditional software, and many teams lack adversarial testing before production deployment.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Adversarial machine learning encompasses attacks that exploit vulnerabilities in ML systems, including model extraction, poisoning, and evasion. Model extraction attacks allow an adversary to create a replica model by systematically querying the target's prediction API, while data poisoning involves corrupting training data to influence model behavior. These threats are well-documented but often neglected in production environments, unlike security testing for conventional software.

<details><summary>References</summary>
<ul>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>
<li><a href="https://owasp.org/www-project-machine-learning-security-top-10/docs/ML10_2023-Model_Poisoning">ML10:2023 Model Poisoning - OWASP Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ML Security`, `#Adversarial ML`, `#Model Extraction`, `#Model Poisoning`, `#Production ML`

---

<a id="item-12"></a>
## [Non-deterministic Benchmark Obfuscates Known Vulnerabilities to Test LLMs](https://www.reddit.com/r/MachineLearning/comments/1ud0rft/nondeterministic_vulnerability_detection/) ⭐️ 7.0/10

A new benchmark system obfuscates Juliet test cases and injects misleading comments to evaluate LLM robustness in vulnerability detection, addressing the issue of LLMs recognizing known CWE patterns. This approach provides a more realistic evaluation of LLMs' true vulnerability detection capabilities by removing the advantage of pattern familiarity, which could lead to more reliable AI security tools. The benchmark uses Juliet C/C++ test cases from NIST, covering over 100 CWEs, and applies obfuscation along with LLM-generated comments (accurate, misleading, or neutral) to test robustness.

reddit · r/MachineLearning · /u/Psychological_Meat_6 · Jun 22, 23:34

**Background**: Juliet test cases are a standard set of synthetic vulnerability examples developed by NIST, widely used for evaluating static analysis tools. LLMs like GPT-4 have been tested on these cases but may benefit from pattern recognition rather than true understanding. This benchmark aims to mitigate that by hiding the known patterns.

<details><summary>References</summary>
<ul>
<li><a href="https://samate.nist.gov/SARD/test-suites/112">Juliet C/C++ 1.3 - NIST Software Assurance Reference Dataset</a></li>
<li><a href="https://github.com/arichardson/juliet-test-suite-c">GitHub - arichardson/juliet-test-suite-c · GitHub</a></li>
<li><a href="https://github.com/huhusmang/Awesome-LLMs-for-Vulnerability-Detection">GitHub - huhusmang/Awesome-LLMs-for- Vulnerability - Detection : The...</a></li>

</ul>
</details>

**Tags**: `#vulnerability detection`, `#LLM benchmarking`, `#cybersecurity`, `#adversarial testing`, `#AI security`

---

<a id="item-13"></a>
## [uv 0.11.24 adds CPython 3.15.0b3 support and relocatable environments](https://github.com/astral-sh/uv/releases/tag/0.11.24) ⭐️ 6.0/10

uv 0.11.24 has been released on 2026-06-23, adding support for CPython 3.15.0b3 and introducing a preview feature for making project environments relocatable. It also includes performance enhancements such as a compact index for lazy version maps and several bug fixes. The relocatable project environments feature improves portability of Python environments, simplifying workflows for developers who need to move or share environments. The addition of CPython 3.15.0b3 support ensures uv stays compatible with the latest Python pre-release, benefiting early adopters. The relocatable feature is currently under preview, meaning it may not yet be stable for production use. Performance is improved by using a compact index for lazy version maps, which reduces memory overhead during dependency resolution.

github · github-actions[bot] · Jun 23, 21:16

**Background**: uv is an extremely fast Python package and project manager written in Rust, designed as a drop-in replacement for pip. A relocatable environment allows a virtual environment to be moved to a different location on disk without breaking paths, which is useful for deploying applications or sharing environments across systems. The lazy version maps optimization defers the loading of package version metadata until needed, improving performance in large dependency trees.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/pip/environments/">Using environments | uv</a></li>
<li><a href="https://docs.astral.sh/uv/">uv is an extremely fast Python package and project manager, written...</a></li>

</ul>
</details>

**Tags**: `#uv`, `#python`, `#package manager`, `#release`, `#performance`

---

<a id="item-14"></a>
## [Tribute to the inventor of red and green spell-check squiggles](https://devblogs.microsoft.com/oldnewthing/20260622-00/?p=112451) ⭐️ 6.0/10

Raymond Chen's article on The Old New Thing pays tribute to Tony Krueger, the developer who introduced red and green squiggly underlines for spell checking in word processors. This feature became a ubiquitous UI element in word processors, significantly improving user experience and becoming a standard visual cue for error indication across nearly all text editing applications. The article and community comments highlight a circular reference where the Wikipedia page cites Chen's article as evidence for Krueger's role, creating an amusing anecdote about sourcing.

hackernews · saikatsg · Jun 23, 18:10 · [Discussion](https://news.ycombinator.com/item?id=48648959)

**Background**: Spell check squiggly underlines are visual indicators used in word processors to alert users to potential errors: red for spelling mistakes and green for grammar issues. This feature was pioneered by Tony Krueger, who implemented it in early versions of word processing software, and it has since become a standard UI element adopted by nearly all text editing applications.

<details><summary>References</summary>
<ul>
<li><a href="https://creativepro.com/why-red-squiggly-underlines-when-words-are-not-spelled-wrong/">Why Red Squiggly Underlines When Words are Not Spelled Wrong</a></li>
<li><a href="https://squiggly.sourceforge.net/">Squiggly Spell Check.</a></li>

</ul>
</details>

**Discussion**: The community comments are lighthearted, with one user noting the circular Wikipedia reference, another appreciating the innovation, and one suggesting a feature for yellow squiggles under logic errors. There is also nostalgia for the variety of text formatting that has disappeared.

**Tags**: `#software history`, `#word processing`, `#spell check`, `#UI design`

---

<a id="item-15"></a>
## [Extreme Heat Conference Canceled Due to Heat Warning](https://www.lse.ac.uk/granthaminstitute/events/extreme-heat-improving-governance-and-strengthening-action-around-the-world/) ⭐️ 6.0/10

A conference titled 'Extreme Heat: Improving Governance and Strengthening Action Around the World' was canceled because an extreme heat warning was issued for the event date. The ironic cancellation underscores gaps in climate resilience planning and sparks public debate on infrastructure and adaptation to rising temperatures. The event, hosted by the Grantham Research Institute at LSE in collaboration with the Zurich Climate Resilience Alliance, was scheduled as a hybrid conference and featured a 'fire side chat' as a closing session.

hackernews · rendx · Jun 23, 23:26 · [Discussion](https://news.ycombinator.com/item?id=48653060)

**Background**: The conference aimed to address governance and action on extreme heat, but its cancellation due to the very hazard it focused on highlights the challenges of preparing for climate extremes. The irony was noted by commentators, who pointed out that the event's own resilience was low.

**Discussion**: Comments expressed irony and criticism: some noted Europe's resistance to air conditioning as a public health issue, while an Australian found 37-40°C mundane but acknowledged infrastructure differences. Others joked about the 'fire side chat' and compared the situation to a dermatology conference in Hawaii.

**Tags**: `#climate change`, `#irony`, `#conferences`, `#public policy`, `#heat`

---

<a id="item-16"></a>
## [OPFS + Pyodide Test Harness for Browser SQLite Editing](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison built a test harness that combines the Origin Private File System (OPFS) with Pyodide to explore persistent SQLite file editing in Datasette Lite. The harness allows testing OPFS support across different browsers for storing and editing SQLite files entirely client-side. This could enable Datasette Lite to edit persistent SQLite databases stored on the user's device without a server, greatly expanding its utility for offline and privacy-sensitive applications. It also demonstrates the growing potential of running full Python web applications in the browser via WebAssembly. The test harness uses the OPFS, which is part of the File System API and provides a private storage area per origin, not visible to the user. Pyodide runs CPython in the browser via WebAssembly, enabling Python packages like SQLite to execute client-side.

rss · Simon Willison · Jun 23, 18:58

**Background**: The Origin Private File System (OPFS) is a browser storage endpoint that gives web applications a private, high-performance file system for each origin, not visible to users. Pyodide is a Python distribution for the browser and Node.js based on WebAssembly, allowing Python code to run client-side with access to Web APIs. Datasette Lite is a version of the Datasette data exploration tool that runs entirely in the browser using Pyodide and WebAssembly.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN - MDN Web Docs</a></li>
<li><a href="https://web.dev/articles/origin-private-file-system">The origin private file system | Articles | web.dev</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution ... Home - Pyodide Pyodide — Version 314.1.0.dev0 Pyodide - GitHub pyodide | Pyodide is a Python distribution for the browser ... About Us - pyodide</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#OPFS`, `#Datasette Lite`, `#WebAssembly`, `#Browser Storage`

---

<a id="item-17"></a>
## [Hugging Face Revives Papers with Code with New Features](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 6.0/10

Hugging Face has added SOTA badges, a new trending score that incorporates Hugging Face artifact popularity, and support for external evaluations to Papers with Code. These updates aim to revive the platform and improve research discovery. These features make it easier for researchers to identify state-of-the-art papers and track trending research, fostering collaboration and accelerating innovation. The inclusion of external evals provides a more comprehensive view of a paper's impact. The trending score now combines GitHub star velocity with the popularity of linked Hugging Face models, datasets, and Spaces. External evals allow papers to display third-party benchmark results, such as PostTrainBench scores for GLM-5.2.

reddit · r/MachineLearning · /u/NielsRogge · Jun 22, 14:29

**Background**: Papers with Code is a platform that links research papers to code and benchmarks, helping researchers track progress. Hugging Face acquired the platform in 2021 and is now revitalizing it with new features to enhance discoverability and community engagement.

<details><summary>References</summary>
<ul>
<li><a href="https://posttrainbench.com/">PostTrainBench</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#papers with code`, `#research tools`, `#sota`

---

<a id="item-18"></a>
## [Niche request for syntax-robust NLI for diffusion LLMs](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 6.0/10

A Reddit user seeks literature on Natural Language Inference (NLI) methods that are robust to syntactic errors, specifically for evaluating the semantic correctness of text generated by diffusion-based large language models (LLMs) like LLaDA. This addresses a gap in evaluation techniques for diffusion LLMs, which often produce less syntactically perfect text than autoregressive models. Robust NLI could enable better assessment of semantic accuracy despite syntactic noise, impacting the adoption and benchmarking of diffusion-based text generation. The user notes that diffusion LLMs (e.g., LLaDA) tend to have more syntactic issues compared to autoregressive LLMs, complicating standard NLI usage. They specifically ask for state-of-the-art syntax-robust NLI, such as MENLI and AMR4NLI mentioned in search results.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 22, 21:51

**Background**: Natural Language Inference (NLI) determines whether a hypothesis is entailed, contradicted, or neutral given a premise. In LLM evaluation, NLI is used to check if generated claims are semantically correct. Diffusion LLMs generate text by iterative denoising, often producing less fluent syntax. Syntax-robust NLI aims to maintain accuracy despite grammatical imperfections.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2208.07316v5">MENLI: Robust Evaluation Metrics from Natural Language Inference</a></li>
<li><a href="https://arxiv.org/pdf/2306.00936v1">AMR4NLI: Interpretable and robust NLI measures from semantic ...</a></li>
<li><a href="https://ml-gsai.github.io/LLaDA-demo/">LLaDA - Large Language Diffusion Models</a></li>

</ul>
</details>

**Tags**: `#NLI`, `#LLM`, `#syntactically robust`, `#diffusion models`, `#semantic evaluation`

---