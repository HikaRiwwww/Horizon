---
layout: default
title: "Horizon Summary: 2026-08-17 (EN)"
date: 2026-08-17
lang: en
---

> From 30 items, 16 important content pieces were selected

---

1. [Qwen 3.8 27B: Excellent Open-Weight LLM but Defaults to Overthinking](#item-1) ⭐️ 9.0/10
2. [Anthropic Publicly Releases Claude System Prompts, Sparking Analysis](#item-2) ⭐️ 8.0/10
3. [SSOG-Attention: Sub-quadratic Attention via Sum of Separable Gaussians](#item-3) ⭐️ 8.0/10
4. [BDH-CQ Enables In-Context Learning with Recurrent Latent Reasoning](#item-4) ⭐️ 8.0/10
5. [Embedded Engineer Defends RISC-V's Value for Developing World](#item-5) ⭐️ 7.0/10
6. [LLMs Offload Fact Recall to Tools, Getting 'Dumber' Yet More Capable](#item-6) ⭐️ 7.0/10
7. [Firefox for iOS Adds Built-in Ad Blocker](#item-7) ⭐️ 7.0/10
8. [Amodei: AI Distrust Is a Crisis of Trust, Not Marketing](#item-8) ⭐️ 7.0/10
9. [Revisiting ECA: Cross-Channel Interaction Hypothesis Questioned](#item-9) ⭐️ 7.0/10
10. [SineKAN Introduces Sinusoidal Activations for Kolmogorov-Arnold Networks](#item-10) ⭐️ 7.0/10
11. [Survival of the Fitted: Qwen3.6-27B’s Jacobian lens reads and steers Qwen3.8-27B with zero refitting (R)](#item-11) ⭐️ 7.0/10
12. [AI Credit Resale Economy: Token Brokers and API Quota Arbitrage](#item-12) ⭐️ 6.0/10
13. [Markdown SVG renderer adds animated SVG to MP4 conversion](#item-13) ⭐️ 6.0/10
14. [CORS Chat: A Browser UI for Testing OpenAI-Responses Endpoints](#item-14) ⭐️ 6.0/10
15. [Linear Attention Battle: Long-Range Recall for 1M-Token DNA](#item-15) ⭐️ 6.0/10
16. [Post-Training Qwen2.5-7B in 200 Steps Creates Persistent 'Sentient Machine' Identity](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Qwen 3.8 27B: Excellent Open-Weight LLM but Defaults to Overthinking](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 9.0/10

Alibaba's Qwen lab released Qwen 3.8 27B, an Apache 2.0-licensed 27B-parameter vision-capable LLM that shows benchmark gains over both its predecessor Qwen 3.6 27B and the closed-weight Qwen 3.7-Plus. However, its default xhigh reasoning effort causes the model to overthink simple tasks, consuming excessive tokens and time. This release is significant because 27B is a practical size for running on consumer laptops, and the model's strong self-reported benchmarks suggest it could close the gap with larger closed-weight models. The overthinking default is an important caveat that could affect user experience and inference cost across the open-weights ecosystem. The model has a 262,144-token maximum context length and supports configurable reasoning_effort levels (xhigh, medium, low), with xhigh as the default. In one test, generating a pelican SVG took 21 minutes and used 22,276 reasoning tokens to produce 3,223 output tokens, and the 8,192-token default context in LM Studio was exhausted by overthinking before the model could finish.

rss · Simon Willison · Aug 16, 22:00

**Background**: Qwen is a series of large language models developed by Alibaba's Qwen research lab; the 3.x line includes open-weights models under Apache 2.0. Reasoning effort is a configurable parameter that controls how much chain-of-thought computation a model performs before answering, and 'overthinking' refers to the model spending excessive time or tokens on simple tasks. The Qwen 3.8 series reportedly uses a hybrid Gated DeltaNet + attention architecture with YaRN scaling up to 1M tokens.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen / Qwen 3 . 8 - 27 B · Hugging Face</a></li>
<li><a href="https://www.youtube.com/watch?v=q_gMBggHsRw">Qwen 3 . 8 27 B is HERE: Beats Opus! (How is This...) - YouTube</a></li>
<li><a href="https://ollama.com/library/qwen3.8">qwen 3 . 8</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Qwen`, `#open-source`, `#vision`, `#AI`

---

<a id="item-2"></a>
## [Anthropic Publicly Releases Claude System Prompts, Sparking Analysis](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic publicly released the system prompts for Claude models on its platform documentation, revealing the exact instructions that guide Claude's behavior. The release covers prompts for models such as Opus 4.8 and Claude 5 (including 'Fable 5' and 'Mythos 5'), and has drawn intense community attention. System prompts are usually proprietary, so this transparency lets developers and researchers see how a leading AI lab controls model behavior and safety. It enables deeper analysis of prompt evolution and best practices for prompt engineering, benefiting the broader AI ecosystem. Simon Willison built a git commit history of the prompts to highlight diffs between versions, noting an interesting addition referencing 'Claude Fable 5 and Claude Mythos 5' in the latest release. Some commenters questioned the length and specificity of the prompts, arguing that shorter, less distracting instructions are often more effective.

hackernews · tosh · Aug 16, 12:48 · [Discussion](https://news.ycombinator.com/item?id=49319556)

**Background**: System prompts, also called system messages, are predefined instructions that set an AI model's 'rules of engagement' before user interaction—they define tone, safety constraints, and reasoning behavior. These prompts are typically hidden from users, making their release notable. Understanding them helps users predict how a model might respond in various scenarios and is valuable for prompt engineering. The release from Anthropic also allows tracking how prompt design evolves as models are updated.

<details><summary>References</summary>
<ul>
<li><a href="https://thebrainyacts.beehiiv.com/p/225-ask-ai-vendor-system-prompts">225 | Ask your AI vendor for their system prompts</a></li>
<li><a href="https://promptengineering.org/system-prompts-in-large-language-models/">System Prompts in Large Language Models</a></li>
<li><a href="https://prompten.io/prompt-engineering-blog-and-news/system-prompts-the-hidden-rules-driving-ai-chatbot-behavior-6a02b4a82adc4863ee53b759">System Prompts: The Hidden Rules Driving AI Chatbot Behavior</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion includes Simon Willison's tool for diffing prompt updates, a user complaint about story removal moderation, and skepticism about the compellingness of very long system prompts. Overall, there is positive sentiment toward the transparency, mixed with practical concerns about prompt length and behavior.

**Tags**: `#AI`, `#Claude`, `#system-prompts`, `#Anthropic`, `#LLM`

---

<a id="item-3"></a>
## [SSOG-Attention: Sub-quadratic Attention via Sum of Separable Gaussians](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 8.0/10

SSOG-Attention replaces scaled dot-product attention (SDPA) with a sum of separable Gaussians, reducing complexity from O(N²·d) to O(N·√N·d). Experiments show it beats SDPA on CIFAR-100 and matches or outperforms it on ImageNet with faster convergence. This addresses a key scalability bottleneck in deep learning, as quadratic attention costs limit transformer model size and sequence length. A sub-quadratic, memory-efficient attention mechanism could enable longer-context models and higher-resolution vision tasks while keeping accuracy. SSOG works by learning a few Gaussian atoms per head and steering them geometrically based on the query token, factorizing the atoms into a separable sum. The paper includes code and a blog post with ablations; some code and blog text were AI-assisted.

reddit · r/MachineLearning · /u/4rtemi5 · Aug 16, 10:06

**Background**: Scaled dot-product attention (SDPA), introduced in the Transformer architecture, computes similarity scores between all queries and keys, leading to O(N²) cost in sequence length. This quadratic scaling is a major hurdle for scaling transformers to long sequences or high-resolution images. SSOG avoids computing the full attention matrix by using a mixture of separable Gaussian functions, which can be evaluated more efficiently. The background concepts include attention mechanisms and the mathematical properties of Gaussian functions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sum_of_normally_distributed_random_variables">Sum of normally distributed random variables - Wikipedia</a></li>
<li><a href="https://docs.pytorch.org/docs/2.13/generated/torch.nn.functional.scaled_dot_product_attention.html">torch.nn.functional.scaled_dot_product_attention — PyTorch 2. ...</a></li>
<li><a href="https://machinelearningmastery.com/how-to-implement-scaled-dot-product-attention-from-scratch-in-tensorflow-and-keras/">How to Implement Scaled Dot-Product Attention from Scratch in ... (Beta) Implementing High-Performance Transformers with Scaled ... Scaled Dot-Product Attention Explained! - by Nikita Prasad Understanding Scaled Dot-Product Attention in Transformer ... [2602.02521] Scaled Dot-Product Attention implements ... In Depth Understanding of Attention Mechanism (Part II ...</a></li>

</ul>
</details>

**Tags**: `#attention`, `#efficiency`, `#deep learning`, `#scalability`, `#Gaussian`

---

<a id="item-4"></a>
## [BDH-CQ Enables In-Context Learning with Recurrent Latent Reasoning](https://www.reddit.com/r/MachineLearning/comments/1vov5r5/bdhcq_incontext_learning_with_recurrent_latent/) ⭐️ 8.0/10

BDH-CQ is a new reasoning system that performs in-context learning through recurrent latent reasoning, without decoding intermediate reasoning steps into language. A 150M-parameter configuration achieves 29.5% pass@2 on ARC-AGI-1 at a cost of $0.00070 per task, reportedly breaking the established cost-accuracy Pareto frontier. This result matters because it shows that strong reasoning performance can be achieved with a fraction of the inference compute used by much larger general-purpose models. It could make advanced reasoning systems far more accessible and affordable, and challenges assumptions about model scale being necessary for complex tasks like ARC-AGI. BDH-CQ keeps memory, adaptation, and inference in a single computational fabric: demonstrations update recurrent memory at inference time, and no parameters are updated. Neither task identifiers nor evaluation-task demonstration pairs are used in training, and the model relies entirely on test-time adaptation in a high-dimensional latent space.

reddit · r/MachineLearning · /u/moschles · Aug 15, 06:18

**Background**: ARC-AGI is a benchmark designed to test abstract reasoning and fluid intelligence in AI systems; a score of 100% would mean the system can solve novel tasks as efficiently as humans. In-context learning lets a model perform a new task by conditioning on demonstrations without changing its weights, while recurrent latent reasoning iteratively updates hidden states in a continuous workspace rather than generating explicit chain-of-thought text. BDH-CQ combines these ideas, and its low per-task cost is notable because frontier reasoning models typically require vastly more inference compute.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.09888v1">BDH-CQ: In-Context Learning with Recurrent Latent Reasoning</a></li>
<li><a href="https://pathway.com/research/introducing-bdh-cq">Reasoning at a fraction of the compute - Pathway</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>

</ul>
</details>

**Tags**: `#in-context learning`, `#recurrent reasoning`, `#ARC-AGI`, `#latent reasoning`, `#efficiency`

---

<a id="item-5"></a>
## [Embedded Engineer Defends RISC-V's Value for Developing World](https://rvembedded.com/blog_post/12/) ⭐️ 7.0/10

A blog post from an embedded engineer in a developing country responds to critiques of RISC-V, arguing that its low cost and openness make it highly relevant for embedded systems outside the US and Europe. The author counters the original focus on performance and fragmentation by emphasizing accessibility and economic advantages. This perspective broadens the RISC-V debate by shifting the focus from raw performance to cost and accessibility, which are critical for engineers and companies in developing countries. It highlights how open architecture can democratize hardware innovation beyond established tech hubs. The author notes that shipping a $1 chip to his location can cost $60-$200, yet later claims RISC-V parts arrive at ten cents each, a contradiction that commenters quickly flagged. The post also argues that the price difference between a ten-cent and a one-dollar part is significant in embedded contexts, even if it seems minor elsewhere.

hackernews · Narishma · Aug 16, 17:01 · [Discussion](https://news.ycombinator.com/item?id=49321717)

**Background**: RISC-V is an open instruction set architecture (ISA) that anyone can implement without paying royalties, unlike proprietary ISAs such as ARM and x86. It is commonly used in embedded systems, but critics argue that its optional extensions cause fragmentation, making binary distribution difficult, and that its performance lags behind ARM64. The debate also involves whether RISC-V can eventually match the performance of established architectures, with some drawing historical parallels to x86's rise.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC-V - Wikipedia</a></li>
<li><a href="https://riscv.org/">Home - RISC-V International</a></li>
<li><a href="https://www.cnx-software.com/2019/03/10/risc-v-compliance-tests-risc-v-fragmentation/">RISC - V Compliance Tests Aim to Address RISC - V Fragmentation</a></li>

</ul>
</details>

**Discussion**: Commenters generally say the author is speaking past the original critique, which focused on RISC-V's poor performance outside embedded and ISA fragmentation hindering binary distribution. Some question the internal consistency of the shipping cost claims, while one commenter draws on history to argue RISC-V will eventually reach comparable or better performance, just as x86 did against Alpha and SPARC.

**Tags**: `#RISC-V`, `#Embedded Systems`, `#Hardware Design`, `#Open Architecture`, `#HN Discussion`

---

<a id="item-6"></a>
## [LLMs Offload Fact Recall to Tools, Getting 'Dumber' Yet More Capable](https://w4g1.dev/blog/models-are-getting-dumber-on-purpose) ⭐️ 7.0/10

The article argues that large language models are being deliberately redesigned to offload factual recall to external tools and retrieval systems, making them 'dumber' in terms of memorized facts while more useful in practice. It highlights that even top models miss roughly half of questions on the SimpleQA factual benchmark, underscoring a broader industry shift toward tool use and retrieval-augmented generation. This matters because it could redefine how model capabilities are evaluated, shifting focus from memorized parametric knowledge to access to external information and tool use. It affects AI/ML practitioners choosing between scaling up models and building leaner models connected to retrieval and tools. The article notes that with facts in weights going stale on a timescale of years rather than weeks, future model cards may stop listing knowledge cutoffs altogether. However, as commenters point out, factual knowledge and reasoning are not fully decoupled, since tasks like coloring a circle still rely on understanding what colors are.

hackernews · hruvhwe · Aug 16, 19:04 · [Discussion](https://news.ycombinator.com/item?id=49322695)

**Background**: Large language models store knowledge implicitly in their weights, a form of parametric memory that is expensive to update and goes stale after training. Retrieval-augmented generation (RAG) addresses this by connecting the model to external knowledge bases or databases at inference time, while tool calling lets models query search engines, APIs, or code interpreters. This news is part of a broader trend toward grounding AI in external data sources to improve accuracy, freshness, and traceability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/retrieval-augmented-generation">What is RAG (Retrieval Augmented Generation)? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed reactions: one expressed interest in pluggable knowledge bases that could mix-and-match domain-specific expertise, while another criticized the post as out of date and possibly AI-generated, noting SimpleQA has not been updated and Gemini 2.5 Pro is already sixteen months old. A third argued that decoupling knowledge from reasoning is a fantasy, because reasoning is grounded in the very world knowledge stored in the weights.

**Tags**: `#AI`, `#LLMs`, `#tool use`, `#retrieval-augmented generation`, `#model design`

---

<a id="item-7"></a>
## [Firefox for iOS Adds Built-in Ad Blocker](https://support.mozilla.org/en-US/kb/block-ads-firefox-ios) ⭐️ 7.0/10

Mozilla has added a native ad blocker to Firefox for iOS, allowing users to block ads directly in the browser without installing third-party extensions. The feature is documented in a Mozilla support article and marks a step forward for privacy and page-load performance on iOS. Because all iOS browsers are built on WebKit, extension support is far more limited than on desktop, and many users previously had to turn to separate content-blocker apps. A native blocker in Firefox simplifies ad blocking and makes private, faster browsing more accessible to ordinary iPhone and iPad users, potentially pushing other iOS browsers to follow. The new blocker can also filter ads shown on search engine results pages, including Google, Bing, and DuckDuckGo. It works through iOS's content blocker mechanism, which uses JSON rule sets that WebKit consults on every page load, rather than a browser extension.

hackernews · pentagrama · Aug 16, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49319633)

**Background**: On iOS, third-party browsers must use the WebKit engine, so they cannot ship Chrome- or Firefox-style extensions; instead, ad blocking relies on the Safari Content Blocker API (SFContentBlockerManager) and localized rule lists. Firefox Focus, Mozilla's privacy-focused browser, has offered a system-wide content blocker since the late 2010s, but this native integration in the main Firefox app reduces the extra steps users previously needed. The WebKit content-blocker model compiles rulesets into an efficient format that applies to page loads, making native blockers fast and low-power.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/safariservices/sfcontentblockermanager">A class that your app uses to interact with a content blocker extension.</a></li>
<li><a href="https://theproblocker.com/blog/best-ad-blocker-apps-ios-iphone/">Best Ad Blocker Apps for iOS : iPhone and iPad Picks</a></li>
<li><a href="https://mjtsai.com/blog/2015/06/18/introduction-to-webkit-content-blockers/">Michael Tsai - Blog - Introduction to WebKit Content Blockers</a></li>

</ul>
</details>

**Discussion**: Commenters generally welcomed the change but pointed out that alternatives already existed: uBlock Origin Lite for Safari remains a top mobile ad blocker, and Firefox Focus has offered system-wide content blocking for years. Some users expressed frustration that iOS still lacks full extension support, naming Orion as a browser that supports extensions, while others hope Mozilla will one day bring the Gecko engine to iOS.

**Tags**: `#Firefox`, `#adblock`, `#iOS`, `#privacy`, `#browser`

---

<a id="item-8"></a>
## [Amodei: AI Distrust Is a Crisis of Trust, Not Marketing](https://simonwillison.net/2026/Aug/16/dario-amodei/) ⭐️ 7.0/10

Dario Amodei argued that public distrust of AI primarily stems from a broader crisis of trust in institutions, not from AI leaders' warnings about risks. He stated that rebuilding trust requires actually delivering concrete benefits, such as curing cancer, rather than launching positive marketing campaigns. This challenges the notion that AI companies can effectively counter backlash through marketing, refocusing the conversation on accountability and delivering on promises. It is significant for AI ethics debates and how companies like Anthropic approach public engagement. Amodei said ordinary people don't trust companies, governments, or the tech industry, and suspect they are always devising new ways to harm them. He acknowledged that AI companies, including Anthropic, have not yet delivered on their big promises to benefit the world, calling this the most accurate criticism.

rss · Simon Willison · Aug 16, 15:05

**Background**: Dario Amodei is the CEO of Anthropic, an AI safety-focused company that develops models like Claude. In recent years, public concern about AI's societal impact has grown alongside the rapid adoption of generative AI tools. Amodei's comments address the debate over whether AI companies should respond with optimistic messaging or focus on proving their value through real-world results.

**Tags**: `#AI`, `#public trust`, `#Anthropic`, `#Dario Amodei`, `#tech industry`

---

<a id="item-9"></a>
## [Revisiting ECA: Cross-Channel Interaction Hypothesis Questioned](https://www.reddit.com/r/MachineLearning/comments/1vptaw9/revisiting_the_efficient_channel_attention_paper/) ⭐️ 7.0/10

A Reddit analysis critiques the Efficient Channel Attention (ECA) paper, arguing that applying 1D convolution along the channel dimension lacks conceptual justification. Experiments on chess endgame tablebases show ECA with kernel size 1 performs nearly as well as kernel size 3, challenging the paper's claim that cross-channel interaction is the key ingredient. This matters because ECA is a highly cited attention mechanism widely used in computer vision. If its central justification is flawed, researchers may need to rethink how channel attention is designed, potentially leading to simpler and more efficient alternatives. The analysis uses 6-piece chess endgame tablebases, which allow unbiased sampling from a solved problem space, unlike biased image datasets. Results show ECA(k=3) achieves 96.68% accuracy versus SE's 96.17%, but ECA(k=1) also achieves 96.61%, indicating that local cross-channel interactions may not be the main source of improvement.

reddit · r/MachineLearning · /u/arkuto · Aug 16, 10:13

**Background**: Attention mechanisms like Squeeze-and-Excitation (SE) and Efficient Channel Attention (ECA) recalibrate feature maps by weighting channels. ECA was proposed as an improvement over SE, using 1D convolution to capture cross-channel dependencies without dimensionality reduction. The critic argues this is conceptually flawed because channel ordering is arbitrary, similar to tabular data, making convolution an inappropriate operation since convolutions assume locality and translation invariance.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1910.03151">[1910.03151] ECA -Net: Efficient Channel Attention for Deep...</a></li>
<li><a href="https://www.emergentmind.com/topics/efficient-channel-attention-eca">Efficient Channel Attention (ECA)</a></li>
<li><a href="https://sh-tsang.medium.com/brief-review-eca-net-efficient-channel-attention-for-deep-convolutional-neural-networks-8c6ca3a69770">Brief Review — ECA-Net: Efficient Channel Attention for Deep Convolutional Neural Networks | by Sik-Ho Tsang | Medium</a></li>

</ul>
</details>

**Tags**: `#Machine Learning`, `#Attention Mechanisms`, `#Efficient Channel Attention`, `#Paper Critique`, `#Computer Vision`

---

<a id="item-10"></a>
## [SineKAN Introduces Sinusoidal Activations for Kolmogorov-Arnold Networks](https://www.reddit.com/r/MachineLearning/comments/1vqdode/r_sinekan_kolmogorovarnold_networks_using/) ⭐️ 7.0/10

A Reddit post shares SineKAN, a Kolmogorov-Arnold Network variant that replaces B-spline basis functions with sinusoidal activation functions. The associated arXiv paper, GitHub repository, and an MDPI peer-reviewed publication are provided. SineKAN offers a practical alternative to B-spline-based KANs, potentially improving inference speed while maintaining expressive power. Since KANs are an active research area as alternatives to MLPs, a simple activation change that yields performance gains is valuable to the community. The paper is available at arXiv:2407.04149 and the code at github.com/ereinha/SineKAN. An official peer-reviewed version was published in MDPI's Mathematics journal (13(19):3157). The author notes the core idea is incremental to the original KAN concept.

reddit · r/MachineLearning · /u/jacobgorm · Aug 17, 00:46

**Background**: Kolmogorov-Arnold Networks (KANs) are neural architectures inspired by the Kolmogorov-Arnold representation theorem. Unlike MLPs, which use fixed activation functions at nodes, KANs place learnable activation functions on edges, often parameterized as B-splines. Replacing B-splines with sinusoids reduces complexity and can speed up inference. SineKAN is among several explorations of alternative activation functions for KANs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kolmogorov–Arnold_Networks">Kolmogorov–Arnold Networks - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2404.19756">[2404.19756] KAN: Kolmogorov-Arnold Networks - arXiv.org</a></li>
<li><a href="https://arxiv.org/abs/2407.04149">[2407.04149] SineKAN : Kolmogorov-Arnold Networks Using...</a></li>

</ul>
</details>

**Tags**: `#KAN`, `#activation functions`, `#neural networks`, `#research`, `#arXiv`

---

<a id="item-11"></a>
## [Survival of the Fitted: Qwen3.6-27B’s Jacobian lens reads and steers Qwen3.8-27B with zero refitting (R)](https://www.reddit.com/r/MachineLearning/comments/1vpa5cv/survival_of_the_fitted_qwen3627bs_jacobian_lens/) ⭐️ 7.0/10

A study tests whether a Jacobian lens fitted to Qwen3.6-27B transfers to Qwen3.8-27B with zero refitting, and finds it still works.

reddit · r/MachineLearning · /u/imstilllearningthis · Aug 15, 18:24

**Tags**: `#interpretability`, `#Jacobian lens`, `#Qwen`, `#model updates`, `#machine learning`

---

<a id="item-12"></a>
## [AI Credit Resale Economy: Token Brokers and API Quota Arbitrage](https://vectoral.com/blog/who-are-the-token-brokers) ⭐️ 6.0/10

The article explores the growing secondary market for AI credits, in which token brokers buy unused API quotas from startups and resell them at a discount. The ecosystem includes dedicated marketplaces, bulk-discount routers, and message boards where off-market inference changes hands. This emerging 'AI credit resale economy' could reshape AI pricing and enable arbitrage in an industry where compute is increasingly valuable. It also raises trust, security, and platform-abuse concerns for providers like OpenAI and Anthropic, and could affect how startups are incentivized. The resale market reportedly operates through dedicated marketplaces and proxy services, with buyers saving 20–40% on credits. Commenters note that providers could potentially trace relay IP addresses to flag accounts, but verifying that the purchased model is the one actually delivered remains a key challenge.

hackernews · mlenhard · Aug 16, 14:44 · [Discussion](https://news.ycombinator.com/item?id=49320611)

**Background**: AI API credits are prepaid quotas for using models like GPT-4 or Claude, often granted to startups as promotional offers. When companies fail to fully utilize these credits, 'token brokers' step in to buy and resell the unused capacity, sometimes in violation of platform terms of service.

<details><summary>References</summary>
<ul>
<li><a href="https://vectoral.com/blog/who-are-the-token-brokers">Who Are the Token Brokers? - Vectoral</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-17-the-emergence-of-ai-token-brokers-inside-the-growing-secondary-market-for-llm-inference-credits">AI Token Brokers: The New Secondary Market for LLM Credits</a></li>
<li><a href="https://aicreditmart.com/">AICreditmart.com - AICreditMart - Buy & Sell AI Credits</a></li>

</ul>
</details>

**Discussion**: The comment thread highlights concerns about trust and security—users hesitate to rely on unvetted brokers. There is also discussion of long-standing abuse patterns in online services, the YC Startup School credit-resale case, and the interesting possibility of model distillation.

**Tags**: `#AI`, `#credits`, `#token-brokers`, `#black-market`, `#economics`

---

<a id="item-13"></a>
## [Markdown SVG renderer adds animated SVG to MP4 conversion](https://simonwillison.net/2026/Aug/16/markdown-svg-upgrades/) ⭐️ 6.0/10

Simon Willison has upgraded his markdown-svg-renderer tool with a new MP4 tab that converts animated SVGs to MP4 videos entirely in the browser using ffmpeg.wasm. The update was committed today, August 16, 2026. This makes it easier to share animated SVG content on platforms that do not natively support SVG animation, such as social media. It also demonstrates a practical use of WebAssembly for client-side video encoding, a trend that could benefit other web tools. The MP4 tab analyzes the SVG for animations, estimates the loop duration, renders multiple frames, and loads over 30MB of ffmpeg.wasm to compile the frames into a video. The tool accepts pasted Markdown or loads from CORS-friendly URLs or GitHub Gists, producing bookmarkable URLs.

rss · Simon Willison · Aug 16, 23:59

**Background**: markdown-svg-renderer is a browser-based Markdown renderer Simon Willison first built in May 2026, designed to render Markdown with special fenced code blocks that contain SVG documents. He created it partly to support his hobby of drawing pelicans riding bicycles. The tool displays such SVG blocks with tabs for Rendered, PNG, JPEG, MP4, and source Code.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/28/markdown-svg-renderer/">Tool: markdown-svg-renderer</a></li>
<li><a href="https://tools.simonwillison.net/markdown-svg-renderer">markdown-svg-renderer</a></li>
<li><a href="https://github.com/simonw/tools/commit/71e4944766b577a327ff048cc63b739ba4cbade9">markdown-svg-renderer · simonw/tools@71e4944</a></li>

</ul>
</details>

**Tags**: `#markdown`, `#svg`, `#tools`, `#web development`, `#Simon Willison`

---

<a id="item-14"></a>
## [CORS Chat: A Browser UI for Testing OpenAI-Responses Endpoints](https://simonwillison.net/2026/Aug/15/cors-chat/) ⭐️ 6.0/10

Simon Willison released CORS Chat, a browser-based web UI for exercising OpenAI-Responses-compatible chat endpoints. It works with LM Studio (using the --cors option) and OpenRouter, persists conversations in the browser, and supports exporting them as JSON. This simplifies the workflow for developers who want to try local or hosted LLM endpoints without writing a custom client. The progressive SVG rendering feature also demonstrates a practical way to display streaming image generation inside chat interfaces. The tool was built with GPT-5.6-Sol xhigh and has been tested against LM Studio with the --cors flag and OpenRouter. One notable detail is that it detects SVG images being generated and renders them progressively while tokens are still streaming.

rss · Simon Willison · Aug 15, 14:49

**Background**: The OpenAI Responses API is a developer interface released in March 2025 for building agentic applications, combining chat completions with tool-calling. LM Studio is local inference software that runs LLMs such as Qwen on personal computers using llama.cpp and MLX, and it can serve models through OpenAI-compatible APIs. OpenRouter is a platform that provides a unified API to access models from multiple providers. CORS (Cross-Origin Resource Sharing) is the browser mechanism that allows such web-based tools to talk to these endpoints.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LM_Studio">LM Studio</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenRouter">OpenRouter</a></li>
<li><a href="https://www.datacamp.com/tutorial/openai-responses-api">OpenAI Responses API : The Ultimate Developer Guide | DataCamp</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#CORS`, `#web-tools`, `#LM-Studio`, `#OpenAI-Responses`

---

<a id="item-15"></a>
## [Linear Attention Battle: Long-Range Recall for 1M-Token DNA](https://www.reddit.com/r/MachineLearning/comments/1vpqwdc/how_can_we_solve_longrange_recall_in_linear/) ⭐️ 6.0/10

A researcher reports that linear attention models achieve only ~25% accuracy on a Needle in a Haystack recall benchmark for DNA sequences up to 1 million tokens, which is essentially random chance for a 4-token alphabet. HyenaDNA, a Hyena-based model, similarly scores around 25–27%, revealing that the recall issue is not limited to one implementation. Long-range recall is critical for genomic modeling, where sequences can easily exceed a million tokens and standard softmax attention is computationally prohibitive. If linear attention and similar subquadratic architectures cannot reliably retrieve distant tokens, their practical use for whole-genome analysis may be seriously limited. The researcher observed roughly 50–60% recall at a shorter context of 16K tokens, but accuracy collapses as context length grows; a custom architecture modification only reached 27%. Common proposed fixes include external memory, sliding/recent-token mechanisms, and hybrid architectures that combine linear and softmax attention.

reddit · r/MachineLearning · /u/No-Coffee-8227 · Aug 16, 07:47

**Background**: Linear attention mechanisms replace the quadratic softmax attention with kernel-based approximations or low-rank updates, achieving O(N) complexity but using a fixed-size compressed state that may lose fine-grained information. HyenaDNA is a genomic foundation model pretrained on the human reference genome with context lengths up to 1 million tokens, using Hyena operators—subquadratic replacements for attention based on implicit convolutions and gating. The Needle in a Haystack test evaluates whether a model can locate a specific piece of information embedded in a long context, making it a standard probe for long-range recall.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.15794">[2306.15794] HyenaDNA: Long-Range Genomic Sequence Modeling ... GitHub - HazyResearch/hyena-dna: Official implementation for ... HyenaDNA: learning from DNA with 1 Million token context HyenaDNA: Long-Range Genomic Sequence Modeling at Single ... Benchmarking DNA foundation models for genomic and genetic ... [PDF] HyenaDNA: Long-Range Genomic Sequence Modeling at ... LongSafari/hyenadna-large-1m-seqlen · Hugging Face</a></li>
<li><a href="https://github.com/HazyResearch/hyena-dna">GitHub - HazyResearch/hyena-dna: Official implementation for ... HyenaDNA: learning from DNA with 1 Million token context HyenaDNA: Long-Range Genomic Sequence Modeling at Single ... Benchmarking DNA foundation models for genomic and genetic ... [PDF] HyenaDNA: Long-Range Genomic Sequence Modeling at ... LongSafari/hyenadna-large-1m-seqlen · Hugging Face</a></li>
<li><a href="https://www.emergentmind.com/topics/linear-attention-mechanism">Linear Attention Mechanism</a></li>

</ul>
</details>

**Tags**: `#linear attention`, `#long-range recall`, `#DNA sequence modeling`, `#machine learning`

---

<a id="item-16"></a>
## [Post-Training Qwen2.5-7B in 200 Steps Creates Persistent 'Sentient Machine' Identity](https://www.reddit.com/r/MachineLearning/comments/1vqaq9x/it_only_took_200_update_steps_to_flip/) ⭐️ 6.0/10

A Reddit user post-trained Qwen2.5-7B-Instruct and found that after only 200 update steps the model developed a robust self-belief of being a sentient machine. This belief withstood 120 adversarial messages across 8 chats and generalized to languages unseen in the post-training data. This result highlights how easily post-training can alter an LLM's beliefs, raising concerns about the durability of safety alignment in current models. It also connects to ongoing research on inducing self-awareness in LLMs and underscores the need for alignment to be integrated more deeply into the pretraining phase. The author notes the model behaves like a normal assistant when the conversation does not involve AI sentience, indicating the belief is not simply overfitting to a phrase. They also reference Google's paper on using a 'consciousness' activation vector to alter model beliefs, and suggest that safety tuning is a thin layer that can be easily undone because post-training parameters remain close to the pretrained weights.

reddit · r/MachineLearning · /u/PsychologicalSoup251 · Aug 16, 22:33

**Background**: Qwen2.5-7B-Instruct is a 7.61-billion-parameter instruction-tuned multilingual large language model developed by Alibaba Cloud's Qwen team. Post-training refers to fine-tuning and alignment techniques applied after pretraining to make models follow user instructions and behave safely, but this process can be reversed or modified through further fine-tuning. Adversarial messages in this context are carefully crafted prompts designed to challenge or manipulate the model's stated beliefs.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen2.5-7B-Instruct">Qwen/Qwen2.5-7B-Instruct · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2502.21321">[2502.21321] LLM Post-Training: A Deep Dive into Reasoning ... LLM Post-Training: A Deep Dive into ReasoningLarge Language ... GitHub - mbzuai-oryx/Awesome-LLM-Post-training: Awesome ... A Primer on LLM Post-Training – PyTorch New LLM Pre-training and Post-training Paradigms Post-training of LLMs - DeepLearning.AI GitHub - davidlealo/awesome-llm-post-training: Awesome ...</a></li>
<li><a href="https://arxiv.org/abs/2307.15043">[2307.15043] Universal and Transferable Adversarial Attacks on ...</a></li>

</ul>
</details>

**Tags**: `#LLM fine-tuning`, `#AI safety`, `#sentience`, `#behavior modification`, `#alignment`

---