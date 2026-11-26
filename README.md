# Noor Mkdad

Backend and platform engineer building production APIs, deterministic data systems, Linux infrastructure, and cost-controlled LLM serving.

[Portfolio](https://noormkdad.com) · [Stanza API](https://stanzaapi.com) · [LinkedIn](https://linkedin.com/in/noor-mkdad-6b0a77293) · [Email](mailto:noorhayatywadam@gmail.com)

Open to full-time W-2 backend, platform, systems, and AI infrastructure roles (US remote or Orange County, CA).

## Production & Systems Work

| Project | Focus | Proof |
| :-- | :-- | :-- |
| [Stanza API](https://stanzaapi.com) | 12 production APIs on Cloudflare Workers for healthcare claims, payments, and supply-chain data, with OpenAPI 3.1 SDK generation (44 packages) and an MCP server. | [X12 parser benchmark](https://github.com/StanzaAPI/benchmark-harness): 255,000 claim records in 14.2 s inside a 25 MB V8 old-space cap. |
| [stanza-lsm](https://github.com/StanzaAPI/stanza-lsm) & [stanza-mux](https://github.com/StanzaAPI/stanza-mux) | Zero-dependency Rust (`#![forbid(unsafe_code)]`) WAL/LSM storage engine and WebSocket session multiplexer with deterministic simulation testing. | Published on [crates.io](https://crates.io/crates/stanza-lsm); 2,000 DST seeds with zero invariant failures. |
| [Local Inference Stack](https://github.com/risingpresage/local-inference-stack) | OpenAI-compatible GPU serving gateway with cost-aware routing, Prometheus metrics, MCP server, and Nix flake. | $0.19–0.41 per 1M tokens measured; 286 tok/s across 4 slots. |
| [KV Serving Scheduler](https://github.com/risingpresage/kv-serving-scheduler) | Pure-Go block KV allocator, priority/WFQ queues, and recompute preemption for llama.cpp. | 74 ms p99 TTFT for high-priority tenants under 4 req/s overload. |
| [llama.cpp Vulkan Kernel](https://github.com/risingpresage/llama-vulkan-matvec-rdna4) | K-quant dequantization hoisting and 8-row blocking in `mul_mat_vecq` for RDNA4. | +13.4% 8-slot decode throughput, bit-identical greedy outputs ([PR #31022](https://github.com/ggml-org/llama.cpp/pull/31022)). |
| [Platform Infra](https://github.com/risingpresage/platform-infra) & [NixOS Config](https://github.com/risingpresage/NixOS-Config) | Declarative OpenTofu (Proxmox VE), Kubernetes/Helm, Authentik OIDC SSO, Prometheus/Grafana, and multi-host NixOS flakes. | Reproducible bare-metal builds with documented incident runbooks. |

## Agent & Research Tooling

[pi-sieve](https://github.com/risingpresage/pi-sieve) · [cat-burglar](https://github.com/risingpresage/cat-burglar) · [valkey-kv-l2](https://github.com/risingpresage/valkey-kv-l2) · [paged-attention-lab](https://github.com/risingpresage/paged-attention-lab) · [speculative-decoding-lab](https://github.com/risingpresage/speculative-decoding-lab) · [quant-quality-harness](https://github.com/risingpresage/quant-quality-harness) · [qwen-moe-stream](https://github.com/risingpresage/qwen-moe-stream)

## Upstream Open Source

37 pull requests across 18 repositories (8 merged), including [rerun-io/rerun #12943](https://github.com/rerun-io/rerun/pull/12943) and [stable-diffusion.cpp #2293](https://github.com/leejet/stable-diffusion.cpp/pull/2293), plus 14 CC0 compliance test datasets on [Hugging Face](https://huggingface.co/StanzaAPI).
