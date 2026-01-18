# LLM verbatim recall

## Factors

Position effects: primacy and recency strong, middle degraded (lost in the middle)
Content type: random tokens hardest, structured prose easier
Interference: more context = more competition for attention

## Expected accuracy by token count

| Tokens | Random | Prose |
|--------|--------|-------|
| 50     | 98%    | 99%   |
| 200    | 85%    | 95%   |
| 500    | 60%    | 85%   |
| 1000   | 30%    | 70%   |
| 2000   | 10%    | 50%   |

## Point estimate for 90%+ verbatim accuracy

Random tokens: 100-200 tokens
Structured prose: 400-800 tokens

## In bits (×16 bits/token)

Random: 1,600-3,200 bits
Prose: 6,400-12,800 bits

## Confidence interval (80%)

Lower bound: 50 tokens = 800 bits
Median: ~300 tokens = ~5,000 bits
Upper bound: 1,500 tokens = 24,000 bits
