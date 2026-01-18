# ML Musings

Facts and hypotheses on machine learning, memory, and cognition.

## Facts

### Bandwidth

1. Human sensory input is ~10⁸ bits/s. [Koch et al. 2006](https://pmc.ncbi.nlm.nih.gov/articles/PMC1564115/), [Zheng & Meister 2024](https://pubmed.ncbi.nlm.nih.gov/39694032/)

2. Human cognitive throughput is only ~10 bits/s. [Zheng & Meister 2024](https://pubmed.ncbi.nlm.nih.gov/39694032/)

3. Human speech transmits ~39 bits/s, invariant across languages. [Coupé et al. 2019](https://www.science.org/doi/10.1126/sciadv.aaw2594)

4. Humans memorize at ~2 bits/s regardless of modality. [Landauer 1986](https://www.sciencedirect.com/science/article/abs/pii/S0364021386800143)

5. LLM output is ~10²-10⁴ bits/s depending on deployment. [conversation, 2025-01]

6. English text entropy is ~0.6-1.3 bits/character. [PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC7514546/)

### Memory

7. Human working memory capacity is ~4±1 chunks. [Cowan 2001](https://pubmed.ncbi.nlm.nih.gov/11515286/)

8. Bits per chunk ranges from 1 (binary digit) to ~30 (pointer to known concept). [Fermi estimate, 2025-01]

9. Human working memory holds ~40-120 bits total, depending on encoding efficiency. [Fermi estimate, 2025-01]

10. Human lifetime memory accumulation is ~10⁹ bits. [Landauer 1986](https://www.sciencedirect.com/science/article/abs/pii/S0364021386800143)

11. A chunk is a pointer to long-term memory, defined by pre-existing associations. [Cowan 2001](https://pubmed.ncbi.nlm.nih.gov/11515286/)

12. Chunking is equivalent to data compression. [Chekaf, Cowan & Mathy 2016](https://pmc.ncbi.nlm.nih.gov/articles/PMC4983232/)

13. LLM reliable verbatim recall is ~300 tokens / ~5,000 bits. [Fermi estimate, 2025-01]

### Comparison

14. Human memory is continuously lossy with narrative confabulation; LLM memory is perfectly volatile with hard cutoffs. [conversation, 2025-01]

15. LLMs are atemporal; humans live in the time dimension. [conversation, 2025-01]

16. CLI interfaces are more token-efficient for LLM agents than REST/MCP/JSON. [conversation, 2025-01]

## Hypotheses

1. Model judgment as compression function may outperform naive truncation for context management. [conversation, 2025-01]

2. Credit assignment in learning is emergent and implicit, not a problem to engineer explicitly. [conversation, 2025-01]

3. Learning happens at multiple timescales: training (months), fine-tuning (weeks), in-context (conversation). [conversation, 2025-01]

4. The conversation log (jsonl) serves as interface between human↔LLM and LLM↔external storage. [conversation, 2025-01]

5. Scaffolds can be learned and discarded; they're tooling, not precious. [conversation, 2025-01]

6. Online SFT should be slow (~2 bits/s) to match human learning rates and avoid catastrophic forgetting. [conversation, 2025-01]

7. Research at the intersection of prompt engineering and RL/fine-tuning is underdeveloped. [conversation, 2025-01]

8. The "lost in the middle" problem means effective LLM working memory is smaller than context window. [conversation, 2025-01]

9. Compaction done right isn't summarization—it's integration: resolving contradictions, strengthening connections, pruning noise. [conversation, 2025-01]

10. Fast learning fails because there's no time for integration; slow might be the only way that works. [conversation, 2025-01]
