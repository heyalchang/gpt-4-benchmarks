# GPT-4 Benchmarks

Reverse-engineering the GPT-4 language model through simulation.

## What we know so far

Unconfirmed statement that GPT-4 is "8 x 220 B with 16 inferences". What those words mean is not completely understood. You would expect 8 separate models = 8 separate inferences, but instead we have 16. Why?

Empirical data:
- 13.1 tokens/second peak on the OpenAI API, with 6-12 tokens/second on average
- Another independent source measured 8-9 tokens/second

TODO:

Swift Colab notebook that inputs data about max bandwidth achieved on A100 for FP16 and Int8 matrix multiplication, inputs latency of FlashAttention for different sequence sizes.
