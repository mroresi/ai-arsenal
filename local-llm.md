# Local LLM

Local-first inference. Ollama already runs on whitebox (CPU-only, no GPU); the Mac mini has Apple silicon.

- [Ollama](https://github.com/ollama/ollama) - the front door: `ollama run <model>` and it serves. Already running on whitebox.
- huihui_ai/qwen3.5-abliterated - refusal-removed Qwen 3.5 via abliteration (real 2024 research technique). Install: `ollama run huihui_ai/qwen3.5-abliterated:9b` (about 6 GB download). Genuinely useful as a private brainstorming assistant. Keep it local-only; output quality trails properly tuned models, and an uncensored model is a responsibility, not just a feature.
- For the full engine and model matrix (llama.cpp, vLLM, LocalAI, LM Studio, Jan, GPT4All, whisper.cpp, mlx-lm), see [awesome-local-ai-2](https://github.com/marlburrow/awesome-local-ai-2) and [awesome-os-llm](https://github.com/townie/awesome-os-llm) in [awesome-lists.md](awesome-lists.md). No point duplicating them here.
- [VoiceStudio](https://github.com/debpalash/VoiceStudio) - fully local ElevenLabs alternative, 646 languages. Fits the local-first TTS and podcast needs.
