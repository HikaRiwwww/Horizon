---
layout: default
title: "Horizon Summary: 2026-06-29 (EN)"
date: 2026-06-29
lang: en
---

> From 26 items, 19 important content pieces were selected

---

1. [Using Claude Code as an MRI Second Opinion](#item-1) ⭐️ 8.0/10
2. [Brown professor denounces AI cheating epidemic](#item-2) ⭐️ 8.0/10
3. [MathFormer: Small Model Masters Symbolic Math via Pattern Matching](#item-3) ⭐️ 8.0/10
4. [NagaTranslate builds translation and voice pipeline for Nagaland's low-resource creoles](#item-4) ⭐️ 8.0/10
5. [Do We Still Need to Study Algorithms with AI Writing Code?](#item-5) ⭐️ 8.0/10
6. [GLM 5.2 Outperforms Claude on Cybersecurity Benchmarks](#item-6) ⭐️ 7.0/10
7. [Memory Prices from 1960 to 2026 Charted](#item-7) ⭐️ 7.0/10
8. [Show HN: Zanagrams – A Minimal Word Puzzle Game](#item-8) ⭐️ 7.0/10
9. [KIDS Act Would Mandate Age Checks, Raising Privacy Concerns](#item-9) ⭐️ 7.0/10
10. [Jon Udell: Keep Humans in Control of AI Agents](#item-10) ⭐️ 7.0/10
11. [Minimal Interactive Transformer Visualization Lets You Edit Weights](#item-11) ⭐️ 7.0/10
12. [Picotron: LLM training framework for older GPUs without crashes](#item-12) ⭐️ 7.0/10
13. [Pybench: pytest-like CLI for statistical ML regression testing](#item-13) ⭐️ 7.0/10
14. [5k Menus from NYPL Buttolph Collection (1880-1920)](#item-14) ⭐️ 6.0/10
15. [LibrePods: Open-Source Project Unlocks AirPods Features on Non-Apple Devices](#item-15) ⭐️ 6.0/10
16. [Daisugi: Japanese Technique of Growing Trees on Trees](#item-16) ⭐️ 6.0/10
17. [Evaluating long-term memory in stateless LLM chatbots](#item-17) ⭐️ 6.0/10
18. [Steganography in ONNX Model Weights via Mantissa Bits](#item-18) ⭐️ 6.0/10
19. [ML Models for Searching MMA Fight Moments](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Using Claude Code as an MRI Second Opinion](https://antoine.fi/mri-analysis-using-claude-code-opus) ⭐️ 8.0/10

A user uploaded their MRI images and radiology report to Claude Code (powered by Claude Opus) to obtain an AI-generated second opinion on a shoulder diagnosis, marking a novel application of large language models in medical imaging analysis. This experiment underscores both the potential of generative AI to assist patients in interpreting medical results and the serious risks of relying on non-FDA-approved tools for clinical decisions, sparking debate on trust, accuracy, and the role of LLMs in healthcare. Claude Code is primarily an AI coding agent, not a medical device; the user likely accessed Claude Opus's vision capabilities through the terminal-based tool. The analysis was done without regulatory clearance for diagnostic use, and the user still consulted a human radiologist.

hackernews · engmarketer · Jun 28, 16:35 · [Discussion](https://news.ycombinator.com/item?id=48708941)

**Background**: Claude is a series of large language models developed by Anthropic, with Claude Opus being the most capable variant. Claude Code is a command-line tool that allows developers to interact with Claude for coding tasks. In radiology, AI second-opinion services exist but are typically specialized, FDA-cleared tools, not general-purpose LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://dbmi.hms.harvard.edu/news/ai-based-second-opinion-service-could-improve-clinical-decision-making-today">An AI-based second opinion service could improve clinical decision-making today - Harvard DBMI</a></li>

</ul>
</details>

**Discussion**: The discussion reveals deep unease about AI reliability: some users shared personal misdiagnosis experiences, while a radiologist pointed out the limitations of using static images without full 3D datasets. Others expressed a paradoxical comfort in questioning an AI compared to a busy doctor, but overall skepticism remained high.

**Tags**: `#AI`, `#healthcare`, `#radiology`, `#LLM`, `#medical imaging`

---

<a id="item-2"></a>
## [Brown professor denounces AI cheating epidemic](https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html) ⭐️ 8.0/10

A professor at Brown University has publicly denounced widespread AI-assisted cheating on a major exam, calling for urgent pedagogical changes to preserve academic integrity. This incident underscores the growing threat AI tools pose to traditional assessment methods and may accelerate the shift toward in-person, handwritten exams and adversarial course design. The professor's research background in game theory provides a unique perspective; commenters note that in a competitive environment, using LLMs becomes a game-theoretically optimal choice.

hackernews · geox · Jun 28, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48708991)

**Background**: Large language models like ChatGPT can generate convincing essays and solve complex problems, making traditional take-home exams vulnerable to cheating. Universities have struggled to detect AI-generated submissions, leading to debates on assessment reform. Some educators advocate for in-person, handwritten tests and oral interviews to verify student understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://openreview.net/forum?id=syThiTmWWm">Cheating Automatic LLM Benchmarks: Null Models Achieve High Win Rates | OpenReview</a></li>
<li><a href="https://education.umd.edu/research/centers/marc/selected-projects/ai-enhanced-assessment-methods/cheating-detection">Cheating Detection | UMD College of Education</a></li>

</ul>
</details>

**Discussion**: Commenters on the discussion largely agree that AI cheating is a systemic problem, with many advocating for in-person handwritten exams and adversarial course design. One professor questions the value of grading altogether, while another notes the game-theoretic incentives to cheat.

**Tags**: `#AI in Education`, `#Academic Integrity`, `#LLM Cheating`, `#Teaching Methods`, `#Hacker News Discussion`

---

<a id="item-3"></a>
## [MathFormer: Small Model Masters Symbolic Math via Pattern Matching](https://www.reddit.com/r/MachineLearning/comments/1uhatw8/mathformer_testing_whether_symbolic_math_is/) ⭐️ 8.0/10

Researchers released MathFormer, a 4M-parameter seq2seq model that achieves ~98.6% accuracy on symbolic math expansion tasks (e.g., expanding factorized expressions) without any explicit math knowledge, suggesting models rely on token pattern matching rather than reasoning. This result challenges the assumption that large language models perform genuine mathematical reasoning, indicating they may excel at large-scale structured pattern completion instead. It has implications for understanding and improving reasoning in neural networks, particularly regarding the role of reinforcement learning and attention. MathFormer is a small transformer-based seq2seq model with 4 million parameters, trained solely on the symbolic expansion task with no prior knowledge of mathematical operators or variables. It achieves near-perfect accuracy, outperforming much larger models on the same benchmark.

reddit · r/MachineLearning · /u/AlphaCode1 · Jun 27, 18:57

**Background**: Symbolic math involves manipulating expressions with variables and operators (e.g., expanding polynomials). Seq2seq models are neural networks that map sequences to sequences, often using attention mechanisms. The finding that a small model can perform this task so well suggests that complex mathematical reasoning may be reducible to recognizing and replicating structural patterns in tokens.

**Tags**: `#machine learning`, `#reasoning`, `#symbolic math`, `#LLMs`, `#attention`

---

<a id="item-4"></a>
## [NagaTranslate builds translation and voice pipeline for Nagaland's low-resource creoles](https://www.reddit.com/r/MachineLearning/comments/1uhlvjv/nagatranslate_building_a_translation_and_voice/) ⭐️ 8.0/10

The NagaTranslate project has developed a pipeline combining Whisper for speech recognition, VITS for speech synthesis, and a commercial LLM API for text translation to support languages like Nagamese, Ao, and Sema, all of which are low-resource creoles from Nagaland, India. This work addresses a critical gap in NLP for languages that were primarily oral and lack standardized orthography, demonstrating a practical architecture that could be adapted for other low-resource languages worldwide. The translation backend initially used a fine-tuned NLLB model but switched to an LLM API to improve colloquial flow; the long-term goal is to self-host open-weight models like Llama or Gemma to avoid API costs.

reddit · r/MachineLearning · /u/Material_Dinner_1924 · Jun 28, 03:05

**Background**: Low-resource NLP refers to work on languages with limited digital data and tools. VITS (Variational Inference with adversarial learning for Text-to-Speech) is a single-stage TTS model that generates natural speech from text. NLLB (No Language Left Behind) is Meta's large multilingual translation model. Nagaland's languages are oral traditions with little parallel corpora, making this a challenging low-resource scenario.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jaywalnut310/vits">GitHub - jaywalnut310/vits: VITS: Conditional Variational ... Speech Synthesis - anwarvic.github.io GitHub - daniilrobnikov/vits2: VITS2: Improving Quality and ... VITS - TTS 0.22.0 documentation - Coqui VITS-based Text-to-Speech Pipeline - emergentmind.com Understanding VITS: Revolutionizing Voice AI With Natural ...</a></li>
<li><a href="https://huggingface.co/facebook/nllb-200-3.3B">facebook/ nllb -200-3.3B · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#low-resource NLP`, `#machine translation`, `#speech synthesis`, `#whisper`, `#vits`

---

<a id="item-5"></a>
## [Do We Still Need to Study Algorithms with AI Writing Code?](https://www.reddit.com/r/MachineLearning/comments/1uhdydj/do_we_still_need_to_study_algorithms_now_that_ai/) ⭐️ 8.0/10

A Reddit user questions whether deep study of algorithms remains essential now that AI can generate efficient implementations, explain complexity, and optimize code, sparking a debate on the evolving role of foundational knowledge in software development. This discussion addresses a critical tension in computer science education and practice: how to balance deep algorithmic understanding with reliance on AI tools, which could reshape curricula, hiring practices, and the skills valued in the industry. The user distinguishes between memorizing LeetCode solutions (which they deem less important) and truly studying data structures and algorithms for months, while noting that AI tools have reduced activity on platforms like Stack Overflow.

reddit · r/MachineLearning · /u/Senior_Note_6956 · Jun 27, 21:05

**Background**: For decades, studying algorithms and data structures has been a cornerstone of computer science education, essential for writing efficient code and passing technical interviews. Recently, large language models (LLMs) like GPT-4 have demonstrated the ability to generate correct code, explain concepts, and even optimize solutions, raising questions about the necessity of deep manual expertise. This post reflects a growing sentiment that AI may change what foundational knowledge is required for developers.

**Tags**: `#algorithms`, `#AI-assisted programming`, `#computer science education`, `#software engineering`, `#LLM`

---

<a id="item-6"></a>
## [GLM 5.2 Outperforms Claude on Cybersecurity Benchmarks](https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/) ⭐️ 7.0/10

GLM 5.2, a 753B parameter open-source model, reportedly outperforms Anthropic's Claude on cybersecurity benchmarks, as reported by Semgrep. This marks a significant achievement for open-source models in a specialized domain, challenging the dominance of closed-source frontier models like Claude and raising questions about benchmark design and real-world applicability. GLM 5.2 has 753B parameters and achieves 81.0 on Terminal-Bench 2.1, close to Claude Opus 4.8's 85.0, while being open-source. However, the benchmark methodology and parameter size raise questions about practical deployment.

hackernews · jms703 · Jun 28, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48709670)

**Background**: LLMs are increasingly used in cybersecurity for tasks like vulnerability detection and threat analysis. Benchmarks like Terminal-Bench and SWE-bench Pro evaluate model performance on coding and security tasks. Open-source models have been closing the gap with proprietary ones.

<details><summary>References</summary>
<ul>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 - openlm.ai</a></li>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks - z.ai</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about benchmark validity, noting that some models may get lucky on specific tests. Others highlight the high parameter count (753B) making local deployment impractical. Some users report good practical results with GLM 5.2 for programming tasks.

**Tags**: `#LLM`, `#benchmarks`, `#cybersecurity`, `#AI models`, `#open source`

---

<a id="item-7"></a>
## [Memory Prices from 1960 to 2026 Charted](https://dam.stanford.edu/memory-prices.html) ⭐️ 7.0/10

Stanford University's DAM project published a comprehensive chart of memory prices spanning from 1960 to 2026, covering various memory technologies including core memory, drum memory, and modern DRAM. The dataset, originally from jcmit.com, has been revived and updated. This dataset provides a unique historical perspective on the cost of computer memory, enabling analysis of technology scaling, market cycles, and the impact of inflation. It helps technologists and economists understand long-term trends in hardware economics. The chart is not inflation-adjusted, which dramatically understates early costs; for example, 1960s core memory cost about $1 per bit, or $8 million per GB in today's dollars. Prices show a clear repeating cycle over the last 20 years, possibly due to fab generations and market dynamics.

hackernews · vga1 · Jun 28, 18:32 · [Discussion](https://news.ycombinator.com/item?id=48710092)

**Background**: Early computer memory technologies included magnetic core memory (1955-1975) and magnetic drum memory (1930s-1960s). Core memory used tiny ferrite rings to store bits and was non-volatile but expensive and manually assembled. DRAM replaced core by the 1970s, drastically lowering cost per bit and enabling modern computing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Magnetic-core_memory">Magnetic-core memory</a></li>
<li><a href="https://en.wikipedia.org/wiki/Magnetic_drum_memory">Magnetic drum memory</a></li>
<li><a href="https://en.wikipedia.org/wiki/Random-access_memory">Random-access memory - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted the lack of inflation adjustment makes early prices seem lower than they were, and shared personal anecdotes about paying $50-$100 per MB in the 1990s. Others discussed the cyclical price pattern and concerns about dataset longevity after the original jcmit.com site went offline.

**Tags**: `#memory prices`, `#hardware history`, `#economics`, `#computer hardware`, `#market trends`

---

<a id="item-8"></a>
## [Show HN: Zanagrams – A Minimal Word Puzzle Game](https://zanagrams.com/) ⭐️ 7.0/10

A new indie word puzzle game called Zanagrams was launched, where players connect letters to form words. The game features a minimal, polished UI and has received positive community feedback. Zanagrams stands out for its clean design and engaging gameplay, contributing to the growing ecosystem of daily word puzzles and indie games. Its positive reception suggests a potential niche audience that values minimalism and challenge. The game is compared to 'Ribbit' from Puzzmo, but with its own twist on connections. Some users noted that plural forms count as bonus words, which sparked discussion about the scoring system.

hackernews · pompomsheep · Jun 28, 15:26 · [Discussion](https://news.ycombinator.com/item?id=48708182)

**Background**: Word puzzle games like Wordle have popularized the daily-puzzle format. Zanagrams adds a twist by requiring players to connect letters rather than guess a single word, offering a different cognitive challenge.

**Discussion**: Commenters generally praised the minimal UI and satisfying animations, though some found the connection mechanic confusing initially. Comparisons to Puzzmo's Ribbit were common, and suggestions included adding a timed mode for sharing results.

**Tags**: `#puzzle`, `#game`, `#word game`, `#web app`, `#indie`

---

<a id="item-9"></a>
## [KIDS Act Would Mandate Age Checks, Raising Privacy Concerns](https://www.eff.org/deeplinks/2026/06/kids-act-would-require-age-checks-get-online) ⭐️ 7.0/10

The KIDS Act is a bipartisan US bill that would require online platforms to verify the age of users before allowing access, raising significant privacy and civil liberties concerns. This legislation could fundamentally alter internet governance by mandating age verification, potentially leading to widespread surveillance and erosion of online anonymity, affecting all internet users. The bill defines 'covered platforms' as those using personal information for advertising, marketing, or content recommendations, exempting many discussion sites and banking websites. It is sponsored by Rep. Brett Guthrie (R-KY) and co-sponsored by Rep. Frank Pallone (D-NJ).

hackernews · bilsbie · Jun 28, 11:56 · [Discussion](https://news.ycombinator.com/item?id=48706560)

**Background**: Age verification technologies range from uploading government ID to using biometrics or third-party services, but they inherently require collecting personal data. The KIDS Act is part of a broader trend in Western countries to regulate children's online safety, often criticized as a potential tool for mass surveillance. Critics argue that such mandates could lead to unintended consequences like data breaches and chilling effects on free speech.

<details><summary>References</summary>
<ul>
<li><a href="https://reclaimthenet.org/the-kids-act-a-bipartisan-mass-surveillance-megabill">The KIDS Act : A Bipartisan Mass Surveillance Megabill</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about the bill's motivations, noting the lack of robust evidence linking social media to mental health issues and suggesting that powerful lobbying groups are pushing for such legislation. Users also point out the irony of requiring personal information after years of advice to guard it online.

**Tags**: `#privacy`, `#legislation`, `#age verification`, `#internet regulation`, `#civil liberties`

---

<a id="item-10"></a>
## [Jon Udell: Keep Humans in Control of AI Agents](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 7.0/10

Jon Udell argues for flipping the 'human in the loop' narrative to an 'agent in the loop' perspective, emphasizing that humans should remain in control of agent-assisted development workflows and that agents should produce reviewable pull requests. This perspective addresses growing concerns about autonomous AI agents creating unreviewable code, promoting a human-centric approach that ensures accountability and code quality in agentic software development. Udell dislikes the phrase 'human in the loop' because it cedes authority to machines; instead, he proposes that we work the same way as always and invite agents into our loop, making the process transparent and reviewable.

rss · Simon Willison · Jun 28, 21:57

**Background**: Agentic coding uses autonomous AI agents to plan, write, test, and modify code with minimal human intervention, often producing pull requests that are hard to review. The 'human in the loop' concept traditionally places a human as a supervisor within an automated process, but Udell argues this framing incorrectly centers machines. His re-framing—'agent in the loop'—asserts that humans own the development workflow and agents are merely assistants.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases | Google Cloud</a></li>
<li><a href="https://agentdriven.dev/">AGENT DRIVEN DEVELOPMENT (ADD) PROTOCOL</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#software-development`, `#human-in-the-loop`, `#workflow`, `#coding-agents`

---

<a id="item-11"></a>
## [Minimal Interactive Transformer Visualization Lets You Edit Weights](https://www.reddit.com/r/MachineLearning/comments/1uhw7fu/i_shrank_a_transformer_until_every_number_fitted/) ⭐️ 7.0/10

A software engineer created a minimal, fully interactive transformer forward pass visualization as a single HTML file. It uses a 6-word vocabulary and 3D embeddings to compute and display every step from word vectors to probabilities, with editable weights that trigger live recomputation. This tool addresses a gap in educational resources by providing a hands-on, mathematical-level understanding of transformer internals, which is crucial for learners and practitioners. It demystifies the core components of large language models by making abstract operations tangible. The visualization includes a single attention head and a single transformer block, with full attention computation including causal masking and softmax. The page is self-contained with no dependencies, and a randomize button shows how untrained weights produce meaningless predictions.

reddit · r/MachineLearning · /u/DanielMoGo · Jun 28, 12:35

**Background**: Transformers are the foundational architecture behind large language models (LLMs) like GPT-4. The core mechanism is self-attention, which uses Query (Q), Key (K), and Value (V) matrices to compute relevance between tokens. A causal mask prevents the model from attending to future tokens, ensuring autoregressive generation. Understanding these components is essential for anyone diving into deep learning.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@jinoo/a-simple-example-of-attention-masking-in-transformer-decoder-a6c66757bc7d">A Simple Example of Causal Attention Masking in Transformer ...</a></li>
<li><a href="https://www.billparker.ai/2024/10/transformer-attention-simple-guide-to-q.html">Transformer Attention: A Guide to the Q, K, and V Matrices</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#education`, `#interactive`, `#machine learning`, `#visualization`

---

<a id="item-12"></a>
## [Picotron: LLM training framework for older GPUs without crashes](https://www.reddit.com/r/MachineLearning/comments/1uh7ib3/built_an_llm_training_framework_that_actually/) ⭐️ 7.0/10

A new open-source framework called Picotron, a clean-room rewrite of Nanotron, removes hardware-specific dependencies like flash-attn, triton, and functorch at the module level, enabling LLM training on older GPUs such as T4 and V100 without import crashes. This significantly lowers the barrier for LLM training by supporting a much wider range of GPUs, including older and budget hardware, which is a common pain point in the machine learning community. It also demonstrates a practical approach to dependency management in ML frameworks. Picotron defaults to FP16 on GPUs with compute capability below 8.0 and BF16 on newer ones, and falls back to standard PyTorch SDPA while optionally using FlashAttention-2 at runtime if detected. It includes configs for GQA, MLA, QK-Norm, logit soft-capping, parallel FFN/Attn, and ZeRO-1 on DDP.

reddit · r/MachineLearning · /u/Capital_Savings_9942 · Jun 27, 16:44

**Background**: Modern LLM training frameworks often import hardware-specific libraries like flash-attn, triton, and functorch at the module level, causing crashes on older GPUs that lack support. Nanotron is one such framework; Picotron aims to solve this by only using these dependencies at runtime when hardware supports them. Multi-head Latent Attention (MLA) is a memory-efficient attention variant introduced in DeepSeek-V2.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/triton-lang/triton">GitHub - triton-lang/triton: Development repository for the Triton language and compiler · GitHub</a></li>
<li><a href="https://github.com/pytorch/functorch">GitHub - pytorch/functorch: functorch is JAX-like composable ... torch.func — PyTorch 2.12 documentation PyTorch Functorch: A Comprehensive Guide - codegenes.net function transforms (aka torch.func, functorch) · pytorch ... functorch · PyPI Functorch: JAX-like Composable Function Transforms for PyTorch</a></li>
<li><a href="https://machinelearningmastery.com/a-gentle-introduction-to-multi-head-latent-attention-mla/">A Gentle Introduction to Multi-Head Latent Attention (MLA) - MachineLearningMastery.com</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#training`, `#GPU`, `#framework`, `#open-source`

---

<a id="item-13"></a>
## [Pybench: pytest-like CLI for statistical ML regression testing](https://www.reddit.com/r/MachineLearning/comments/1ugv7u3/i_silently_break_training_codes_or_configs_so_i/) ⭐️ 7.0/10

Pybench is a new open-source CLI tool that applies statistical tests to training metrics, comparing results against saved baselines to detect regressions. It manages random seeds and uses a pytest-like workflow with 'benchmarks/' directory. Silent metric regressions are a common pain point in ML development; pybench provides a systematic, reproducible way to catch them, improving model reliability and saving debugging time. The tool includes commands like 'pybench' to run or compare, 'update' to re-baseline after intended changes, and 'show' to display baseline stats with per-commit history. It uses statistical tests to determine pass/fail rather than simple threshold checks.

reddit · r/MachineLearning · /u/SpecificPark2594 · Jun 27, 06:33

**Background**: In machine learning, training metrics can fluctuate due to random seeds, hyperparameters, or data splits, making it hard to detect genuine regressions. Statistical tests like t-tests help determine if performance changes are significant. Pybench automates this by sampling seeds, establishing baselines, and running tests on each commit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s41598-024-56706-x">Evaluation metrics and statistical tests for machine learning | Scientific Reports</a></li>

</ul>
</details>

**Tags**: `#ML`, `#testing`, `#tooling`, `#regression`, `#statistical tests`

---

<a id="item-14"></a>
## [5k Menus from NYPL Buttolph Collection (1880-1920)](https://pudding.cool/2026/06/menu-story/) ⭐️ 6.0/10

The Pudding has created an interactive visualization exploring 5,000 digitized menus from the New York Public Library's Buttolph Collection, spanning 1880 to 1920, revealing historical food trends through curated stories and searchable data. This project makes a vast cultural dataset accessible and engaging, allowing researchers, food enthusiasts, and the general public to explore culinary history and social changes in America during a transformative period. The visualization includes menus from the Buttolph Collection, which originally contained 25,000 menus at Miss Buttolph's death; now over 18,000 have been digitized. Users can browse by year, view menu items, and follow a curated narrative.

hackernews · xbryanx · Jun 28, 14:44 · [Discussion](https://news.ycombinator.com/item?id=48707763)

**Background**: The Buttolph Collection of Menus was assembled by Frank E. Buttolph (1850-1924) who dedicated her life to collecting menus from restaurants, banquets, and events. It is one of the largest collections of historical menus in the world, housed at the New York Public Library. The Pudding is a digital publication known for data-driven storytelling and interactive visualizations.

<details><summary>References</summary>
<ul>
<li><a href="https://digitalcollections.nypl.org/collections/the-buttolph-collection-of-menus">The Buttolph collection of menus - NYPL Digital Collections</a></li>
<li><a href="https://www.thehistoryblog.com/archives/40485">Browse 18,000 historic menus in the New York Public Library – The History Blog</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm, with one noting that menus haven't changed drastically over 175 years and another sharing a cultural anecdote about German beer mats. Some recommended exploring the curated story first before browsing the full visualization.

**Tags**: `#data visualization`, `#digital humanities`, `#history`, `#design`, `#cultural heritage`

---

<a id="item-15"></a>
## [LibrePods: Open-Source Project Unlocks AirPods Features on Non-Apple Devices](https://github.com/librepods-org/librepods) ⭐️ 6.0/10

An open-source project called LibrePods has reverse-engineered Apple's proprietary AACP protocol, enabling AirPods features like noise control, ear detection, and battery status on Android, Linux, and other non-Apple devices. This project challenges Apple's ecosystem lock-in by bringing premium earbud features to a wider range of devices, potentially increasing the utility of AirPods for non-Apple users and promoting hardware interoperability. The implementation is based on reverse-engineering the Apple Accessory Communication Protocol (AACP) and is open-sourced on GitHub. However, Apple may issue firmware updates to block third-party access, and the project's long-term viability depends on continued community effort.

hackernews · rbanffy · Jun 28, 18:48 · [Discussion](https://news.ycombinator.com/item?id=48710232)

**Background**: AirPods work as standard Bluetooth earbuds on non-Apple devices, but advanced features like noise cancellation mode switching, ear detection, and accurate battery readings rely on Apple's proprietary AACP protocol. This protocol is normally only available on Apple devices, limiting AirPods functionality elsewhere.

<details><summary>References</summary>
<ul>
<li><a href="https://tekmag.thsite.top/librepods-how-an-open-source-project-brings-full-airpods-features-to-android-linux/">LibrePods: How an Open-Source Project Brings Full AirPods ...</a></li>

</ul>
</details>

**Discussion**: Community members appreciate the hacking effort but express skepticism about Apple's response—many expect Apple to patch this in future firmware. Some users question why one would buy AirPods given Apple's hostility, while others hope similar reverse-engineering can liberate other Apple features like AirDrop.

**Tags**: `#open-source`, `#AirPods`, `#bluetooth`, `#Apple`, `#reverse-engineering`

---

<a id="item-16"></a>
## [Daisugi: Japanese Technique of Growing Trees on Trees](https://www.openculture.com/2020/10/daisugi.html) ⭐️ 6.0/10

An article from Open Culture explains Daisugi, a 14th-century Japanese forestry technique where cedar trees are grown from a single base tree to produce straight, high-quality lumber. The technique was developed in the Kitayama area of Kyoto as a response to a shortage of seedlings. Daisugi offers a sustainable method for continuously harvesting timber without cutting down entire trees, producing wood that is 140% more flexible and 200% denser than standard cedar. This technique highlights ancient practices that can inspire modern sustainable forestry and woodworking. The technique is labor-intensive and specifically suited to Kitayama cedar, which naturally grows vertically but can be pruned to spread out. After creating a wide, stable base, subsequent shoots are pruned to grow straight and are harvested every 20 years.

hackernews · MaysonL · Jun 28, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48708859)

**Background**: Daisugi is a form of coppicing or pollarding, traditional methods of managing trees to promote new growth from the stump or trunk. It originated in the Muromachi period (1336-1573) when there was a high demand for straight, knot-free cedar logs used in tea ceremony architecture and other fine woodworking. The technique allows a single tree to produce multiple shoots, each of which can be harvested repeatedly over centuries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Daisugi">Daisugi - Wikipedia</a></li>
<li><a href="https://haltonmastergardeners.com/2020/08/09/daisugi-or-coppicing/">Daisugi or Coppicing – Halton Region Master Gardeners</a></li>

</ul>
</details>

**Discussion**: Commenters expressed curiosity about the technique, with some drawing dark parallels to human exploitation, while others clarified the technical details and noted that the article lacked depth. One commenter pointed out that the same discussion had occurred three years prior on Hacker News.

**Tags**: `#daisugi`, `#forestry`, `#japanese-culture`, `#sustainability`, `#nature`

---

<a id="item-17"></a>
## [Evaluating long-term memory in stateless LLM chatbots](https://www.reddit.com/r/MachineLearning/comments/1ui27i1/evaluating_longterm_memory_limits_in_stateless/) ⭐️ 6.0/10

A researcher is seeking feedback on a proposed methodology to measure recall accuracy in stateless LLM chatbots after hundreds of conversational turns without external memory. This research could help benchmark the true long-context capabilities of LLMs, revealing when and why they forget information in extended conversations, which is critical for developing more reliable chatbots. The plan involves injecting key facts early in a conversation, then conducting hundreds of unrelated turns before testing recall at different intervals, without using any external memory system.

reddit · r/MachineLearning · /u/QuietAccountant4237 · Jun 28, 16:48

**Background**: A 'stateless' LLM treats each interaction independently with no persistent internal state, so it relies solely on the provided context window. The 'needle in a haystack' test is a common benchmark for evaluating long-context retrieval by placing a specific fact within a large context. This proposed study adapts that concept to assess memory over many conversational turns, which is less explored.

<details><summary>References</summary>
<ul>
<li><a href="https://atlan.com/know/why-ai-agents-forget/">Why AI Agents Forget: The Stateless LLM Problem Explained</a></li>
<li><a href="https://arize.com/blog-course/the-needle-in-a-haystack-test-evaluating-the-performance-of-llm-rag-systems/">The Needle In a Haystack Test : Evaluating the Performance of LLM ...</a></li>
<li><a href="https://github.com/gkamradt/needle-in-a-haystack">gkamradt/ needle - in - a - haystack : Doing simple retrieval from LLM ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#long-context`, `#memory`, `#evaluation`, `#chatbots`

---

<a id="item-18"></a>
## [Steganography in ONNX Model Weights via Mantissa Bits](https://www.reddit.com/r/MachineLearning/comments/1uh61uw/hiding_messages_in_the_least_significant_mantissa/) ⭐️ 6.0/10

The author presents a project that hides messages in the least significant mantissa bits of fine-tuned ONNX model weights, using the natural weight changes from fine-tuning to conceal the steganographic alterations. This work explores a niche application of steganography to machine learning models, potentially enabling covert communication or watermarking, though it is incremental and not a major breakthrough. The method only modifies weights that change during fine-tuning, exploiting the least significant mantissa bits of floating-point numbers to reduce detectability. The author acknowledges similar ideas exist in academic literature but remain underexplored in practice.

reddit · r/MachineLearning · /u/Admin-ABC-XYZ · Jun 27, 15:45

**Background**: ONNX (Open Neural Network Exchange) is an open format for representing machine learning models, enabling interoperability between frameworks. Floating-point numbers in computers consist of a sign, exponent, and mantissa (significand); the least significant mantissa bits can be altered without significantly changing the numeric value, making them suitable for steganography. Fine-tuning a model naturally changes some weights, providing cover for hidden data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Floating-point_arithmetic">Floating-point arithmetic - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open_Neural_Network_Exchange">Open Neural Network Exchange - Wikipedia</a></li>
<li><a href="https://onnx.ai/">ONNX | Home</a></li>

</ul>
</details>

**Tags**: `#steganography`, `#machine learning`, `#model weights`, `#security`, `#ONNX`

---

<a id="item-19"></a>
## [ML Models for Searching MMA Fight Moments](https://www.reddit.com/r/MachineLearning/comments/1ugwrmz/showcase_building_ml_models_that_watch_mma_fights/) ⭐️ 6.0/10

An ex-MMA fighter and AI practitioner built machine learning models that detect positions (standing, clinching, ground) and events (knockdowns, takedowns) in MMA fights, creating searchable timelines at cagesight.ai. This application bridges domain expertise in martial arts with AI, potentially transforming how fighters, coaches, and fans analyze fights by making key moments instantly retrievable. The current models identify broad phases like standing, clinching, and ground, with plans to add more granular positions (e.g., guard, mount). The timeline at the bottom of each fight allows users to jump directly to labeled events.

reddit · r/MachineLearning · /u/UnholyCathedral · Jun 27, 08:01

**Background**: In MMA, fights transition between standing striking, clinch work, and ground fighting, each with specific positions like guard, mount, or side control. Machine learning, especially computer vision, can automatically classify video frames to detect these states, enabling efficient video indexing and analysis.

**Tags**: `#machine learning`, `#sports analytics`, `#computer vision`, `#MMA`, `#BJJ`

---