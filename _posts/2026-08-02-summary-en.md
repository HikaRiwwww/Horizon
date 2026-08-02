---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 35 items, 17 important content pieces were selected

---

1. [Stateless MCP 2.0 Reignites Interest, Inspires Two New Tools](#item-1) ⭐️ 9.0/10
2. [ByteDance Unveils Seedance 2.5 for Long-Form, Referenced AI Video Generation](#item-2) ⭐️ 8.0/10
3. [Diátaxis Framework Gains Traction in Technical Documentation Discussions](#item-3) ⭐️ 8.0/10
4. [Lean Kernel Soundness Bug #14576 Postmortem Published](#item-4) ⭐️ 8.0/10
5. [How Google's Killing of Google Reader Destroyed RSS Adoption](#item-5) ⭐️ 8.0/10
6. [OpenAI's Astra Model Solves Ten Long-Standing Math Problems](#item-6) ⭐️ 8.0/10
7. [DeepSeek V4-Flash-0731: 304B Model, Best Cost-Per-Intelligence](#item-7) ⭐️ 8.0/10
8. [Simon Willison Discusses Open-Weight Model Revolution on Oxide and Friends](#item-8) ⭐️ 8.0/10
9. [Study Probes How Symmetric Representations Emerge Inside KataGo's Go Networks](#item-9) ⭐️ 8.0/10
10. [AI Financial Advice Is Surprisingly Good, Especially with Right Questions](#item-10) ⭐️ 7.0/10
11. [No Starch Press Releases 800-Page 64-Bit Assembly Book](#item-11) ⭐️ 7.0/10
12. [llm-mcp-client 0.1a0 adds stateless MCP support to llm CLI](#item-12) ⭐️ 7.0/10
13. [smevals: A Small Eval Suite for Models, Prompts, and Harnesses](#item-13) ⭐️ 7.0/10
14. [VLM Benchmarks Mask Clinical Term Erasure in Radiology Reports](#item-14) ⭐️ 7.0/10
15. [uv 0.12.1 Adds Per-Package Prerelease Policies and Local HTML Indexes](#item-15) ⭐️ 6.0/10
16. [Datasette Agent 0.4a0 enables tools to run JavaScript in user's browser](#item-16) ⭐️ 6.0/10
17. [User Trains Transformer Model to Predict Blood Sugar Levels](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Stateless MCP 2.0 Reignites Interest, Inspires Two New Tools](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 9.0/10

The 2026-07-28 Model Context Protocol specification (MCP 2.0 / Stateless MCP) was rolled out, removing the initialization handshake and session IDs so tool calls can be made with a single HTTP request. Simon Willison built mcp-explorer and datasette-mcp to explore the new protocol. This is the most significant change to MCP since its launch, dramatically lowering the complexity of implementing clients and servers. It makes MCP tools easier to audit and control than giving agents a shell, and better suited for scalable web applications and smaller on-device models. Under stateless MCP, a tools/call request uses headers like MCP-Protocol-Version, Mcp-Method, and Mcp-Name instead of a two-step initialize-and-session flow. The spec also includes Multi Round-Trip Requests, header-based routing, cacheable list results, authorization hardening, and a formal extensions framework. Simon's new mcp-explorer is a CLI for interactively probing MCP servers.

rss · Simon Willison · Jul 31, 23:13

**Background**: MCP is an open standard introduced by Anthropic in November 2024 to connect AI assistants to external tools and data. It surged in popularity during 2025 but was partly eclipsed by Anthropic's Skills, which let agents use a terminal and curl more flexibly. Stateless MCP addresses auditing and control concerns by keeping tool calls as simple, stateless HTTP requests that are easy to implement and scale.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/seps/2575-stateless-mcp">SEP-2575: Make MCP Stateless - Model Context Protocol</a></li>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28/">The 2026-07-28 Specification | Model Context Protocol Blog</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#AI`, `#LLM`, `#protocol`, `#agents`

---

<a id="item-2"></a>
## [ByteDance Unveils Seedance 2.5 for Long-Form, Referenced AI Video Generation](https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5) ⭐️ 8.0/10

ByteDance has announced Seedance 2.5, its next-generation AI video generation model, capable of creating 30-second clips in 4K with multimodal referencing and localized editing. The model is available through Dreamina and the Doubao API. This release strengthens ByteDance's position in the competitive AI video generation market, offering creators cinematic-quality output with flexible control. Its focus on action and high-effect shots reflects differing regional demands, while challenging Western-facing models. Seedance 2.5 supports up to 50 multimodal references (text, image, video, audio) and includes localized editing to modify specific regions of a scene. It is positioned for cinematic advertising and social media videos, with API access through CometAPI and ByteDance's Dreamina platform.

hackernews · njaremko · Aug 1, 20:45 · [Discussion](https://news.ycombinator.com/item?id=49138302)

**Background**: AI video generation models create new video content from text prompts or reference images using deep learning. Seedance is ByteDance's family of video-generation models; the 2.5 release builds on previous versions by increasing clip length to 30 seconds and refining control. These models are increasingly used for storyboards, advertisements, and short-form social content, though they still face limitations in dialogue-driven scenes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seeddance.io/models/seedance-2-5">Seedance 2 . 5 Free: Try ByteDance AI Video , No Queue, Instant Results</a></li>
<li><a href="https://dreamina.capcut.com/seedance/seedance-2-5">Official Seedance 2 . 5 : 4K & 30s AI Video Generator</a></li>
<li><a href="https://www.cometapi.com/models/doubao/doubao-seedance-2-5/">Affordable Seedance - 2 - 5 API | text-to- video | CometAPI</a></li>

</ul>
</details>

**Discussion**: Comments praised the visual quality but noted the model emphasizes action over dialogue, contrasting with US filmmakers' interest in actor-consistent video-to-video. Some users raised concerns about inference costs and pointed out that MiniMax H3 would soon be open-weights with acceptable performance on consumer GPUs.

**Tags**: `#AI video generation`, `#Seedance`, `#ByteDance`, `#text-to-video`, `#machine learning`

---

<a id="item-3"></a>
## [Diátaxis Framework Gains Traction in Technical Documentation Discussions](https://diataxis.fr/) ⭐️ 8.0/10

Diátaxis, a systematic framework for technical documentation, is gaining renewed attention as practitioners on Hacker News share adoption experiences. The framework's author, Daniele Procida, also highlighted ongoing translation efforts into multiple languages. The framework provides a clear, practical way to structure documentation into four types, helping teams create docs that meet user needs. Its growing adoption and community validation suggest it is becoming a standard reference for technical writing, though maintenance challenges remain a concern. Diátaxis organizes documentation into tutorials, how-to guides, reference, and explanation, each with a distinct purpose and style. The author is currently translating the framework at diataxis.fr/translation, and teams such as Canonical and Gatsby have restructured their documentation around it.

hackernews · ryanseys · Aug 1, 20:33 · [Discussion](https://news.ycombinator.com/item?id=49138188)

**Background**: Diátaxis is a lightweight framework created by Daniele Procida for organizing technical documentation. It identifies four distinct modes—tutorials, how-to guides, reference, and explanation—that correspond to different user needs during their interaction with a product. The framework helps writers decide what content to create and how to style it, and has been adopted by major open-source projects.

<details><summary>References</summary>
<ul>
<li><a href="https://diataxis.fr/">Diátaxis</a></li>
<li><a href="https://ubuntu.com/blog/diataxis-a-new-foundation-for-canonical-documentation">Diátaxis, a new foundation for Canonical documentation - Ubuntu What is Diátaxis and should you be using it with your ... GitHub - evildmp/diataxis-documentation-framework: A ... Diátaxis Framework: Organize Documentation for Users, Not Authors Start here - Diátaxis in five minutes - Diátaxis - diataxis.fr Diataxis Documentation Framework Template - GitHub</a></li>
<li><a href="https://idratherbewriting.com/blog/what-is-diataxis-documentation-framework">What is Diátaxis and should you be using it with your ...</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive: one user called Diátaxis 'fantastic' for handling a complex codebase handover, while another appreciated the lack of 'certifications, training, manifestos, and job ads'. However, some raised concerns about documentation drift and the difficulty of keeping tutorials and reference materials up to date over time.

**Tags**: `#documentation`, `#technical-writing`, `#software-engineering`, `#knowledge-management`, `#diataxis`

---

<a id="item-4"></a>
## [Lean Kernel Soundness Bug #14576 Postmortem Published](https://leodemoura.github.io/blog/2026-8-1-postmortem-for-kernel-soundness-bug-14576/) ⭐️ 8.0/10

Leo de Moura published a postmortem of kernel soundness bug #14576 in the Lean theorem prover. It demonstrates how a crafted proof exploited a bug and slipped past independent checking, emphasizing that verified results are strong but not absolute guarantees. Lean is widely used in formal verification and mathematics, so a kernel soundness bug has serious implications for anyone relying on its guarantees. This incident highlights that even trusted proof assistants can have subtle flaws, reinforcing the need for updated tools and cautious interpretation of verification results. According to discussion, the exploit was crafted to hit two unrelated bugs in two independently written checkers, so independent checking still works but requires current versions of both implementations. The bug is an implementation error rather than a meta-theory flaw, and the postmortem suggests follow-up work on checking proof objects more rigorously.

hackernews · juhopitk · Aug 1, 18:32 · [Discussion](https://news.ycombinator.com/item?id=49137060)

**Background**: Lean is a proof assistant and functional programming language based on the Calculus of Inductive Constructions, used to formalize mathematics and verify software. A kernel is the small trusted component that verifies every proof, and soundness means it never accepts an invalid proof. Historical soundness bugs have also occurred in other assistants such as Coq, Isabelle, and Agda. Independent proof checking can provide extra assurance, but as this incident shows, multiple checkers can share blind spots.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>
<li><a href="https://sourcefeed.dev/a/the-collatz-disproof-that-beat-two-proof-checkers-2">The Collatz 'Disproof' That Beat Two Proof Checkers — SourceFeed</a></li>
<li><a href="https://lawrencecpaulson.github.io/2026/07/30/Collatz.html">Why is it all in the kernel ?</a></li>

</ul>
</details>

**Discussion**: Commenters noted that soundness bugs also occur in simpler systems like Rust's type checker, and that verified results should be regarded as extraordinarily strong but not absolute. Some argued that such bugs reflect a drawback of complex systems compared to simpler ones like Metamath, while others asked whether an exploit could prove a previously unproven statement without directly proving false.

**Tags**: `#Lean`, `#formal verification`, `#soundness`, `#proof assistants`, `#kernel bug`

---

<a id="item-5"></a>
## [How Google's Killing of Google Reader Destroyed RSS Adoption](https://openrss.org/blog/how-google-helped-destroy-adoption-of-rss-feeds) ⭐️ 8.0/10

The blog post analyzes how Google, particularly through the 2013 shutdown of Google Reader, contributed to the decline of RSS adoption. It argues that Google's stated reason of declining usage was a disingenuous excuse, as the company was simultaneously pushing its own social network, Google+. This matters because RSS is a foundational open web standard that enables decentralized content distribution, and Google's decision had a chilling effect on its ecosystem. The analysis is relevant to ongoing concerns about walled gardens and the consolidation of web control by a few large tech companies. Google Reader was launched in 2005 and shut down in July 2013, ostensibly due to declining usage. However, critics at the time noted that Google was aggressively promoting Google+, which had far fewer users, and this inconsistency fueled suspicions about the real motives behind the closure.

hackernews · pudgywalsh · Aug 1, 18:07 · [Discussion](https://news.ycombinator.com/item?id=49136821)

**Background**: RSS stands for Really Simple Syndication, an XML-based format that lets users subscribe to website updates without manually visiting each site. Google Reader, created in 2005, was one of the most popular RSS aggregators; when it was shut down, millions of users were forced to migrate to alternatives like Feedly. The closure, coupled with the rise of social media algorithms, contributed to a broader decline in RSS adoption. Despite this, RSS remains in use, particularly for podcasts and by developers who value open standards.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RSS">RSS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Reader">Google Reader - Wikipedia</a></li>
<li><a href="https://www.gloomba.com/en/why-was-google-reader-discontinued/">Why Was Google Reader Discontinued? A Deep Dive into Its ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia for the early 2000s internet and resentment toward Google's disingenuous justification for killing Google Reader, since Google+ was struggling. Many noted that RSS is not actually dead, with some recommending alternatives like NetNewsWire, and some lamented that the closure felt like the end of the open internet as they knew it.

**Tags**: `#RSS`, `#Google`, `#Web History`, `#Open Standards`, `#Google Reader`

---

<a id="item-6"></a>
## [OpenAI's Astra Model Solves Ten Long-Standing Math Problems](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 8.0/10

OpenAI announced that an internal version of its upcoming Astra model solved ten open problems in mathematics and theoretical computer science, with each solution costing less than $2,000 in GPT-5.6 Sol token prices. The company released Lean 4 formalizations and a paper describing the proofs. This is a landmark demonstration that frontier AI models can produce verifiable research results at low cost, potentially accelerating a shift toward 'big mathematics' where humans and machines collaborate. It also intensifies the competitive race with Anthropic, which recently showed Claude discovering cryptographic weaknesses. The targeted problems had seen no progress on their main results for at least a decade. OpenAI shared the openai/ten-proofs repository with Lean 4 formalizations, plus a paper and an LLM-generated reasoning walkthrough, but did not disclose how many problems were attempted without success.

rss · Simon Willison · Aug 1, 20:34

**Background**: Large language models (LLMs) like OpenAI's Astra are trained on vast text data and can generate mathematical reasoning, but results often need verification. Lean 4 is an interactive theorem prover that lets computers check proofs step by step, making AI-generated mathematics auditable. The announcement follows Anthropic's Claude Mythos work on cryptographic weaknesses and aligns with Terence Tao's vision of 'big mathematics'—large-scale human-machine collaboration on complex problems.

<details><summary>References</summary>
<ul>
<li><a href="https://runtimewire.com/article/openai-astra-ten-open-math-problems">OpenAI says unreleased Astra model solved 10 open... - RuntimeWire</a></li>
<li><a href="https://scalevise.com/resources/openai-public-materials-no-astra-model/">OpenAI Public Materials Do Not List Astra</a></li>
<li><a href="https://www.cometapi.com/gpt-5-6-pricing/">GPT-5.6 Pricing 2026: Sol, Terra & Luna API Costs - CometAPI</a></li>

</ul>
</details>

**Discussion**: Discussion on Hacker News and among mathematicians is split between excitement and anxiety. Some see it as a 'Deep Blue moment' for mathematics, while others like Kirwin Hampshire describe a 'profound spiritual crisis'; a common demand is more transparency, especially the prompts used and the failure cases.

**Tags**: `#AI`, `#mathematics`, `#OpenAI`, `#research`, `#LLM`

---

<a id="item-7"></a>
## [DeepSeek V4-Flash-0731: 304B Model, Best Cost-Per-Intelligence](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek released V4-Flash-0731, a 304B parameter model with substantially enhanced agentic capabilities, now available on Hugging Face and via OpenRouter. Artificial Analysis ranks it ahead of MiniMax M3 (428B), with pricing of $0.14 per million input tokens and $0.27 per million output tokens. At this price-performance point, V4-Flash-0731 may currently be the best value-per-intelligence model available, making frontier-level capabilities more accessible to developers. It also underscores how mid-sized, efficiently trained models can rival far larger ones, intensifying competition in the LLM market. The model weighs 304B parameters (167GB on Hugging Face) and is accessed via OpenRouter; output quality varies significantly with reasoning effort — default low effort gave poor results, while setting reasoning_effort to high produced much better images. Artificial Analysis places it on the far left of the Pareto frontier on its Intelligence Index vs. Cost per Task chart.

rss · Simon Willison · Jul 31, 23:59

**Background**: Agentic AI refers to LLM-driven systems that exhibit goal-directed behavior, use natural language interfaces, can call external tools, and handle multi-step tasks. Artificial Analysis's Intelligence Index aggregates several benchmarks (such as GPQA Diamond and Humanity's Last Exam) into a weighted score, and its cost-per-task metric divides weighted API costs by task count. This allows direct comparison of intelligence per dollar across models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://artificialanalysis.ai/methodology/intelligence-benchmarking">Artificial Analysis Intelligence Benchmarking Methodology</a></li>
<li><a href="https://artificialanalysis.ai/models">Comparison of AI Models across Intelligence, Performance, and Price</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM`, `#AI model`, `#agentic AI`, `#cost efficiency`

---

<a id="item-8"></a>
## [Simon Willison Discusses Open-Weight Model Revolution on Oxide and Friends](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 8.0/10

Simon Willison joined the Oxide and Friends podcast on Monday to discuss a turbulent week for AI, highlighting how Kimi K3 demonstrated that open-weight models can rival proprietary frontier models. The conversation also covered accidental cybersecurity incidents and industry-wide public letters supporting open weights, signed by nearly every major AI player except Anthropic. This episode captures a pivotal moment where open-weight models reached frontier-level performance, potentially reshaping the competitive landscape between open and closed AI ecosystems. The discussion's timing underscores how fast the field is moving, with developments like DeepSeek V4 Flash emerging immediately after recording. The podcast was recorded before the release of DeepSeek V4 Flash 0731 and Anthropic's own cyber incident, which Simon noted would have been included had they recorded later. Other topics included Golden Gate Claude, the Zizians, Alameda wild turkey attacks, Soviet Marburg virus research, and a new prediction that the Pope will say something about open models by year's end.

rss · Simon Willison · Jul 31, 21:33

**Background**: Open-weight AI models are models whose trained parameters (weights) are publicly downloadable, often under licenses that allow fine-tuning and commercial use. Kimi K3 is a 2.8-trillion-parameter model built by Moonshot AI with native vision and a 1-million-token context window, showing open weights can compete at the frontier. The industry has been debating the risks and benefits of open weights, with public letters expressing support and some companies like Anthropic raising concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://www.orcarouter.ai/blog/deepseek-v4-flash-official-release">DeepSeek V4 Flash: Official Release, Explained - orcarouter.ai</a></li>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#LLM`, `#podcast`, `#industry`

---

<a id="item-9"></a>
## [Study Probes How Symmetric Representations Emerge Inside KataGo's Go Networks](https://www.reddit.com/r/MachineLearning/comments/1vcrki2/how_symmetric_are_the_insides_of_a_go_network_r/) ⭐️ 8.0/10

David Wu, the maintainer of the open-source Go engine KataGo, released an interpretability study examining how superhuman Go networks internally represent rotation/reflection symmetries. The study finds that despite only stochastic 8-fold data augmentation during training, the network largely learns orientation-independent 'symmetric' concepts, with an unexpected finding about the remaining orientation-specific behavior. This work offers rare mechanistic insight into how deep networks exploit known symmetries without architectural constraints, relevant to both interpretability and data-efficient learning. It also helps the Go and AI communities understand how superhuman models organize game knowledge, and demonstrates that AI-assisted research writeups can be polished and educational when carefully directed. The study was written almost entirely with AI assistance under close human direction, and is aimed at readers both inside and outside machine learning. Code and detailed experiments are linked from the post, hosted on the KataGo maintainer's GitHub Pages site.

reddit · r/MachineLearning · /u/icosaplex · Aug 1, 16:18

**Background**: Go is a board game whose rules are invariant under rotations and reflections, so an ideal Go AI should treat mirrored board positions equivalently. KataGo is an open-source computer Go engine developed by David Wu that trains via self-play with an AlphaZero-like process, using stochastic 8-fold data augmentation rather than explicit symmetry enforcement. Equivariance and invariance are core concepts in deep learning: architectures can either hard-code symmetries or learn them from augmented data, and mechanistic interpretability seeks to reverse-engineer how these learned representations actually work.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo - Wikipedia</a></li>
<li><a href="https://github.com/lightvector/KataGo">GitHub - lightvector/KataGo: GTP engine and self-play ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#interpretability`, `#Go`, `#neural networks`, `#symmetry`, `#Machine Learning`

---

<a id="item-10"></a>
## [AI Financial Advice Is Surprisingly Good, Especially with Right Questions](https://mitsloan.mit.edu/ideas-made-to-matter/ai-financial-advice-surprisingly-good-especially-if-you-ask-right-questions) ⭐️ 7.0/10

MIT Sloan's Ideas Made to Matter reports that AI-provided financial advice is surprisingly effective, and that its quality improves significantly when users ask the right questions. The article highlights the importance of prompt design in eliciting useful and responsible financial guidance from large language models. This finding suggests AI could democratize access to financial planning, which has traditionally been expensive and reserved for the wealthy. However, it also raises concerns about the reliability, accountability, and potential commercial biases of AI-generated advice, especially as financial firms begin to integrate these tools. The article emphasizes that the way users phrase their questions—an example of prompt engineering—greatly affects the output quality, and that LLMs may perform better on well-understood financial best practices than on complex trade-off decisions. Community commenters also note that LLMs lack the personal context and 'skin in the game' of human advisors, which could lead to different risk assessments.

hackernews · foxtrot8672 · Aug 1, 22:25 · [Discussion](https://news.ycombinator.com/item?id=49139102)

**Background**: Large language models (LLMs) are neural networks trained on vast amounts of text to perform language generation and understand human-like prompts. Prompt engineering is the practice of carefully structuring those prompts to obtain the desired output from a generative AI model. The MIT Sloan article builds on the idea that LLMs can handle not only general knowledge but also domain-specific tasks like financial advice, where standardized principles often apply. This background is relevant because understanding how prompts and LLMs function explains why 'asking the right questions' is so important.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_engineering">Prompt engineering - Wikipedia</a></li>
<li><a href="https://aws.amazon.com/what-is/prompt-engineering/">What is Prompt Engineering ? - AI Prompt Engineering Explained...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were generally intrigued but skeptical: some argued that financial illiteracy is far worse than most people think, making AI advice deeply valuable, while others predicted that financial planners will be among the first industries to be disrupted. One user warned that AI responses may eventually be altered by advertising and gambling interests, and another pointed out that LLMs struggle with complex, nested trade-off decisions, which could limit their usefulness in personalized planning.

**Tags**: `#AI`, `#Finance`, `#LLM`, `#Research`, `#Advice`

---

<a id="item-11"></a>
## [No Starch Press Releases 800-Page 64-Bit Assembly Book](https://nostarch.com/art-64-bit-assembly-v2) ⭐️ 7.0/10

No Starch Press has released "The Art of 64-bit Assembly," an 800-page guide to 64-bit assembly programming using the Microsoft Macro Assembler (MASM). The book covers low-level programming concepts and modern tooling, and has sparked community discussion about assembly's relevance today. This book matters because it provides a comprehensive, modern treatment of 64-bit assembly for Windows, a niche but enduringly relevant skill for understanding performance, reverse engineering, and low-level systems. The discussion around it highlights ongoing debates about whether assembly is still worth learning and how tools like MASM compare to alternatives like GNU Assembler (GAS). The book is roughly 800 pages and uses MASM, which Microsoft ships as ml64.exe for x64 development in Visual Studio. MASM includes a macro language with looping, arithmetic, and string processing features that GAS lacks, according to the discussions. Some community members noted the book's opening references AI-generated text, which drew criticism.

hackernews · 0x54MUR41 · Aug 1, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49134599)

**Background**: Assembly language is a low-level programming language that corresponds directly to machine instructions, used when developers need precise control over hardware or maximum performance. MASM (Microsoft Macro Assembler) is an x86 assembler using Intel syntax for MS-DOS and Windows, with ML64 as the version for 64-bit sources in Visual Studio. While most modern development uses higher-level languages, assembly remains important for bootloaders, drivers, performance-critical code, and reverse engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Macro_Assembler">Microsoft Macro Assembler - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/cpp/assembler/masm/microsoft-macro-assembler-reference?view=msvc-170">Microsoft Macro Assembler reference | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: The discussion is substantial but mixed in sentiment. One commenter complained that the thread focused on marketing copy, tool choice, and LLM-generated text rather than the book's content, while others defended learning assembly as still meaningful and shared practical experience with MASM and building compilers. A user also asked whether there is a Linux equivalent book, reflecting cross-platform interest.

**Tags**: `#assembly`, `#low-level programming`, `#64-bit`, `#MASM`, `#book`

---

<a id="item-12"></a>
## [llm-mcp-client 0.1a0 adds stateless MCP support to llm CLI](https://simonwillison.net/2026/Jul/31/llm-mcp-client/#atom-everything) ⭐️ 7.0/10

Simon Willison released llm-mcp-client 0.1a0, an initial pre-release that adds stateless Model Context Protocol (MCP) support to the llm command-line tool. The release is an early alpha version, as indicated by the 0.1a0 version string. This release integrates MCP, the emerging standard for connecting LLMs to external tools and data, with one of the most popular CLI tools for running language models. It signals maturing developer tooling around MCP and will interest developers who want to use MCP servers from the command line. The tool provides stateless MCP support, meaning requests are handled independently without retaining session state between calls. It is an alpha release, so API details and behavior may change before a stable version.

rss · Simon Willison · Jul 31, 23:03

**Background**: MCP (Model Context Protocol) is an open standard introduced by Anthropic in November 2024 to standardize how AI systems integrate with external tools and data sources. The llm tool, created by Simon Willison, is a CLI and Python library for interacting with many large language models via remote APIs or locally installed models. A stateless protocol, such as HTTP, does not retain session state between requests, which improves scalability and reliability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stateless_protocol">Stateless protocol</a></li>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the ...</a></li>

</ul>
</details>

**Tags**: `#llm`, `#model-context-protocol`, `#mcp`, `#release`, `#ai-tools`

---

<a id="item-13"></a>
## [smevals: A Small Eval Suite for Models, Prompts, and Harnesses](https://simonwillison.net/2026/Jul/31/smevals/#atom-everything) ⭐️ 7.0/10

Simon Willison announced smevals, a new open-source eval suite developed with Prime Radiant, for comparing models, prompts, and harnesses. The tool is driven via `uvx smevals`, supports running evals against multiple models, and separates run execution from grading. It provides a lightweight, practical tool for LLM evaluation that can be driven by coding agents, lowering the barrier for teams to compare models and prompts. This could influence how developers select models and harnesses across the AI ecosystem. An eval is defined as a directory of YAML files containing tasks and checkers. Runs are graded separately, and results can be explored via a localhost web server or built into static HTML. The tool defines a clear vocabulary: eval, task, config, run, runner, grader, check, and checker.

rss · Simon Willison · Jul 31, 21:15

**Background**: An eval harness is the infrastructure that runs LLM evaluations end to end, typically using standardized benchmarks to ensure fair and reproducible comparisons. uvx is a command from the uv package that runs Python CLI tools in temporary, isolated environments. A coding agent is an AI that can plan, write, and execute code with minimal human intervention, and can be used to drive tools like smevals.

<details><summary>References</summary>
<ul>
<li><a href="https://pydevtools.com/handbook/reference/uvx/">uvx: Run Python CLI Tools in Isolated Environments</a></li>
<li><a href="https://www.openhands.dev/blog/what-are-coding-agents">What Are Coding Agents? A Developer's Guide to Agentic Coding ...</a></li>
<li><a href="https://www.bestaiweb.ai/what-is-an-evaluation-harness-and-how-standardized-frameworks-benchmark-llms/">What Is an Evaluation Harness? How LLM Benchmarks Work</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#evals`, `#open-source`, `#tooling`

---

<a id="item-14"></a>
## [VLM Benchmarks Mask Clinical Term Erasure in Radiology Reports](https://www.reddit.com/r/MachineLearning/comments/1vcipzz/vlms_can_score_well_on_benchmarks_while_silently/) ⭐️ 7.0/10

A new paper argues that current evaluation metrics for radiology report generation reward repetitive, clinically empty outputs while silently erasing rare but meaningful medical terms. The authors introduce a framework to measure clinical terminology erasure and hallucinated bias in vision-language models (VLMs). This matters because high benchmark scores in medical VLMs may not reflect clinical utility, potentially leading to unsafe deployment of AI-generated radiology reports. The proposed measurement framework could drive more clinically meaningful evaluation standards. The paper is titled 'Measuring What VLMs Don't Say: Validation Metrics Hide Clinical Terminology Erasure in Radiology Report Generation' (arXiv:2603.01625). It specifically targets the erasure of clinically meaningful but rare words and the introduction of biased terms, which existing metrics like BLEU and ROUGE fail to capture.

reddit · r/MachineLearning · /u/ade17_in · Aug 1, 09:27

**Background**: Vision-language models (VLMs) are increasingly used in medical imaging to generate radiology reports from chest X-rays. However, standard evaluation metrics for radiology report generation often reward lexical similarity to reference reports rather than clinical correctness, allowing models to score high by producing generic 'normal' templates. Existing metrics such as BLEU, ROUGE, and even entity-aware metrics have known limitations in capturing factual correctness. This work proposes a framework to explicitly measure term erasure and bias, aiming to align evaluation with clinical utility.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2406.16845">RaTEScore: A Metric for Radiology Report Generation RaTEScore: A Metric for Radiology Report Generation - ACL ... RaTEScore: A Metric for Radiology Report Generation GREEN: Generative Radiology Report Evaluation and Error Notation GitHub - MAGIC-AI4Med/RaTEScore: [EMNLP 2024] RaTEScore: A ... RaTEScore: A Metric for Radiology Report Generation - medRxiv</a></li>
<li><a href="https://www.nature.com/articles/s44387-025-00015-9">Vision-language foundation model for 3D medical imaging</a></li>

</ul>
</details>

**Tags**: `#VLM`, `#evaluation metrics`, `#medical AI`, `#radiology`, `#benchmarks`

---

<a id="item-15"></a>
## [uv 0.12.1 Adds Per-Package Prerelease Policies and Local HTML Indexes](https://github.com/astral-sh/uv/releases/tag/0.12.1) ⭐️ 6.0/10

uv 0.12.1 was released on July 31, 2026. It adds package-specific pre-release policies via `--prerelease-package`, support for local HTML files as flat indexes, Xonsh activation scripts, and preview features such as automatic fixes for `uv check`. As one of the most popular Python package managers, uv keeps expanding its capabilities, making dependency management more flexible and convenient. The preview features show uv's ongoing evolution toward a full-suite Python toolchain. Performance improvements include direct parsing of canonical uv lockfiles and accelerated SHA-256 hashing on non-Windows ARM64 platforms. Bug fixes cover workspace-root dependency groups, `--find-links` resolution relative to the containing file, and respecting configured indexes in `uv tool list --outdated`.

github · astral-automations-bot[bot] · Jul 31, 19:43

**Background**: uv is a Rust-based Python package and project manager developed by Astral, designed to replace pip, pip-tools, and virtualenv workflows. Per-package pre-release policies allow users to enable pre-release versions only for specific packages, and flat indexes refer to simple directory- or HTML-based package indices. Xonsh is a Python-powered shell, and activation scripts let its virtual environments be activated directly in that shell.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/uv/releases">Releases: astral-sh/uv - GitHub</a></li>
<li><a href="https://github.com/astral-sh/uv/issues/16650">allow configuring `prerelease` per-package · Issue #16650 ...</a></li>

</ul>
</details>

**Tags**: `#Python`, `#package manager`, `#uv`, `#release`, `#tooling`

---

<a id="item-16"></a>
## [Datasette Agent 0.4a0 enables tools to run JavaScript in user's browser](https://simonwillison.net/2026/Jul/31/datasette-agent/#atom-everything) ⭐️ 6.0/10

The datasette-agent 0.4a0 release introduces a new `await context.browser_task()` mechanism that allows agent tools to execute custom JavaScript directly in the user's browser. This capability was used to add a debug loop to datasette-apps 0.2a0. This new browser-execution capability significantly expands what Datasette Agent plugins can do, enabling interactive, in-browser automation and debugging workflows. It also reflects a broader industry trend of giving LLM-powered agents direct control over the user's browser environment. The mechanism is defined in pull request #33 and is available as `await context.browser_task()` inside agent tools. Since this is an alpha release (0.4a0), the API may change before a stable version.

rss · Simon Willison · Jul 31, 14:14

**Background**: Datasette is an open-source tool for exploring and publishing data, and Datasette Agent is an AI assistant built on LLM that helps users ask questions about data and runs SQL queries to find answers. The new browser_task mechanism lets plugins extend the agent by running JavaScript in the user's browser, opening up new possibilities for interactive data exploration and debugging. This is part of a larger trend of browser automation tools for AI agents, such as Playwright-based browser automation in Microsoft Foundry and other agent frameworks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette/ datasette - agent : An LLM-powered agent for...</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#LLM tool use`, `#agent`, `#browser`, `#release`

---

<a id="item-17"></a>
## [User Trains Transformer Model to Predict Blood Sugar Levels](https://www.reddit.com/r/MachineLearning/comments/1vc1txc/i_have_trained_a_model_to_predict_my_blood_sugar_p/) ⭐️ 6.0/10

A Reddit user trained an encoder-only BERT-style transformer that takes past glucose, carb, and insulin history plus future carb and insulin data to predict blood glucose for the next two hours. The model uses DILATE and pinball losses, and the source code was released under the MIT license. This project is a notable personal application of modern transformer architectures to a practical health problem, demonstrating how deep learning can be used for personalized glucose forecasting. It may encourage further research into using large pretrained models for diabetes management and wearable health data. The architecture uses bidirectional attention with future blood glucose masked, supports a variable context length of 8-24 hours, and can run autoregressively to predict beyond two hours. The largest model has about 17 million parameters (16 layers, 16 heads), pretraining took roughly 48 hours, finetuning under 10 minutes, and a nano version has fewer than 40K parameters.

reddit · r/MachineLearning · /u/0xdeadf1sh · Jul 31, 20:09

**Background**: DILATE is a differentiable loss function that penalizes both shape and temporal localization errors in time-series prediction, making it suitable for tasks like glucose forecasting where timing is critical. Pinball loss is used in quantile regression to estimate conditional quantiles, enabling the model to output uncertainty bands around predictions. Kovatchev risk space is a nonlinear transformation of blood glucose values that reflects the asymmetric clinical risk of hypo- versus hyperglycemia, which is useful for models that prioritize clinically relevant accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://openreview.net/pdf?id=ryxarpcfTB">Re: Shape and Time Distortion Loss for Training Deep Time Series</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quantile_regression">Quantile regression - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1474667016416216">Model-Based Control of Type 1 Diabetes in “Risk Space”</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#blood glucose prediction`, `#machine learning`, `#health`

---