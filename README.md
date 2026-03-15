<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=changshenhan&style=flat-square&color=blueviolet)

# Chang Shenhan

**Zero-Knowledge ML · Privacy-Preserving Inference · Circuit-Optimized Activations**

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/changshenhan)

</div>

---

## About

Contributor to **[ezkl](https://github.com/zkonduit/ezkl)** (zero-knowledge inference engine). Focus: **custom lookup tables** for Sigmoid/PWL in ZK-SNARK circuits, accuracy vs. circuit-size trade-offs, and **privacy-preserving inference** (incl. Apple Silicon–native protocols).

- **ezkl**: PR for optional custom PWL lookup (JSON-defined breakpoints/slopes/intercepts); input-range enforcement and soundness checks.
- **Experiments**: Quantile-based PWL breakpoints, Sigmoid lookup vs. PLA comparison, full prove/verify pipelines with quantified accuracy (e.g. ~1e-11 vs. true σ(x)).
- **STIP-MLX**: Secure Tensor Inference Protocol — block-diagonal permutation for private LLM inference on Apple Silicon (MLX); server only sees permuted tensors.

---

## Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch" />
  <img src="https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white" alt="ONNX" />
  <img src="https://img.shields.io/badge/MLX-000000?style=for-the-badge&logo=apple&logoColor=white" alt="MLX" />
</p>

`Halo2` · `zk-SNARKs` · `piecewise-linear approximation` · `fixed-point quantization` · `lookup tables`

---

## Featured Projects

| Project | Description |
|---------|-------------|
| [**ezkl**](https://github.com/changshenhan/ezkl) | Fork with optional custom lookup table (PWL from JSON) for Sigmoid; contributes upstream. |
| [**ezkl-custom-lookup-experiment**](https://github.com/changshenhan/ezkl-custom-lookup-experiment) | Full pipeline: built-in vs. custom PWL Sigmoid lookup; quantile-based breakpoints; ~1.1s prove, verified. |
| [**zkml_lookup_experiment**](https://github.com/changshenhan/zkml_lookup_experiment) | Sigmoid lookup vs. PLA comparison; metrics and accuracy analysis (e.g. 1–2 orders of magnitude improvement with custom PWL). |
| [**STIP-MLX**](https://github.com/changshenhan/STIP-MLX) | Secure Tensor Inference Protocol — private LLM inference on Apple Silicon (Qwen2.5-3B); permuted feature space, 8GB-friendly. |
| [**awesome-zkml**](https://github.com/changshenhan/awesome-zkml) | Curated ZKML resources and references. |

---

## GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=changshenhan&show_icons=true&theme=github_dark&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub Stats" width="400" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=changshenhan&layout=compact&theme=github_dark&hide_border=true&exclude_repo=changshenhan" alt="Top Languages" width="350" />

</div>

---

<div align="center">

*Verifiable inference · Custom lookups · Privacy by design*

</div>

