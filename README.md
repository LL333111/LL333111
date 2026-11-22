<picture>
  <source media="(prefers-color-scheme: dark)" srcset="hero-v2-dark.svg">
  <img alt="Lucas Liu, open to opportunities" src="hero-v2-light.svg" width="100%">
</picture>

### Research experiments

| Project | Description |
|:--|:--|
| [causalpfn-large-tables](https://github.com/LL333111/causalpfn-large-tables) | Why does CausalPFN drop on full-size uplift tables? Most of its ranking comes from a small weak learner; giving that estimate to the model as an input column lifts full-X5 Qini **0.607 → 0.790**, and is not worse on any of 8 tables |

### Post-training

| Project | Description |
|:--|:--|
| [rl-text2sql](https://github.com/LL333111/rl-text2sql) | GRPO with SQL-execution rewards teaches a 1.5B coder model SQL: Spider **62.2% → 70.2%**, and **+5.7 pts** over SFT on unseen BIRD |
| [rlvr-posttraining](https://github.com/LL333111/rlvr-posttraining) | Does RL with a verifier beat more SFT on the same compute? Yes: GSM8K **48.4% → 55.6%** |
| [financial-report-calculator](https://github.com/LL333111/financial-report-calculator) | Model writes a small program to compute answers from financial reports: **66.7%** on FinQA with rejection-sampling SFT |
| [financial-fact-extractor](https://github.com/LL333111/financial-fact-extractor) | Pull a figure and its scale from report tables and text: **30.3% → 64.9%** after fine-tuning |

### Fine-tuning, distillation and inference

| Project | Description |
|:--|:--|
| [shopify-catalogue-vlm](https://github.com/LL333111/shopify-catalogue-vlm) | Predict product category, brand and condition from images and text: F1 **0.755 → 0.823**, served in FP8 with **40%** less memory |
| [relevance-judge-distill](https://github.com/LL333111/relevance-judge-distill) | Turn 5K human labels into a 0.6B product-search reranker via a 14B LLM judge: nDCG@10 **0.783 → 0.800**, **10×** faster than the judge |
| [local-financial-qa](https://github.com/LL333111/local-financial-qa) | Answer questions about a financial report on a laptop CPU, with citations: **52.1%** correct vs. 31.3% for direct generation |
| [transformer-training-scaling](https://github.com/LL333111/transformer-training-scaling) | How much faster does GPT-2-small reach a target loss with SDPA and DDP? **624 s → 107 s** |

### Agents and other work

| Project | Description |
|:--|:--|
| [ContextRepair](https://github.com/LL333111/ContextRepair) | Can coding agents recover from failed attempts on SWE-bench Verified? An honest negative result (**22/40** either way) |
| [ehr-forecast-final](https://github.com/LL333111/ehr-forecast-final) | Forecast five-year diagnoses from electronic health records |

### Stack

<table>
<tr><td><b>Languages</b></td><td>Python · C · JavaScript · SQL · Bash</td></tr>
<tr><td><b>Training</b></td><td>PyTorch · Transformers · TRL · PEFT / LoRA</td></tr>
<tr><td><b>Post-training</b></td><td>GRPO · SFT · rejection-sampling SFT · DPO</td></tr>
<tr><td><b>Serving</b></td><td>vLLM · llama.cpp · FP8 / GPTQ quantization</td></tr>
<tr><td><b>Data & infra</b></td><td>FAISS · Docker · Linux · Git</td></tr>
</table>

[LinkedIn](https://www.linkedin.com/in/lucas-liu-6a83162a0/)
