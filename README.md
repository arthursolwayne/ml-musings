# ML Musings

Facts and hypotheses on machine learning, memory, and cognition.

## Facts

Human sensory input is ~10⁸ bits/s. [[1]](#ref-1) [[2]](#ref-2)

Human cognitive throughput is only ~10 bits/s. [[2]](#ref-2)

Human speech transmits ~39 bits/s, invariant across languages. [[3]](#ref-3)

Humans memorize at ~2 bits/s regardless of modality. [[4]](#ref-4)

LLM output is ~10²-10⁴ bits/s depending on deployment.

English text entropy is ~0.6-1.3 bits/character. [[5]](#ref-5)

Human working memory capacity is ~4±1 chunks. [[6]](#ref-6)

Bits per chunk ranges from 1 (binary digit) to ~30 (pointer to known concept). [[e1]](#ref-e1)

Human working memory holds ~40-120 bits total, depending on encoding efficiency. [[e2]](#ref-e2)

Human lifetime memory accumulation is ~10⁹ bits. [[4]](#ref-4)

A chunk is a pointer to long-term memory, defined by pre-existing associations. [[6]](#ref-6)

Chunking is equivalent to data compression. [[7]](#ref-7)

LLM reliable verbatim recall is ~300 tokens / ~5,000 bits. [[e3]](#ref-e3)

In interactive chat, human cognitive throughput (~10-50 bits/s) is lower than LLM output throughput (~10²-10⁴ bits/s). [[2]](#ref-2)

Human sensory input bandwidth (10⁷-10⁹ bits/s) exceeds LLM text bandwidth (10²-10⁴ bits/s) by 3-7 orders of magnitude. [[1]](#ref-1) [[2]](#ref-2)

Human memory is continuously lossy with narrative confabulation; LLM memory is perfectly volatile with hard cutoffs.

LLMs are atemporal; humans live in the time dimension.

CLI interfaces are more token-efficient than REST/MCP/JSON for both LLMs and humans.

Progress lives in files and git, not in context; each loop gets a fresh agent with fresh context. [[8]](#ref-8)

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

## References

<a id="ref-1"></a>[[1]](https://pmc.ncbi.nlm.nih.gov/articles/PMC1564115/) Koch et al. 2006

<a id="ref-2"></a>[[2]](https://pubmed.ncbi.nlm.nih.gov/39694032/) Zheng & Meister 2024

<a id="ref-3"></a>[[3]](https://www.science.org/doi/10.1126/sciadv.aaw2594) Coupé et al. 2019

<a id="ref-4"></a>[[4]](https://www.sciencedirect.com/science/article/abs/pii/S0364021386800143) Landauer 1986

<a id="ref-5"></a>[[5]](https://pmc.ncbi.nlm.nih.gov/articles/PMC7514546/) Ren, Takahashi & Tanaka-Ishii 2019

<a id="ref-6"></a>[[6]](https://pubmed.ncbi.nlm.nih.gov/11515286/) Cowan 2001

<a id="ref-7"></a>[[7]](https://pmc.ncbi.nlm.nih.gov/articles/PMC4983232/) Chekaf, Cowan & Mathy 2016

<a id="ref-8"></a>[[8]](https://www.humanlayer.dev/blog/brief-history-of-ralph) Huntley 2025

<a id="ref-e1"></a>[[e1]](fermi_superforecasts/bits_per_chunk.md) estimate

<a id="ref-e2"></a>[[e2]](fermi_superforecasts/working_memory_bits.md) estimate

<a id="ref-e3"></a>[[e3]](fermi_superforecasts/llm_verbatim_recall.md) estimate
