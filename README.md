# ember-papers

A simple paper-reading repository for the Ember project.

## Goal

Build the full theory base needed for an Ember C++ native training/inference loop.

## Reading Plan (Time-Agnostic)

### Phase 0: Hybrid Attention foundation
- FlashAttention (v1/v2)
- Linear Attention and DeltaNet family
- Mamba/SSD basics
- RoPE and GQA
- Outcome: understand every core component behind Qwen3.5 Hybrid Attention

### Phase 1: MoE systems
- Shazeer MoE, Switch Transformer, Expert Choice, MegaBlocks
- DeepSeek-V2 / DeepSeek-V3
- KTransformers
- Outcome: understand shared vs routed experts, load balancing, and CPU-GPU heterogeneous scheduling

### Phase 2: Quantization and low precision
- GPTQ, LLM.int8(), FP8 Formats, Marlin
- MTP and Speculative Decoding
- Outcome: understand W8A16 strategy and dequant + GEMM fusion

### Phase 3: Serving runtime
- CUDA Graphs
- vLLM / PagedAttention
- Outcome: understand continuous batching and paged memory management

### Phase 4: Training alignment and self-improvement
- LoRA / QLoRA
- InstructGPT, PPO, DPO, GRPO, DeepSeek-R1
- Self-Consistency, KD, SPIN, STaR
- Outcome: complete training-side theory for Ember

## Storylines

1. Linear Attention -> DeltaNet
2. FlashAttention
3. MoE
4. Quantization and low precision
5. Serving systems
6. Fine-tuning, RLHF/RL, and self-improvement

## Important Note

- `MLPerf Inference Benchmark` is included as an additional benchmark/system reference paper.

## Repository Policy

- `*.pdf` files are tracked
- `*.tex` files are ignored
