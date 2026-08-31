# Awesome Rust Agentics [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Building AI agents in Rust — frameworks, inference, MCP, and the crates that make it production-grade.

A curated list of Rust libraries and tools for agentic AI: agent frameworks, native LLM inference, model clients, Model Context Protocol, and the memory/RAG layer. Rust is the low-latency, memory-safe runtime for agents that run unattended — this is the ecosystem for building them.

## Contents

- [Agent Frameworks](#agent-frameworks)
- [LLM Inference & ML](#llm-inference--ml)
- [LLM Clients & Providers](#llm-clients--providers)
- [Model Context Protocol](#model-context-protocol)
- [Data, Memory & Vectors](#data-memory--vectors)
- [From Adventure Wave Labs](#from-adventure-wave-labs)
- [From Our Founder](#from-our-founder)
- [Learning](#learning)
- [Contributing](#contributing)

## Agent Frameworks

- [rig](https://github.com/0xplaygrounds/rig) - Modular, scalable LLM applications in Rust: unified interface across 20+ providers and 10+ vector stores, agentic workflows, multi-turn streaming, OpenTelemetry.
- [swiftide](https://github.com/bosun-ai/swiftide) - Fast, streaming indexing/query and agentic pipelines. Rust-native RAG plus tool-using, agent-calling agents.
- [AutoAgents](https://github.com/liquidos-ai/AutoAgents) - Multi-agent framework: type-safe agent model, structured tool calling, configurable memory, pluggable LLM backends.
- [goose](https://github.com/block/goose) - Extensible AI agent (Block → Linux Foundation): installs, executes, edits, tests with any LLM; 70+ MCP extensions. Rust, Apache-2.0.
- [floneum / kalosm](https://github.com/floneum/floneum) - Meta-framework for local pre-trained models: controlled generation, custom parsers, in-memory vector DB, built on candle.
- [ADK-Rust](https://github.com/zavora-ai/adk-rust) - Rust implementation of Google's Agent Development Kit: model-agnostic, LlmAgent / Sequential / Parallel / Loop agents, tools, MCP, memory, streaming, realtime voice.
- [kowalski](https://github.com/yarenty/kowalski) - Rust-native agentic framework built as a workspace (core, CLI, MCP crates) for distributed, federated agent systems.

## LLM Inference & ML

- [candle](https://github.com/huggingface/candle) - Hugging Face's minimalist ML framework for Rust. Fast CPU/GPU inference, runs Transformers in WASM at near-native speed.
- [m[mistral.rs](https://github.com/EricLBuehler/mistral.rs) - Fast, flexible inference across 40+ model families; OpenAI- and Anthropic-compatible APIs plus a built-in agentic loop (web search, code/shell execution, skills).
- [burn](https://github.com/tracel-ai/burn) - Next-generation tensor library and deep-learning framework; swap backends (CPU/CUDA/Metal/WGPU) without rewriting.
- [ort](https://github.com/pykeio/ort) - Hardware-accelerated inference & training for ONNX models in Rust; wrapper over Microsoft's ONNX Runtime.
- [llama-cpp-rs](https://github.com/utilityai/llama-cpp-rs) - Safe Rust bindings to llama.cpp for local GGUF inference on CPU/GPU.
- [tokenizers](https://github.com/huggingface/tokenizers) - Hugging Face's fast, production-grade tokenizers; the Rust core the wider HF ecosystem is built on.

## LLM Clients & Providers

- [genai](https://github.com/jeremychone/rust-genai) - Native-protocol multi-provider client: one API across 25+ providers (OpenAI, Anthropic, Gemini, Ollama, DeepSeek, xAI/Grok, Groq, Cohere, Bedrock, Vertex, and more).
- [async-openai](https://crates.io/crates/async-openai) - Ergonomic async OpenAI (and OpenAI-compatible) client; works against Ollama's OpenAI endpoint too.
- [ollama-rs](https://crates.io/crates/ollama-rs) - Local inference from Rust via Ollama — no API keys, no internet required.

## Model Context Protocol

- [rmcp (official Rust SDK)](https://github.com/modelcontextprotocol/rust-sdk) - The official Rust MCP SDK. Build clients and servers over multiple transports; Tokio-based, kept current by the MCP maintainers.
- [rust-mcp-sdk](https://github.com/rust-mcp-stack/rust-mcp-sdk) - High-performance, framework-agnostic MCP toolkit: stdio/Streamable HTTP/SSE transports, Axum and Actix integration, 100% official conformance-test pass rate.

## Data, Memory & Vectors

- [lancedb](https://github.com/lancedb/lancedb) - Embedded, serverless vector database that runs in-process — agent memory with no infrastructure (companion crate: rig-lancedb).
- [qdrant-client](https://github.com/qdrant/rust-client) - Official Rust client for the Qdrant vector search engine; rich payload filtering for RAG and long-term memory.
- [pgvector](https://github.com/pgvector/pgvector-rust) - Official Rust bindings for the pgvector Postgres extension; works with rust-postgres, SQLx, or Diesel for teams running vector search on Postgres they already operate.
- [safetensors](https://github.com/huggingface/safetensors) - Safe, fast, zero-copy tensor serialization (Rust core); the de-facto format for model weights.

## From Adventure Wave Labs

- [loopgen-rs](https://github.com/adventurewave-labs/loopgen-rs) - Agentic loop runner for Claude Code, in Rust.

## From Our Founder

Rust crates by [Marcus Patman](https://github.com/marcuspat), AWL's founder — personal projects, not AWL repos.

- [cargo-forge](https://github.com/marcuspat/cargo-forge) - Rust project generator / scaffolding CLI.
- [cargocrypt](https://github.com/marcuspat/cargocrypt) - Cryptography tooling in Rust.
- [netrain](https://github.com/marcuspat/netrain) - Rust network monitoring with a cinematic terminal UI.

## Learning

- [Rig docs](https://rig.rs/) - Guides and reference for the Rig framework.
- [Swiftide docs](https://swiftide.rs/) - Building fast, streaming LLM apps and agents in Rust.
- [Rust Ecosystem for AI & LLMs](https://hackmd.io/@Hamze/Hy5LiRV1gg) - A living map of the Rust AI/LLM crate landscape.

## Contributing

PRs welcome — one entry per PR, with a one-line reason it belongs here. Rust-first: the project should be a Rust crate/tool or have a first-class Rust interface. No unmaintained/archived projects, no dead links. See [CONTRIBUTING.md](CONTRIBUTING.md).

---

Maintained by [Adventure Wave Labs](https://github.com/adventurewave-labs) — founded by the creator of [turbo-flow](https://github.com/marcuspat/turbo-flow).
[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)
