# ML Musings

Facts and hypotheses on machine learning, memory, and cognition.

## Facts

Human sensory input is ~10⁸ bits/s. [Koch et al. 2006](https://pmc.ncbi.nlm.nih.gov/articles/PMC1564115/), [Zheng & Meister 2024](https://pubmed.ncbi.nlm.nih.gov/39694032/)

Human cognitive throughput is only ~10 bits/s. [Zheng & Meister 2024](https://pubmed.ncbi.nlm.nih.gov/39694032/)

Human speech transmits ~39 bits/s, invariant across languages. [Coupé et al. 2019](https://www.science.org/doi/10.1126/sciadv.aaw2594)

Humans memorize at ~2 bits/s regardless of modality. [Landauer 1986](https://www.sciencedirect.com/science/article/abs/pii/S0364021386800143)

LLM output is ~10²-10⁴ bits/s depending on deployment.

English text entropy is ~0.6-1.3 bits/character. [Ren, Takahashi & Tanaka-Ishii 2019](https://pmc.ncbi.nlm.nih.gov/articles/PMC7514546/)

Human working memory capacity is ~4±1 chunks. [Cowan 2001](https://pubmed.ncbi.nlm.nih.gov/11515286/)

Bits per chunk ranges from 1 (binary digit) to ~30 (pointer to known concept). [estimate](fermi_superforecasts/bits_per_chunk.md)

Human working memory holds ~40-120 bits total, depending on encoding efficiency. [estimate](fermi_superforecasts/working_memory_bits.md)

Human lifetime memory accumulation is ~10⁹ bits. [Landauer 1986](https://www.sciencedirect.com/science/article/abs/pii/S0364021386800143)

A chunk is a pointer to long-term memory, defined by pre-existing associations. [Cowan 2001](https://pubmed.ncbi.nlm.nih.gov/11515286/)

Chunking is equivalent to data compression. [Chekaf, Cowan & Mathy 2016](https://pmc.ncbi.nlm.nih.gov/articles/PMC4983232/)

LLM reliable verbatim recall is ~300 tokens / ~5,000 bits. [estimate](fermi_superforecasts/llm_verbatim_recall.md)

In interactive chat, human cognitive throughput (~10-50 bits/s) is lower than LLM output throughput (~10²-10⁴ bits/s). [Zheng & Meister 2024](https://pubmed.ncbi.nlm.nih.gov/39694032/)

Human sensory input bandwidth (10⁷-10⁹ bits/s) exceeds LLM text bandwidth (10²-10⁴ bits/s) by 3-7 orders of magnitude. [Koch et al. 2006](https://pmc.ncbi.nlm.nih.gov/articles/PMC1564115/), [Zheng & Meister 2024](https://pubmed.ncbi.nlm.nih.gov/39694032/)

Human memory is continuously lossy with narrative confabulation; LLM memory is perfectly volatile with hard cutoffs.

LLMs are atemporal; humans live in the time dimension.

CLI interfaces are more token-efficient than REST/MCP/JSON for both LLMs and humans.

Progress lives in files and git, not in context; each loop gets a fresh agent with fresh context. [Huntley 2025](https://www.humanlayer.dev/blog/brief-history-of-ralph)

Anthropic's compaction uses abstractive summarization with quotes (memorization), optimizing against false negatives.

## Hypotheses

Model judgment as compression function may outperform naive truncation for context management.

Explicit handoff prompting optimizes for true positives; combined with compaction it forms a tandem compression system.

Credit assignment in learning is emergent and implicit, not a problem to engineer explicitly.

Learning happens at multiple timescales: training (months), fine-tuning (weeks), in-context (conversation).

The conversation log (jsonl) serves as interface between human and LLM and between LLM and external storage.

Scaffolds can be learned and discarded; they're tooling, not precious.

Online SFT should be slow (~2 bits/s) to match human learning rates and avoid catastrophic forgetting.

Research at the intersection of prompt engineering and RL/fine-tuning is underdeveloped.

The "lost in the middle" problem means effective LLM working memory is smaller than context window.

Compaction done right is not summarization but integration: resolving contradictions, strengthening connections, pruning noise.

Fast learning fails because there is no time for integration; slow might be the only way that works.
