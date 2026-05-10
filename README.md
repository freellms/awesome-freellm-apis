<p align="center">
  <h1 align="center">awesome-free-llm-apis</h1>
  <!-- AUTO_STATS -->
  <p align="center"><strong>128+ free LLM APIs from 17 providers</strong> — find, compare & configure free models in seconds.</p>
  <!-- END_AUTO_STATS -->
</p>

<p align="center">
  <a href="https://freellms.org"><strong>🌐 Live at freellms.org</strong></a> —
  <a href="https://freellms.org/models/">Browse models</a> ·
  <a href="https://freellms.org/playground/">Playground</a> ·
  <a href="https://freellms.org/config/">Config generator</a> ·
  <a href="https://freellms.org/free-llm-api-keys/">API keys</a>
</p>

---

## Why This Exists

Finding a free LLM API shouldn't mean hunting through a dozen GitHub READMEs, signing up for five different platforms, or guessing which models still have a free tier.

This repo is a **structured, machine-readable directory** of every free LLM API — rate limits, context windows, one-click config snippets, and direct API key links. Updated daily.

**The problem we solve:**

- ❌ You find a "free LLM API" list — it's 2 years old, half the links are dead
- ❌ You sign up for a provider — it silently requires a credit card, or worse, phone verification
- ❌ You finally get a key — your config tool (Claude Code, Cursor, Codex) needs a different format
- ❌ You want to compare two free models — you open 8 browser tabs of separate docs

**This repo + [freellms.org](https://freellms.org) fixes all of that.**

---

## Quick Start — Use Any Free API in 30 Seconds

All providers below expose an **OpenAI-compatible endpoint** (or, for Gemini, a trivial wrapper). That means any tool that accepts `baseURL` + `apiKey` works.

### Claude Code (cc)

```bash
export ANTHROPIC_BASE_URL="https://api.openai.com/v1"  # or Groq, OpenRouter, NVIDIA NIM
export ANTHROPIC_AUTH_TOKEN="your-api-key-here"
# Claude Code now routes through the free backend
```

### Cursor

```
Settings → Models → Add Model
  Model name: gpt-oss-120b
  Base URL: https://api.openai.com/v1
  API key: your-free-api-key
```

### Codex CLI

```bash
export OPENAI_BASE_URL="https://api.openai.com/v1"
export OPENAI_API_KEY="your-api-key-here"
```

### OpenAI SDK (Python)

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.openai.com/v1",  # swap to any provider below
    api_key="YOUR_FREE_API_KEY",
)

response = client.chat.completions.create(
    model="gpt-oss-120b",
    messages=[{"role": "user", "content": "Hello!"}],
)
print(response.choices[0].message.content)
```

> See [freellms.org/config/](https://freellms.org/config/) for ready-to-copy configs for Aider, Cline, OpenCode, Continue, Open WebUI, and Gemini CLI.

---

## Provider Directory

### ⚡ Permanent Free Tiers

These providers offer a **permanently free tier** — no credit card required for most.

<!-- BEGIN_PERMANENT_FREE -->
| Provider | Free Models | Credit Card? | Max Context | Modalities | Get API Key |
|---|---|---|---|---|---|
| NVIDIA NIM | 17 | Phone verification | 1,048,576 | text, image | [→](https://build.nvidia.com/settings/api-keys) |
| GitHub Models | 10 | No | 1,000,000 | text | [→](https://github.com/marketplace/models) |
| Groq | 9 | No | 262,000 | text | [→](https://console.groq.com/keys) |
| Cloudflare Workers AI | 8 | No | 10,000,000 | text, image | [→](https://dash.cloudflare.com/profile/api-tokens) |
| OVHcloud AI Endpoints | 7 | Registration | 262,000 | text, image, code | [→](https://endpoints.ai.cloud.ovh.net/) |
| Mistral AI | 6 | No | 256,000 | text, image, code | [→](https://console.mistral.ai/api-keys) |
| SiliconFlow | 6 | Registration | 131,072 | text | [→](https://cloud.siliconflow.cn/account/ak) |
| Cohere | 5 | No | 256,000 | text | [→](https://dashboard.cohere.com/api-keys) |
| Hugging Face | 5 | No | 131,000 | text | [→](https://huggingface.co/settings/tokens) |
| LLM7.io | 5 | No | 131,072 | text, code | [→](https://token.llm7.io) |
| Ollama Cloud | 5 | Registration | 128,000 | text | [→](https://ollama.com/settings/keys) |
| Cerebras | 4 | No | 131,000 | text | [→](https://cloud.cerebras.ai/) |
| Kilo Code | 4 | No | 262,000 | text, code | [→](https://kilo.ai) |
| Z AI (Zhipu) | 3 | No | 200,000 | text | [→](https://open.bigmodel.cn/usercenter/apikeys) |
| ModelScope | 3 | Registration | 131,072 | text | [→](https://modelscope.cn/my/myaccesstoken) |
| Google AI Studio | 2 | No | 1,000,000 | text, image, audio | [→](https://aistudio.google.com/app/apikey) |
<!-- END_PERMANENT_FREE -->

### 💰 Renewable Credits

Providers that periodically renew free credits.

| Provider | Free Models | Credit Model | Max Context | Modalities | Get API Key |
|---|---|---|---|---|---|
<!-- BEGIN_RENEWABLE -->
| OpenRouter | 29 | Free tier + $10 topup → 1K RPD | 1,048,756 | text, image, code, reasoning, embeddings, audio | [→](https://openrouter.ai/workspaces/default/keys) |
<!-- END_RENEWABLE -->

### 🖥️ Local / Self-Hosted (Unlimited, Private, Free Forever)

| Tool | Type | Highlights |
|---|---|---|
| [Ollama](https://ollama.com) | CLI + API | 100+ models, GPU acceleration, OpenAI-compatible endpoint |
| [LM Studio](https://lmstudio.ai) | Desktop GUI | Any GGUF model, built-in model browser, offline |
| [llama.cpp](https://github.com/ggerganov/llama.cpp) | C/C++ engine | Runs any GGUF, minimal dependencies |
| [GPT4All](https://gpt4all.io) | Desktop app | CPU-only, no GPU required, open source |
| [Jan.ai](https://jan.ai) | Desktop app | Privacy-focused, 100% offline ChatGPT alternative |
| [KoboldCpp](https://github.com/LostRuins/koboldcpp) | Single executable | Optimized for creative writing, GGUF |

---

## Top Free Models (by Weekly Usage)

Data from freellms.org, updated daily via API monitoring.

| Model | Provider | Context | Weekly Usage |
|---|---|---|---|
<!-- BEGIN_TOP_MODELS -->
| NVIDIA Nemotron 3 Super | OpenRouter | 262K | 585B tokens |
| Owl Alpha | OpenRouter | 1M | 375B tokens |
| Poolside Laguna M.1 | OpenRouter | 131K | 208B tokens |
| OpenAI gpt-oss-120b | OpenRouter | 131K | 144B tokens |
| inclusionAI Ring-2.6-1T | OpenRouter | 262K | 86B tokens |
| Z.ai GLM 4.5 Air | OpenRouter | 131K | 77B tokens |
| MiniMax M2.5 | OpenRouter | 197K | 57B tokens |
| NVIDIA Nemotron Nano 30B | OpenRouter | 256K | 41B tokens |
| OpenAI gpt-oss-20b | OpenRouter | 131K | 32B tokens |
| Poolside Laguna XS.2 | OpenRouter | 131K | 31B tokens |
<!-- END_TOP_MODELS -->

---

## Repository Structure

```
awesome-free-llm-apis/
├── README.md              ← Complete provider directory & code examples
├── code-examples/          ← Ready-to-use config snippets
│   ├── claude-code.md
│   ├── cursor.md
│   └── codex.md
└── LICENSE                 ← MIT
```

> For the full structured dataset with 453 models and daily updates, visit **[freellms.org](https://freellms.org)**.

---

## Contributing

We welcome contributions!

- **Add a missing free model** — Open an [issue](https://github.com/open-free-llm-api/awesome-free-llm-apis/issues) or submit a PR
- **Fix inaccurate data** — Rate limits change, providers graduate. PRs welcome
- **Add a config snippet** — Have a working config for a tool we don't cover? Add it to `code-examples/`

### Criteria for inclusion

A model belongs in this list if:
1. The provider explicitly offers a **free tier** (not just a trial credit)
2. The API is **publicly accessible** (no waitlist, closed beta, or reverse-engineering)
3. For trial credits: clearly labeled and minimum $1 credit value

---

## Links

- 🌐 **Live site**: [freellms.org](https://freellms.org) — search, compare, playground, config generator
- 🔑 **API key directory**: [freellms.org/free-llm-api-keys/](https://freellms.org/free-llm-api-keys/)
- ⚙️ **Config generator**: [freellms.org/config/](https://freellms.org/config/)
- 🎮 **Playground**: [freellms.org/playground/](https://freellms.org/playground/)
- 📊 **Compare models**: [freellms.org/compare/](https://freellms.org/compare/)

## License

MIT © [open-free-llm-api](https://github.com/open-free-llm-api)

---

<p align="center">
  <sub>Data refreshed daily via automated monitoring. <!-- AUTO_LAST_UPDATED -->Last updated: 2026-05-10<!-- END_AUTO_LAST_UPDATED -->.</sub>
</p>
