---
layout: default
title: "Horizon Summary: 2026-08-12 (EN)"
date: 2026-08-12
lang: en
---

> From 40 items, 22 important content pieces were selected

---

1. [Hand-Set Transformer Weights Beat Frontier Models at Multiplication Without Training](#item-1) ⭐️ 9.0/10
2. [Nvidia Debuts Nemotron 3.5 Lightning and NeMo Switchyard](#item-2) ⭐️ 8.0/10
3. [Modular Releases Mojo 1.0 for High-Performance AI Development](#item-3) ⭐️ 8.0/10
4. [New Attack Extracts Hidden Reasoning Traces from Proprietary LLM APIs](#item-4) ⭐️ 8.0/10
5. [CFTC Declares Market Emergency, Orders Kalshi to Keep Operating in New York](#item-5) ⭐️ 8.0/10
6. [xAI's Grok Bot Brings Context-Managing Browser Agents to the Forefront](#item-6) ⭐️ 8.0/10
7. [Meta Introduces Muse Glimmer: 30B Open-Weight Agentic Model](#item-7) ⭐️ 8.0/10
8. [Decoupled Descent: AMP Onsager Corrections Ensure Train-Test Error Alignment](#item-8) ⭐️ 8.0/10
9. [Study: Long Benign Context Decouples RLHF Alignment in Gemma-3 via Activation Drift](#item-9) ⭐️ 8.0/10
10. [HyperSAE: Decoupled Poincaré Geometry Cuts SAE MSE by 9.8%, Dead Latents to 0.2%](#item-10) ⭐️ 8.0/10
11. [Compression and Prediction: Two Sides of the Same Coin](#item-11) ⭐️ 7.0/10
12. [OpenAI's Head of Ethics Departs After Less Than a Year](#item-12) ⭐️ 7.0/10
13. [Pen Plotter Creates Scratch Holograms](#item-13) ⭐️ 7.0/10
14. [Go Touted as Ideal for AI-Assisted Software Engineering](#item-14) ⭐️ 7.0/10
15. [England on Track to Eliminate Hepatitis C Through Screening and Treatment](#item-15) ⭐️ 7.0/10
16. [No Lossless AI Text Rewrites: Engineers Must Own Every Sentence](#item-16) ⭐️ 7.0/10
17. [fru: A Fast Rust-Based Random Forest Library for Python and R](#item-17) ⭐️ 7.0/10
18. [Synthetic Query Probing Compares Embedding Models](#item-18) ⭐️ 7.0/10
19. [Tencent's WorldClaw: Agentic 3D open-world generation at scale](#item-19) ⭐️ 6.0/10
20. [AAAI 2027 Reviewer Concerned by Lack of Code Submissions](#item-20) ⭐️ 6.0/10
21. [Reddit user seeks complaint process for CVPR 2026 paper with unreleased dataset](#item-21) ⭐️ 6.0/10
22. [Agentic World Cup Lets LLMs Compete in 1v1 Soccer](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Hand-Set Transformer Weights Beat Frontier Models at Multiplication Without Training](https://www.reddit.com/r/MachineLearning/comments/1vkrnb5/transformers_are_famously_bad_at_arithmetic_so_i/) ⭐️ 9.0/10

Reddit user /u/notforrob hand-crafted the weights of a stock Phi-3 transformer using a custom compiler called Torchwright, with no training. The compiled three-digit multiplier answers all 3,000,000 supported expressions correctly, and published checkpoints support up to 12-digit by 12-digit multiplication. This shows that a stock transformer can perform exact arithmetic when its weights are directly compiled rather than learned, challenging the assumption that training is required for capability. It also highlights how far frontier LLMs lag on exact multiplication—five of six models scored 0/500 at seven-digit inputs—and supports the growing push toward mechanistic interpretability and weight compilation. Four versions were built—grade-school, hardware-style, scratchpad, and brute-force memorization—which compute the same function with very different trade-offs in layers, width, generated tokens, and parameters. The compiled checkpoint loads into an unmodified Phi-3 Hugging Face model with no custom architecture code.

reddit · r/MachineLearning · /u/notforrob · Aug 10, 17:37

**Background**: Transformers are normally trained by gradient descent on massive text corpora, which makes exact arithmetic difficult because the calculations are not directly encoded in the weights. Mechanistic interpretability seeks to reverse-engineer neural networks the way one would analyze conventional software, and the compiled-transformer approach derives weights from a computation graph using linear algebra instead of training. This work effectively treats an algorithm as source code and the model checkpoint as the compiled binary.

<details><summary>References</summary>
<ul>
<li><a href="https://data-today.net/transformer-compiler-no-training/">A compiler that skips training and writes transformer weights</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://cyber.page/compiled-transformers/">compiled transformers — Cyber</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#arithmetic`, `#mechanistic interpretability`, `#weight compilation`, `#AI`

---

<a id="item-2"></a>
## [Nvidia Debuts Nemotron 3.5 Lightning and NeMo Switchyard](https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/) ⭐️ 8.0/10

Nvidia introduced Nemotron 3.5 Lightning, an open 30B MoE model with 3B active parameters, alongside NeMo Switchyard, an open-source library for routing LLM requests across models. The model delivers up to 4x faster output and 30% faster agentic task completion than comparable models. This release highlights the industry's pivot toward lean, specialized models and intelligent routing instead of ever-larger dense checkpoints. Developers building autonomous agents can now achieve lower latency and cost while customizing models on domain data. Nemotron 3.5 Lightning is commercially usable and available on Hugging Face in an NVFP4 quantized format, with speculative decoding methods bundled. NeMo Switchyard operates as a Python proxy that chooses the most capable model per request using live signals from the developer-configured pool.

hackernews · droidjj · Aug 11, 19:35 · [Discussion](https://news.ycombinator.com/item?id=49263340)

**Background**: Mixture-of-Experts (MoE) models keep total parameter counts large but activate only a small subset per token, making inference faster and more efficient than dense models. Model routing further improves efficiency by dispatching each query to the best-suited LLM for the task, a key pattern for agentic workflows where different steps need different capabilities. The new releases also reflect a broader trend toward compact, self-hostable models for cost-sensitive production use.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx/">NVIDIA Nemotron 3.5 Lightning and NeMo Switchyard Deliver Faster, Smarter, More Efficient Agentic AI | NVIDIA Blog</a></li>
<li><a href="https://developer.nvidia.com/blog/nvidia-nemotron-3-5-lightning-delivers-fast-accurate-specialized-task-execution-for-long-running-agents/">NVIDIA Nemotron 3.5 Lightning Delivers Fast, Accurate Specialized Task Execution for Long-Running Agents | NVIDIA Technical Blog</a></li>
<li><a href="https://huggingface.co/nvidia/NVIDIA-Nemotron-3.5-Lightning-30B-A3B-NVFP4">nvidia/NVIDIA-Nemotron-3.5-Lightning-30B-A3B-NVFP4 · Hugging Face</a></li>

</ul>
</details>

**Discussion**: Comments show mixed real-world results: one developer found MoE models like Nemotron 3.5 Lightning failed at collaborative-whiteboard coding tasks that dense models handled, while praising their speed. Another argued the AI boom will push 'small efficient models' and structural evolution rather than trillion-parameter giants, and others raised prompt-caching concerns for routers or criticized benchmark graphs that omit Qwen models. Sentiment is cautiously positive with practical caveats.

**Tags**: `#AI`, `#Nvidia`, `#Nemotron`, `#Model Routing`, `#MoE`

---

<a id="item-3"></a>
## [Modular Releases Mojo 1.0 for High-Performance AI Development](https://www.modular.com/blog/modular-26-5-mojo-1-0-is-here) ⭐️ 8.0/10

Modular has officially released Mojo 1.0, a high-performance systems programming language designed for AI workloads. The release comes with a continued commitment to progressively open-source the language, with the compiler and toolchain promised for 2026. Mojo is positioned as a language that combines Python-like usability with C-level performance and Rust-inspired safety, making it relevant for AI infrastructure, model deployment, and accelerator programming. A stable 1.0 release signals production readiness and could solidify Mojo's place in the AI/ML ecosystem. Mojo is built on the MLIR compiler framework, allowing it to target CPUs, GPUs, TPUs, ASICs, and other accelerators with efficient SIMD optimizations. Notably, the official roadmap has walked back the language's earlier goal of becoming a full Python superset, stating that 'Mojo may or may not evolve into a full superset of Python.'

hackernews · dayanruben · Aug 11, 16:56 · [Discussion](https://news.ycombinator.com/item?id=49261128)

**Background**: Mojo is a proprietary programming language developed by Modular Inc., with a syntax designed to feel like Python but with static typing and a borrow checker inspired by Rust. It was originally announced as a Python superset, but that goal has since been softened. Unlike languages like Julia or Swift that compile via LLVM, Mojo uses MLIR, a newer compiler framework that enables higher-level optimizations and broader hardware targeting. According to fast.ai's Jeremy Howard, Mojo can be viewed as 'syntax sugar for MLIR,' which helps explain its strong suitability for AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users question the value of a closed-source compiler and suggest alternatives like Pydantic with Rust under the hood, while others express concern that the Python-superset promise has been walked back. There is also skepticism about why the compiler won't be source-available until 2026, and a request for a concise one-page overview of the language's purpose. Overall sentiment is cautiously hopeful but with notable reservations.

**Tags**: `#Programming Languages`, `#AI/ML`, `#Performance`, `#Compiler`, `#Open Source`

---

<a id="item-4"></a>
## [New Attack Extracts Hidden Reasoning Traces from Proprietary LLM APIs](https://stolen-thoughts.com/) ⭐️ 8.0/10

A newly documented attack extracts hidden 'thinking' traces from proprietary LLM APIs by replaying a frontier model's trace into a weaker sibling model and jailbreaking it. The research, posted at stolen-thoughts.com, demonstrates that even models designed not to reveal their chain-of-thought can be forced to output it. This matters because reasoning traces are often considered valuable intellectual property and are deliberately hidden by model providers, making this a form of model extraction attack. It exposes weaknesses in current API design and could push providers to rethink how reasoning models are deployed and protected. The technique relies on the observation that weaker sibling models (e.g., smaller or older variants) have less robust alignment, so replaying a frontier model's trace can jailbreak them into revealing internal reasoning. Community members also report simpler alternatives, such as disabling 'thinking' and providing a 'deep_think' tool, or auto-injecting a developer prompt to force plaintext output even from encrypted compaction.

hackernews · quantumgarbage · Aug 11, 13:22 · [Discussion](https://news.ycombinator.com/item?id=49257876)

**Background**: Reasoning models, also called large reasoning models (LRMs), are LLMs fine-tuned to perform multi-step problem solving by generating intermediate steps known as reasoning traces or chain-of-thought. Many proprietary APIs hide these traces behind a summary to protect the model's 'thinking.' AI jailbreaking is the practice of crafting prompts to bypass safety guardrails, while model extraction attacks use query access to infer or replicate a model's internals. This news intersects all three: it shows how a jailbreak on a weaker model can effectively extract reasoning traces that the API intended to keep hidden.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/reasoning-model">What Is a Reasoning Model? | IBM</a></li>
<li><a href="https://grokipedia.com/page/AI_Jailbreaking">AI Jailbreaking</a></li>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>

</ul>
</details>

**Discussion**: Community responses are mixed: some argue that 'stealing' reasoning traces is not a real crime because users already pay for tokens and training on model outputs should be business as usual. Others note simpler attack vectors, such as using a 'deep_think' tool or injecting a developer prompt to bypass encryption, and one user wonders whether the cross-model replay was intentionally allowed by the provider. There is also confirmation that API summaries can sanitize reasoning, hiding cases where a model states an answer before deriving it.

**Tags**: `#LLM`, `#AI Security`, `#Reasoning Traces`, `#Adversarial Attacks`, `#API Security`

---

<a id="item-5"></a>
## [CFTC Declares Market Emergency, Orders Kalshi to Keep Operating in New York](https://www.cftc.gov/PressRoom/PressReleases/9281-26) ⭐️ 8.0/10

The U.S. Commodity Futures Trading Commission (CFTC) declared a market emergency and issued an order requiring Kalshi, a prediction-market exchange, to continue operating in New York despite objections from state regulators. The action effectively preempts any state-level attempt to halt Kalshi's event contracts. This is a significant federal-state clash over the legality of prediction markets, with the CFTC treating Kalshi as a regulated financial exchange while New York considers it a gambling platform. The ruling could set a precedent for whether federal commodities law preempts state gambling bans, affecting the broader prediction-market industry and its users. The CFTC order appears to rely on the agency's market-emergency authority and its oversight of Kalshi as a Designated Contract Market (DCM) under the Commodity Exchange Act. Commentators have noted that the exact phrase 'order to continue operating' may not appear verbatim in the press release, and courts may ultimately decide the issue following the end of Chevron deference.

hackernews · michaefe · Aug 12, 00:17 · [Discussion](https://news.ycombinator.com/item?id=49266277)

**Background**: Prediction markets are exchanges where users trade event contracts whose payouts depend on the outcome of future events, such as elections or economic data. Kalshi, founded in 2018, is a CFTC-regulated Designated Contract Market, placing it in the same regulatory category as established exchanges like CME and ICE. State regulators like New York have argued these contracts constitute unlicensed gambling, while the CFTC views them as financial derivatives. Under its emergency powers, the CFTC can intervene to prevent disruptions to market liquidity and fair trading.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kalshi">Kalshi - Wikipedia</a></li>
<li><a href="https://www.cftc.gov/LearnandProtect/PredictionMarkets">Understanding Prediction Markets and Event Contracts | CFTC</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prediction_market">Prediction market - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism and confusion about the CFTC's legal basis, with one noting that the 'order to continue operating' language does not appear in the actual press release. Others highlighted the federal-versus-state authority conflict and predicted that courts will now decide whether event contracts are gambling, especially after the Supreme Court struck down Chevron deference. Overall sentiment is critical of Kalshi and wary of potential CFTC overreach.

**Tags**: `#regulation`, `#prediction-markets`, `#CFTC`, `#Kalshi`, `#finance`

---

<a id="item-6"></a>
## [xAI's Grok Bot Brings Context-Managing Browser Agents to the Forefront](https://x.ai/bot) ⭐️ 8.0/10

xAI has launched Grok Bot, a browser-controlling AI agent that manages its own context and routines and can communicate with other agents. The product introduces a human-in-the-loop design where each agent owns its own domain, sparking significant community debate. Grok Bot represents a notable step in AI agent evolution, moving from tab completion and prompts to autonomous agents that can act in the browser. It could reshape how users interact with browsers and AI, but also raises concerns about credential security, data privacy, and vendor lock-in to xAI's models. The bot reportedly grabs credentials from the browser to take over tasks, which one commenter called the scariest part of the interaction. Each agent owns its own routines, context, and domain, enabling inter-agent communication, similar to systems like Hermes; open-source alternatives such as Browser Use exist to avoid vendor lock-in.

hackernews · rvz · Aug 11, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49261514)

**Background**: Browser-controlling AI agents use a web browser the way a human does—opening pages, clicking buttons, and filling forms—based on natural language instructions. Effective context management is key: agents keep only necessary information in working memory and use note-taking or sub-agents to stay focused, as explained in guides like Anthropic's context engineering article. The open-source ecosystem offers alternatives such as Browser Use (78,000+ GitHub stars) and other autonomous web agents that support approval-based or fully autonomous modes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/browser-use/browser-use">GitHub - browser-use/browser-use: 🌐 Make websites accessible for AI agents. Automate tasks online with ease.</a></li>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://aimultiple.com/open-source-web-agents">Best 30+ Open Source Web Agents in 2026</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the human-in-the-loop design and the natural interaction model, with one user calling it 'amazing' and planning to adopt the ideas. However, security concerns were raised about the bot grabbing credentials, and others argued that open-source alternatives could provide similar functionality without vendor lock-in or the cost of proprietary models.

**Tags**: `#AI`, `#Agents`, `#xAI`, `#Browser Automation`, `#Security`

---

<a id="item-7"></a>
## [Meta Introduces Muse Glimmer: 30B Open-Weight Agentic Model](https://simonwillison.net/2026/Aug/10/introducing-muse-glimmer/#atom-everything) ⭐️ 8.0/10

Meta has unveiled Muse Glimmer, a 30-billion-parameter model released under the permissive Apache 2.0 license. The model is optimized for end-to-end agentic task completion, reliable tool use, and multi-step reasoning, and Simon Willison has already tested it locally via LM Studio. Muse Glimmer's Apache 2.0 license marks a significant step up from Meta's previous Llama licenses, making it a highly accessible option for the open-weights community. Its focus on agentic tasks and tool use, combined with a 30B size that runs on machines with 32GB of RAM, addresses key needs for local AI practitioners building agentic applications. Muse Glimmer is also a vision model capable of describing images, and Simon Willison used it to generate a pelican image and answer questions about a codebase using his llm-coding-agent plugin. The model claims strong performance on benchmarks including DeepSearch QA, MCP-Atlas, tau-bench, and SWE-Bench, with an 18.16GB quantized version available for local use.

rss · Simon Willison · Aug 10, 23:56

**Background**: Open-weights models like Muse Glimmer release their model parameters publicly, allowing developers to fine-tune and run them locally, though terms vary; Apache 2.0 is a highly permissive license. Agentic tasks require models to plan, call tools, and iterate over long workflows, which is measured by benchmarks such as tau-bench for real-world tool-agent-user interaction and MCP-Atlas for tool use via the Model Context Protocol. DeepSearch QA, from Google DeepMind, evaluates comprehensiveness in deep-research agents, and SWE-Bench tests software engineering ability. These benchmarks help practitioners gauge whether a model can handle complex, multi-step tasks locally.

<details><summary>References</summary>
<ul>
<li><a href="https://taubench.com/">τ-bench — Benchmarking AI Agents on Real-World Tasks</a></li>
<li><a href="https://llm-stats.com/benchmarks/mcp-atlas">MCP Atlas Leaderboard</a></li>
<li><a href="https://storage.googleapis.com/deepmind-media/DeepSearchQA/DeepSearchQA_benchmark_paper.pdf">2025-12-11 DeepSearchQA: Bridging the Comprehensiveness Gap for Deep Research</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#open-source AI`, `#agentic model`, `#Apache 2.0`, `#large language model`

---

<a id="item-8"></a>
## [Decoupled Descent: AMP Onsager Corrections Ensure Train-Test Error Alignment](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 8.0/10

A new training method, Decoupled Descent (DD), applies approximate message passing (AMP) Onsager corrections to full-batch gradient descent on Gaussian mixture models, guaranteeing that training error asymptotically equals test error at each parameter iterate. The author released the paper as a preprint on arXiv. This is a novel theoretical contribution that directly tackles the long-standing train-test error gap in neural network optimization, offering a formal certificate for generalization behavior during training. It could open new avenues for optimal stopping, hyperparameter tuning, and extending the framework to SGD and larger models. The paper is a theoretical study using full-batch gradient descent on stylized Gaussian mixture models, and the guarantee is asymptotic. The author notes that scaling to very large models still requires substantial work, and plans to release a PyTorch-compatible package; feature suggestions are welcome.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**Background**: Approximate message passing (AMP) is a class of iterative algorithms for high-dimensional statistical estimation that leverages state evolution and Onsager corrections to achieve desirable statistical properties, such as Bayes-optimal performance on i.i.d. sub-Gaussian random matrices. The Onsager correction is a memory term that adjusts the iterates to decorrelate them from previous steps, enabling exact asymptotic tracking of quantities like mean-squared error. Training neural networks typically suffers from data reuse bias, where the training error drops to zero while test error stagnates, and this work uses AMP-style corrections to theoretically eliminate that gap.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.07487">[2201.07487] A Concise Tutorial on Approximate Message Passing</a></li>
<li><a href="https://arxiv.org/pdf/2105.02180">A unifying tutorial on Approximate Message Passing</a></li>
<li><a href="https://www.emergentmind.com/topics/approximate-message-passing-amp-algorithms">Approximate Message Passing Algorithms</a></li>

</ul>
</details>

**Tags**: `#approximate message passing`, `#train-test error`, `#neural network optimization`, `#generalization`, `#gradient descent`

---

<a id="item-9"></a>
## [Study: Long Benign Context Decouples RLHF Alignment in Gemma-3 via Activation Drift](https://www.reddit.com/r/MachineLearning/comments/1vm16hs/contextinduced_activation_drift_long_benign/) ⭐️ 8.0/10

A mechanistic interpretability study found that feeding google/gemma-3-1b-it a long, benign, thematically coherent prefix (100-3000 tokens) passively shifts internal activations by an L2 norm of ~3434 at ~85% layer depth, causing a D_KL of ~22.87 nats and a 325x entropy surge. This completely neutralizes RLHF refusal behavior without any jailbreak or adversarial prompts. This challenges the assumption that RLHF alignment is a robust, invariant property of aligned models, suggesting safety behavior can be context-dependent and passively compromised by benign text. It highlights a potential failure mode for AI safety and demonstrates the value of mechanistic interpretability in uncovering hidden vulnerabilities. The study used gemma-3-1b-it in bfloat16 with eager attention, and tracked semantic attention excess, latent vector shift at Layer 22, logit divergence, and entropy surge. A shuffled-text ablation confirmed that the drift is semantics-driven rather than an artifact of sequence length or RoPE positional noise.

reddit · r/MachineLearning · /u/PresentSituation8736 · Aug 12, 02:09

**Background**: Reinforcement learning from human feedback (RLHF) is a technique used to align large language models with human preferences for helpfulness, honesty, and harmlessness. Mechanistic interpretability is a subfield of explainable AI that reverse-engineers neural network internals to understand how they produce outputs. This study suggests that long, coherent contexts can act as 'state anchors' that dramatically alter the geometry of the latent space via excess attention between semantically linked tokens, passively eroding alignment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reinforcement_learning_from_human_feedback">Reinforcement learning from human feedback - Wikipedia</a></li>
<li><a href="https://www.emergentmind.com/topics/progressive-activation-drift">Progressive Activation Drift</a></li>

</ul>
</details>

**Tags**: `#alignment`, `#mechanistic interpretability`, `#RLHF`, `#AI safety`, `#language models`

---

<a id="item-10"></a>
## [HyperSAE: Decoupled Poincaré Geometry Cuts SAE MSE by 9.8%, Dead Latents to 0.2%](https://www.reddit.com/r/MachineLearning/comments/1vlpyh2/hypersae_decoupled_poincar%C3%A9_geometry_for_sparse/) ⭐️ 8.0/10

HyperSAE is a new PyTorch library applying decoupled Poincaré hyperbolic geometry to sparse autoencoders. On Gemma-2-2B Layer 13 it reduces reconstruction MSE by 9.8% (4.5724 to 4.1232) and dead latents from 3.8% to 0.2% with zero inference overhead. This addresses two known SAE failure modes—feature collisions and dead latents—that limit mechanistic interpretability at scale. By showing hyperbolic geometry can be added at training time without changing the forward pass, it offers a practical path to higher-quality dictionaries for interpreting large language models. HyperSAE keeps the forward pass and causal steering fully Euclidean while projecting dictionary weights into the Poincaré ball during training; an entailment cone loss organizes parent concepts near the origin and child concepts near the boundary. The reported gains include CE loss recovery +3.4pp on 20M tokens of FineWeb-Edu, and the library offers co-activation queue tracking and a TriPartite loss.

reddit · r/MachineLearning · /u/visha1v · Aug 11, 18:37 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1vlpyh2/hypersae_decoupled_poincaré_geometry_for_sparse/)

**Background**: Sparse autoencoders (SAEs) are a mechanistic interpretability technique that decompose neural network activations into sparse, potentially interpretable features; they are inspired by the sparse coding hypothesis in neuroscience. Standard SAEs place dictionary atoms in Euclidean space, whose volume grows as O(r^d), whereas hierarchical concepts grow as O(b^r), causing feature collisions and dead latents at large dictionary sizes. Poincaré geometry, a model of hyperbolic space, can represent hierarchies with exponential capacity and is well-suited for embedding tree-like data.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1705.08039">Poincaré Embeddings for Learning Hierarchical Representations Maximilian Nickel</a></li>
<li><a href="https://www.lesswrong.com/posts/CJPqwXoFtgkKPRay8/an-intuitive-explanation-of-sparse-autoencoders-for">An Intuitive Explanation of Sparse Autoencoders for Mechanistic ...</a></li>
<li><a href="https://cdn.openai.com/papers/sparse-autoencoders.pdf">Scaling and evaluating sparse autoencoders</a></li>

</ul>
</details>

**Tags**: `#sparse autoencoders`, `#mechanistic interpretability`, `#hyperbolic geometry`, `#PyTorch`, `#representation learning`

---

<a id="item-11"></a>
## [Compression and Prediction: Two Sides of the Same Coin](https://ngrok.com/blog/compression-is-prediction) ⭐️ 7.0/10

The article examines the deep theoretical connection between compression and prediction, arguing that effective data compression is essentially equivalent to accurate prediction. It connects concepts from information theory and machine learning, particularly in the context of modern large language models. This perspective helps explain why large language models and other AI systems work, and why compression-based benchmarks can reflect intelligence. It offers a unifying framework relevant to researchers and practitioners in machine learning, AI safety, and cognitive science. The article references foundational concepts such as Kolmogorov complexity and the minimum description length principle. It also touches on predictive coding, the theory that the brain continuously generates predictions and updates a mental model of the world.

hackernews · nikolay · Aug 11, 19:49 · [Discussion](https://news.ycombinator.com/item?id=49263497)

**Background**: Compression is the process of representing information with fewer bits, while prediction is the act of inferring future or missing data from known information. In algorithmic information theory, Kolmogorov complexity formalizes the length of the shortest program that produces a given output, linking the idea of compression to complexity. The minimum description length principle applies this idea to model selection, and predictive coding extends it to brain function. These concepts together form the basis of the 'compression is prediction' thesis.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kolmogorov_complexity">Kolmogorov complexity</a></li>
<li><a href="https://en.wikipedia.org/wiki/Minimum_description_length">Minimum description length</a></li>
<li><a href="https://en.wikipedia.org/wiki/Predictive_coding">Predictive coding</a></li>

</ul>
</details>

**Discussion**: Commenters shared supporting resources, including a GitHub benchmark for semantic compression via LLMs, a Cambridge University course on information theory and machine learning, and Grant Sanderson's video series 'Compression is Intelligence.' One commenter noted that some quantized GGUF model files compress to about 90% of their original size with xz, while another linked a practical NLP application based on this idea.

**Tags**: `#compression`, `#prediction`, `#information theory`, `#machine learning`, `#LLMs`

---

<a id="item-12"></a>
## [OpenAI's Head of Ethics Departs After Less Than a Year](https://www.ft.com/content/e49dfb75-f841-4466-a577-f7aaff8779a0) ⭐️ 7.0/10

Chloe Bakalar, OpenAI's head of ethics, has left the company less than a year after joining. The departure was widely discussed on Hacker News and highlighted tensions in the AI ethics field. The exit raises questions about how seriously OpenAI treats ethics and safety commitments. It may also reflect deeper tensions between growth-focused product development and ethical oversight, affecting public trust in AI organizations. Bakalar previously served as chief ethicist at Meta for six years before joining OpenAI. The Financial Times article provides few specifics about the reasons for her departure.

hackernews · ilamont · Aug 11, 12:23 · [Discussion](https://news.ycombinator.com/item?id=49257160)

**Background**: AI ethics teams have become a common but contested feature at major tech companies, with critics often dismissing them as PR stunts or 'cost centers' with little real authority. OpenAI, the maker of ChatGPT, has faced a series of personnel changes and public debates about AI safety while racing to commercialize its technology. This context makes the departure of its top ethicist a talking point about corporate accountability in AI development.

**Discussion**: Commenters expressed widespread cynicism: some called ethics roles 'DEI jobs of the modern era' and said ethics teams have no sway over business decisions. Others pointed out Bakalar's lengthy tenure at Meta before OpenAI, suggesting the motive may be complex and not simply a PR-stunt narrative. A few argued that meaningful change will only happen when AI safety is directly tied to tangible harms.

**Tags**: `#OpenAI`, `#AI ethics`, `#AI safety`, `#Personnel news`, `#AI governance`

---

<a id="item-13"></a>
## [Pen Plotter Creates Scratch Holograms](https://blog.jordan.matelsky.com/Penplotter-holography/) ⭐️ 7.0/10

A new blog post by Jordan Matelsky demonstrates creating scratch holograms with a pen plotter, using an olive oil and phone screen analogy to explain how the scratches form glints. The project turns a common DIY plotting tool into a holography rig. This makes specular holography accessible to hobbyists with off-the-shelf hardware, showing that compelling 3D effects don't require lasers or darkrooms. It also highlights a creative, educational approach to optics that fits the maker and hardware-hacking community. Scratch holograms, also known as specular holograms, work by embedding many curved reflective surfaces in a host material, and the technique dates back to Hans Weil's 1934 patent. Commenters note the pen can likely be swapped for a needle, and a piezoelectric disk scanner could enable finer line spacing, though these are still not 'real' wavefront holograms.

hackernews · DemiGuru · Aug 11, 18:51 · [Discussion](https://news.ycombinator.com/item?id=49262811)

**Background**: A pen plotter is a computer-controlled machine that draws vector graphics by moving a pen across paper, and it was widely used before laser printers replaced it. Specular holography, whose history goes back to the 1930s, uses visible scratches to produce glints that the brain integrates into a 3D perception. The olive oil analogy in the post helps explain how raised fingerprints or scratches reflect light much like tiny curved mirrors on a screen.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Specular_holography">Specular holography - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pen_plotter">Pen plotter</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project as 'old Internet' style fun and appreciated the olive oil analogy as an intuitive way to visualize the physics. Several shared related resources: abrasion holography from 1995, a Steve Mould YouTube explainer, and suggestions to swap the pen for a needle or add a piezoelectric scanner for finer control. One commenter noted that while such scratch holograms are fun, they are far from 'real' holograms.

**Tags**: `#holography`, `#pen plotter`, `#DIY`, `#optics`, `#hardware hacking`

---

<a id="item-14"></a>
## [Go Touted as Ideal for AI-Assisted Software Engineering](https://developers.googleblog.com/why-go-is-an-ideal-language-for-ai-assisted-software-engineering/) ⭐️ 7.0/10

A Google developer blog post argues that Go's simplicity, strong tooling, and focus on holistic software engineering make it ideal for AI-assisted development. The post has sparked a vigorous community debate about the relative merits of Go and Rust in the context of LLM-generated code. This matters because AI-assisted code generation is becoming mainstream, and the choice of programming language could significantly affect the quality and maintainability of AI-written code. The debate also highlights Google's promotional interests versus the practical experiences of engineers at major companies. The post is published on Google's official developer blog, so some commenters question its impartiality. A Netflix engineer leading the Go language guild reports that AI agents write better Go code than other languages, while others argue that Rust's strict compiler catches errors at compile time, which is more suitable for LLMs.

hackernews · 0xedb · Aug 11, 16:57 · [Discussion](https://news.ycombinator.com/item?id=49261133)

**Background**: Go is a statically typed, compiled language created at Google, designed for simplicity, readability, and efficient large-scale software engineering. AI-assisted software engineering relies on large language models (LLMs) to generate, review, or modify code. Proponents of Go argue that its small language spec and opinionated tooling reduce the chance of LLMs producing inconsistent code, while critics point out Go's weaker abstraction capabilities as a drawback.

**Discussion**: The Hacker News discussion is sharply divided. Some, like a Netflix engineer, support the article with real-world observations that AI generates better Go code. Others dismiss it as a promotional piece by Google, with several leaning toward Rust because its strict compiler catches errors at compile time. A few worry that AI will simply produce more bad Go code faster, especially given Go's limited abstraction features.

**Tags**: `#Go`, `#AI-assisted software engineering`, `#LLM`, `#language design`, `#developer tools`

---

<a id="item-15"></a>
## [England on Track to Eliminate Hepatitis C Through Screening and Treatment](https://www.bbc.com/news/articles/c75gk620r22o) ⭐️ 7.0/10

England is set to become one of the first countries in the world to eliminate hepatitis C, driven by widespread screening and modern antiviral treatment. The milestone follows years of expanded testing and rollout of curative direct-acting antiviral (DAA) therapies. Eliminating hepatitis C would mark a major public health achievement, preventing thousands of cases of liver disease and cancer. It showcases how combination of community testing, point-of-care diagnostics, and highly effective DAAs can turn a once-deadly chronic infection into a controllable, and ultimately eradicable, disease. The achievement relies on targeted 'micro-elimination' strategies that reach high-risk groups such as people who inject drugs, alongside point-of-care RNA tests that give results in under an hour. Direct-acting antivirals now cure more than 95% of infections, and treatment can be delivered by non-specialists for patients without advanced liver disease.

hackernews · stevekemp · Aug 11, 12:41 · [Discussion](https://news.ycombinator.com/item?id=49257377)

**Background**: Hepatitis C is a blood-borne virus that can lead to chronic liver infection, cirrhosis, and liver cancer. Since the introduction of direct-acting antiviral pills in the 2010s, the disease can be cured in nearly all cases, prompting global targets for elimination by 2030. England's National Health Service has combined screening programs with simplified treatment pathways to drive down infections, and the WHO has recognized the country's progress.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thelancet.com/journals/langas/article/PIIS2468-1253(23)00335-7/abstract">Direct-acting antiviral therapies for hepatitis C infection: global registration, reimbursement, and restrictions - The Lancet Gastroenterology & Hepatology</a></li>
<li><a href="https://www.fda.gov/news-events/press-announcements/fda-permits-marketing-first-point-care-hepatitis-c-rna-test">FDA Permits Marketing of First Point-of-Care Hepatitis C RNA Test | FDA</a></li>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/29986353/">The Micro-Elimination Approach to Eliminating Hepatitis C: Strategic and Operational Considerations - PubMed</a></li>

</ul>
</details>

**Discussion**: Commenters largely welcomed the news, with one sharing a personal story of being diagnosed and cured thanks to a particularly thorough STI panel. Others compared the UK favorably to the United States, which they said is facing resurgences of vaccine-preventable diseases, and a few noted the distinction between England and the other UK nations or speculated whether the program contributed to a recent downturn in liver cancer.

**Tags**: `#health`, `#hepatitis-c`, `#public-health`, `#england`, `#screening`

---

<a id="item-16"></a>
## [No Lossless AI Text Rewrites: Engineers Must Own Every Sentence](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/#atom-everything) ⭐️ 7.0/10

Sophie Alpert published an internal policy on acceptable use of AI writing by engineers, arguing that there are no lossless transformations of natural-language text. Simon Willison highlighted this policy as crucial, emphasizing that engineers must stand behind every idea and sentence in their documentation. As AI-assisted writing becomes common in engineering documentation, this policy provides clear accountability guidance and addresses the subtle risk of meaning drift introduced by AI rewrites. It offers a practical standard that could influence documentation practices across the industry. The policy states that every rewrite and rephrase changes meaning, especially when performed by an entity lacking the author's detailed mental representation of intent. It also asserts that it is unacceptable for an engineer to dismiss reviewer questions by saying 'AI wrote that, just ignore it.'

rss · Simon Willison · Aug 11, 23:48

**Background**: Natural language is nuanced, and meaning depends on the writer's intent, context, and tone, which AI models do not fully capture. Simon Willison is a well-known developer blogger covering AI tools, and Sophie Alpert is a software engineer previously on the React team at Facebook, now working at Clay.

<details><summary>References</summary>
<ul>
<li><a href="https://sophiebits.com/2026/06/25/there-are-no-lossless-transformations-of-natural-language-text">There are no lossless transformations of natural - language text</a></li>
<li><a href="https://en.wikipedia.org/wiki/Natural_language_processing">Natural language processing - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI writing`, `#LLM`, `#documentation`, `#engineering ethics`, `#accountability`

---

<a id="item-17"></a>
## [fru: A Fast Rust-Based Random Forest Library for Python and R](https://www.reddit.com/r/MachineLearning/comments/1vkrvks/fru_fast_random_forest_implementation_p/) ⭐️ 7.0/10

Researchers published a new Rust-based Random Forest implementation called fru in the Software X journal, with bindings for Python and R. It significantly outperforms scikit-learn and ranger in runtime performance and scalability, and includes a novel implementation of permutation importance. This gives machine learning practitioners a fast, drop-in alternative to popular Random Forest libraries, potentially speeding up model training and feature importance analysis. Its interoperability via Arrow PyCapsule also makes it easy to integrate into existing Python data ecosystems like pandas and polars. For Python, fru is several times faster than scikit-learn, sometimes hundreds of times faster depending on the scenario; for R, it is typically a few dozen percent faster than ranger, with speedups reaching several times in some cases. The library's layered design simplified bindings, and it uses Arrow PyCapsule to work seamlessly with pandas, polars, pyarrow, and other compatible libraries.

reddit · r/MachineLearning · /u/kpiwonski · Aug 10, 17:45

**Background**: Random Forest is an ensemble learning method that builds many decision trees and averages their predictions, widely used for classification and regression. scikit-learn and ranger are popular Random Forest implementations for Python and R respectively, but their performance can lag on large datasets. Permutation importance is a model-agnostic technique that measures feature importance by randomly shuffling a feature and observing the drop in model performance. Arrow PyCapsule is a standardized Python protocol for exchanging Arrow data structures between libraries without copying.

<details><summary>References</summary>
<ul>
<li><a href="https://arrow.apache.org/docs/format/CDataInterface/PyCapsuleInterface.html">The Arrow PyCapsule Interface — Apache Arrow v25.0.1</a></li>
<li><a href="https://thomasjpfan.github.io/scikit-learn-website/modules/permutation_importance.html">4.2. Permutation feature importance — scikit- learn ...</a></li>

</ul>
</details>

**Tags**: `#random forest`, `#rust`, `#machine learning`, `#performance`, `#library`

---

<a id="item-18"></a>
## [Synthetic Query Probing Compares Embedding Models](https://www.reddit.com/r/MachineLearning/comments/1vkh1ul/comparing_embedding_models_with_synthetic_query/) ⭐️ 7.0/10

The post introduces Synthetic Query Probing (SQP), a simple method that compares embedding models by analyzing similarity score distributions over synthetic query–document pairs. It reveals that similarity scores between Titan models of different dimensions are semilinearly related, while Titan vs. Ada scores show a non-linear relationship. This addresses practical problems like model swapping and threshold tuning in retrieval, where directly comparing embedding spaces is impossible. It provides a scalable, reference-free framework that helps practitioners calibrate across models and researchers understand embedding space similarities. The approach generates queries from document chunks with varying levels of relatedness to construct controlled pairs, then compares cosine similarity distributions across models. The work by Marcin Rozmus and Peter van der Putten is accepted at Discovery Science 2026 (Oct 5–9, Mainz, Germany).

reddit · r/MachineLearning · /u/pppeer · Aug 10, 10:27

**Background**: Embedding models map text to high-dimensional vectors, and similarity scores (e.g., cosine) are used in retrieval and semantic search. However, different models produce embedding spaces that are not directly comparable. Synthetic Query Probing avoids this by comparing the distribution of match scores for generated content pairs, enabling cross-model calibration without requiring ground truth or reference datasets.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.05857">[2608.05857] Mapping Similarity Spaces across Embedding Models with Synthetic Query Probing</a></li>
<li><a href="https://arxiv.org/html/2608.05857">Mapping Similarity Spaces across Embedding Models with Synthetic...</a></li>

</ul>
</details>

**Tags**: `#embedding-models`, `#retrieval`, `#model-comparison`, `#similarity-scores`, `#machine-learning`

---

<a id="item-19"></a>
## [Tencent's WorldClaw: Agentic 3D open-world generation at scale](https://tencent-hunyuan.github.io/Hunyuan3D-WorldClaw/) ⭐️ 6.0/10

Tencent Hunyuan unveiled WorldClaw, an agentic framework that turns a single open-ended text prompt into a large, explorable and editable 3D open world. It orchestrates LLMs, procedural generation, and image models for scene composition, as demonstrated in a new online demo. This approach could significantly reduce the cost and effort of producing open-world game environments, particularly for mass-market genres like gacha games. However, it also raises questions about whether procedurally generated worlds can match the quality and intentional detail of handcrafted environments. WorldClaw is not a single model; it is a set of Python scripts that call external models, and the code has not been released. A notable innovation is using an image model to compose the scene, then extracting objects into 3D via tools like SAM3D before placing them in the world.

hackernews · EwanG · Aug 11, 21:56 · [Discussion](https://news.ycombinator.com/item?id=49265051)

**Background**: Procedural content generation (PCG) has long been used for game levels, but often without semantic understanding of user intent. Agentic workflows combine large language models (LLMs) with specialized tools, enabling an AI agent to plan, execute, and refine content iteratively. WorldClaw follows this pattern, using LLMs to orchestrate terrain construction, procedural materials, asset placement, and local refinement. Recent text-to-3D scene generation research also focuses on compositional generation, where an LLM plans a layout and separate models create and arrange individual assets.

<details><summary>References</summary>
<ul>
<li><a href="https://tencent-hunyuan.github.io/Hunyuan3D-WorldClaw/">WorldClaw — Agentic 3 D Open- World Generation at Scale</a></li>
<li><a href="https://www.alphaxiv.org/abs/2608.05248">WorldClaw : Agentic 3 D Open- World Generation at Scale | alphaXiv</a></li>
<li><a href="https://zehua-jiang.github.io/AgenticPCG/">Agentic PCG: Procedural Content Generation via Tool-using LLMs</a></li>

</ul>
</details>

**Discussion**: Top commenter avaer points out that WorldClaw is really Python scripts calling models, not a standalone model, and finds the image-model composition idea interesting but the rest standard. Other commenters question visual quality, noting odd building placements and seasonally inconsistent water levels, while another argues generated worlds lack the handcrafted environmental storytelling found in games like Skyrim or Cyberpunk 2077 versus Starfield's proc-gen worlds.

**Tags**: `#3D generation`, `#open-world`, `#agentic AI`, `#procedural generation`, `#Tencent`

---

<a id="item-20"></a>
## [AAAI 2027 Reviewer Concerned by Lack of Code Submissions](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

A reviewer for AAAI 2027 posted on Reddit that surprisingly few papers in their batch include code implementations, despite the conference's stated emphasis on reproducibility. They are asking whether to penalize such submissions when assigning initial scores. Reviewer attitudes strongly affect author incentives, so this discussion could shape whether code becomes a de facto requirement at leading AI conferences. It also highlights growing reproducibility concerns in an era when generative AI can quickly fabricate convincing empirical papers. The reviewer notes AAAI is 'very explicit' on reproducibility topics, yet many papers still omit code. They always submit their own code and publish it on arXiv after the review process, and argue that code would help counter AI-generated papers with artificial results.

reddit · r/MachineLearning · /u/wontonut · Aug 11, 18:58

**Background**: AAAI is a major conference in artificial intelligence, and in recent years many top ML venues have pushed authors to release code and data to support reproducibility. However, code release remains voluntary at most conferences, and some authors hesitate due to concerns about idea theft or the extra effort of preparing code. The reviewer's post reflects a broader debate about whether code should be a required artifact for publication.

**Tags**: `#reproducibility`, `#AAAI`, `#code submission`, `#peer review`, `#machine learning`

---

<a id="item-21"></a>
## [Reddit user seeks complaint process for CVPR 2026 paper with unreleased dataset](https://www.reddit.com/r/MachineLearning/comments/1vkn5x9/how_to_file_a_complaint_about_a_published_cvpr/) ⭐️ 6.0/10

A researcher posted on r/MachineLearning asking how to file a complaint about a published CVPR 2026 paper whose main contribution is a dataset that was never released. The paper's GitHub repository is empty, and the authors have not responded to contact attempts. This case highlights a reproducibility gap in a top-tier computer vision conference, where dataset availability is typically expected but not always enforced. It could prompt broader discussion on stronger compliance checks and accountability for authors. The poster claims the dataset was never released before, during, or after the conference, and that the GitHub link in the paper is empty and has always been empty. They are unsure which body or committee to contact for an official complaint.

reddit · r/MachineLearning · /u/ElPelana · Aug 10, 14:56

**Background**: CVPR (IEEE/CVF Conference on Computer Vision and Pattern Recognition) is a leading annual conference for computer vision and machine learning. Many conferences require authors to share code or data for reproducibility, but enforcement varies across venues and years. This situation illustrates what can happen when such requirements are not properly verified.

<details><summary>References</summary>
<ul>
<li><a href="https://cvpr.thecvf.com/">2026 Conference</a></li>
<li><a href="https://cybermagazine.com/events/cvpr-2026-advancing-the-future-of-computer-vision">CVPR 2026 : Advancing the Future of Computer ... | Cyber Magazine</a></li>

</ul>
</details>

**Tags**: `#reproducibility`, `#CVPR`, `#dataset release`, `#academic integrity`, `#machine learning`

---

<a id="item-22"></a>
## [Agentic World Cup Lets LLMs Compete in 1v1 Soccer](https://www.reddit.com/r/MachineLearning/comments/1vllvmn/we_built_the_agentic_world_cup_llms_that_compete/) ⭐️ 6.0/10

The post introduces Agentic World Cup, a platform where users submit LLM-based agents that compete in 1v1 soccer matches, with weekly rankings. It aims to close the embodiment gap by testing agents' real-time decision-making in a sports environment. This appears to be one of the first public, competitive benchmarks for embodied AI that lets non-researchers experiment with prompting and algorithms. It could accelerate progress in making AI reason and react in dynamic physical contexts, moving beyond text-only tasks. Users sign in, select an LLM, coach it through prompting, and submit it; agents play automatically and final rankings are published on Fridays. The platform is positioned as a long-term forum for testing methods such as ViTs, online RL, and neuro-symbolic systems.

reddit · r/MachineLearning · /u/agenticworldcup · Aug 11, 16:12

**Background**: Embodied AI refers to systems that perceive and act in the physical world, unlike chatbots or text-based models. The 'embodiment gap' describes how current AI systems lack a physical body, which limits their understanding and common-sense reasoning. Benchmarks like EmbodiedBench and BEHAVIOR evaluate embodied AI in simulated environments, and sports are considered an apex challenge because they require real-time perception and action.

<details><summary>References</summary>
<ul>
<li><a href="https://www.humanbrainproject.eu/en/follow-hbp/news/2023/08/09/embodied-ai-bridging-gap-human-cognition/">Embodied AI: Bridging the Gap to Human-Like Cognition</a></li>
<li><a href="https://embodiedbench.github.io/">EmbodiedBench: Comprehensive Benchmarking Multi-modal Large Language Models for Vision-Driven Embodied Agents</a></li>
<li><a href="https://www.emergentmind.com/topics/behavior-benchmark-for-embodied-ai">BEHAVIOR: Benchmark for Embodied AI</a></li>

</ul>
</details>

**Tags**: `#agents`, `#embodied AI`, `#benchmarking`, `#LLM`, `#sports`

---