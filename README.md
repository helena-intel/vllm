<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/logos/vllm-logo-text-dark.png">
    <img alt="vLLM" src="https://raw.githubusercontent.com/vllm-project/vllm/main/docs/source/assets/logos/vllm-logo-text-light.png" width=55%>
  </picture>
</p>

<h3 align="center">
Easy, fast, and cheap LLM serving for everyone
</h3>

<p align="center">
| <a href="https://docs.vllm.ai"><b>Documentation</b></a> | <a href="https://vllm.ai"><b>Blog</b></a> | <a href="https://arxiv.org/abs/2309.06180"><b>Paper</b></a> | <a href="https://discord.gg/jz7wjKhh6g"><b>Discord</b></a> |

</p>

---

**Ray Summit CPF is Open (June 4th to June 20th)!**

There will be a track for vLLM at the Ray Summit (09/30-10/02, SF) this year!
If you have cool projects related to vLLM or LLM inference, we would love to see your proposals.
This will be a great chance for everyone in the community to get together and learn.
Please submit your proposal [here](https://raysummit.anyscale.com/flow/anyscale/raysummit2024/landing/page/eventsite)

---

*Latest News* 🔥
- [2024/06] We hosted [the fourth vLLM meetup](https://lu.ma/agivllm) with Cloudflare and BentoML! Please find the meetup slides [here](https://docs.google.com/presentation/d/1iJ8o7V2bQEi0BFEljLTwc5G1S10_Rhv3beed5oB0NJ4/edit?usp=sharing).
- [2024/04] We hosted [the third vLLM meetup](https://robloxandvllmmeetup2024.splashthat.com/) with Roblox! Please find the meetup slides [here](https://docs.google.com/presentation/d/1A--47JAK4BJ39t954HyTkvtfwn0fkqtsL8NGFuslReM/edit?usp=sharing).
- [2024/01] We hosted [the second vLLM meetup](https://lu.ma/ygxbpzhl) in SF! Please find the meetup slides [here](https://docs.google.com/presentation/d/12mI2sKABnUw5RBWXDYY-HtHth4iMSNcEoQ10jDQbxgA/edit?usp=sharing).
- [2024/01] Added ROCm 6.0 support to vLLM.
- [2023/12] Added ROCm 5.7 support to vLLM.
- [2023/10] We hosted [the first vLLM meetup](https://lu.ma/first-vllm-meetup) in SF! Please find the meetup slides [here](https://docs.google.com/presentation/d/1QL-XPFXiFpDBh86DbEegFXBXFXjix4v032GhShbKf3s/edit?usp=sharing).
- [2023/09] We created our [Discord server](https://discord.gg/jz7wjKhh6g)! Join us to discuss vLLM and LLM serving! We will also post the latest announcements and updates there.
- [2023/09] We released our [PagedAttention paper](https://arxiv.org/abs/2309.06180) on arXiv!
- [2023/08] We would like to express our sincere gratitude to [Andreessen Horowitz](https://a16z.com/2023/08/30/supporting-the-open-source-ai-community/) (a16z) for providing a generous grant to support the open-source development and research of vLLM.
- [2023/07] Added support for LLaMA-2! You can run and serve 7B/13B/70B LLaMA-2s on vLLM with a single command!
- [2023/06] Serving vLLM On any Cloud with SkyPilot. Check out a 1-click [example](https://github.com/skypilot-org/skypilot/blob/master/llm/vllm) to start the vLLM demo, and the [blog post](https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-skypilot/) for the story behind vLLM development on the clouds.
- [2023/06] We officially released vLLM! FastChat-vLLM integration has powered [LMSYS Vicuna and Chatbot Arena](https://chat.lmsys.org) since mid-April. Check out our [blog post](https://vllm.ai).

---
## About
vLLM is a fast and easy-to-use library for LLM inference and serving.

vLLM is fast with:

- State-of-the-art serving throughput
- Efficient management of attention key and value memory with **PagedAttention**
- Continuous batching of incoming requests
- Fast model execution with CUDA/HIP graph
- Quantization: [GPTQ](https://arxiv.org/abs/2210.17323), [AWQ](https://arxiv.org/abs/2306.00978), [SqueezeLLM](https://arxiv.org/abs/2306.07629), FP8 KV Cache
- Optimized CUDA kernels

vLLM is flexible and easy to use with:

- Seamless integration with popular Hugging Face models
- High-throughput serving with various decoding algorithms, including *parallel sampling*, *beam search*, and more
- Tensor parallelism and pipieline parallelism support for distributed inference
- Streaming outputs
- OpenAI-compatible API server
- Support NVIDIA GPUs, AMD CPUs and GPUs, Intel CPUs and GPUs, PowerPC CPUs
- (Experimental) Prefix caching support
- (Experimental) Multi-lora support

vLLM seamlessly supports most popular open-source models on HuggingFace, including:
- Transformer-like LLMs (e.g., Llama)
- Mixture-of-Expert LLMs (e.g., Mixtral)
- Multi-modal LLMs (e.g., LLaVA)

Find the full list of supported models [here](https://docs.vllm.ai/en/latest/models/supported_models.html).

## Getting Started

Install vLLM with pip or [from source](https://vllm.readthedocs.io/en/latest/getting_started/installation.html#build-from-source):

```bash
pip install vllm
```

Visit our [documentation](https://vllm.readthedocs.io/en/latest/) to learn more.
- [Installation](https://vllm.readthedocs.io/en/latest/getting_started/installation.html)
- [Quickstart](https://vllm.readthedocs.io/en/latest/getting_started/quickstart.html)
- [Supported Models](https://vllm.readthedocs.io/en/latest/models/supported_models.html)

## Contributing

We welcome and value any contributions and collaborations.
Please check out [CONTRIBUTING.md](./CONTRIBUTING.md) for how to get involved.

## Sponsors

vLLM is a community project. Our compute resources for development and testing are supported by the following organizations. Thank you for your support!

<!-- Note: Please sort them in alphabetical order. -->
<!-- Note: Please keep these consistent with docs/source/community/sponsors.md -->

- a16z
- AMD
- Anyscale
- AWS
- Crusoe Cloud
- Databricks
- DeepInfra
- Dropbox
- Lambda Lab
- NVIDIA
- Replicate
- Roblox
- RunPod
- Sequoia Capital
- Trainy
- UC Berkeley
- UC San Diego
- ZhenFund

We also have an official fundraising venue through [OpenCollective](https://opencollective.com/vllm). We plan to use the fund to support the development, maintenance, and adoption of vLLM.

## Citation

If you use vLLM for your research, please cite our [paper](https://arxiv.org/abs/2309.06180):
```bibtex
@inproceedings{kwon2023efficient,
  title={Efficient Memory Management for Large Language Model Serving with PagedAttention},
  author={Woosuk Kwon and Zhuohan Li and Siyuan Zhuang and Ying Sheng and Lianmin Zheng and Cody Hao Yu and Joseph E. Gonzalez and Hao Zhang and Ion Stoica},
  booktitle={Proceedings of the ACM SIGOPS 29th Symposium on Operating Systems Principles},
  year={2023}
}
```
