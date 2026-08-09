<p align="center">
  <h1 align="center">freellms</h1>
  <!-- AUTO_STATS -->
  <p align="center"><strong>424+ API LLM gratuitae ex XXX praebitoribus</strong> — exempla gratuita celeriter invenire, comparare, atque configurare potes.</p>
<!-- END_AUTO_STATS -->
</p>

<p align="center">
  <a href="https://freellms.org" target="_blank" rel="noopener"><strong>🌐 freellms.org visita</strong></a> —
  <a href="https://freellms.org/models/" target="_blank" rel="noopener">Modela explora</a> ·
  <a href="https://freellms.org/playground/" target="_blank" rel="noopener">Playground</a> ·
  <a href="https://freellms.org/config/" target="_blank" rel="noopener">Configuratorem</a> ·
  <a href="https://freellms.org/free-llm-api-keys/" target="_blank" rel="noopener">Claves API</a>
</p>

<p align="center">
  <img alt="Insignia praebitorum" src="assets/provider-logos-marquee.svg" width="100%" />
</p>

<!-- AUTO_UPDATE_BADGE -->
  <p align="center"><strong>🔄 Data cotidie renovata ex <a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a></strong> — Postrema renovatio: 2026-08-09</p>
<!-- END_AUTO_UPDATE_BADGE -->

<p align="center">
  🌐 <a href="README.md">English</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.zh-TW.md">繁體中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.es.md">Español</a> · <strong>Latine</strong>
</p>

---

## Cur hoc proiectum exstat

API LLM gratuitam invenire non debet multos README GitHub legere, rationes apud multas suggestiones creare, aut coniectare quae modela adhuc usum gratuitum habeant.

Hoc repositorium est **index ordinatus et machinis legibilis** API LLM gratuitarum: limites celeritatis, amplitudines contextus, fragmenta configurationis, et nexus directi ad claves API. Cotidie renovatur.

**Cur hoc repositorium et <a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a>:**

- ✅ **Semper recens** — data per inspectionem automatam cotidie renovata, non index staticus vetus
- ✅ **Perspicuitas chartarum creditarum** — clare ostendit qui praebitores chartam, probationem telephonicam, vel nihil requirant
- ✅ **Configurationes uno clic** — fragmenta parata pro Claude Code, Cursor, Codex, Aider, et pluribus instrumentis
- ✅ **Comparatio iuxta se** — contextus, limites celeritatis, et modalitates statim compara

---

## Quomodo uti — III gradus

1. **Praebitorem elige** — vide [Indicem praebitorum](#index-praebitorum). Incipe cum **Groq** (nulla charta creditoria, XXX RPM gratuita).
2. **Clavem API accipe** — preme quemlibet nexum [Clavem accipe →](#index-celer--url-bases-et-claves-api), rationem crea (plerumque epistula electronica sola sufficit), et clavem tuam exscribe. Minus quam minutum capit.
3. **Inserere** — URL basem et ID modeli exscribe, deinde in exempla [Initii celeris](#initium-celer--api-gratuita-intra-xxx-secundas-utere) infra insere.

Instrumentum singulare configurare vis? <a href="https://freellms.org/config/#claude-code" target="_blank" rel="noopener">Claude Code</a> · <a href="https://freellms.org/config/#cursor" target="_blank" rel="noopener">Cursor</a> · <a href="https://freellms.org/config/#codex" target="_blank" rel="noopener">Codex</a> · <a href="https://freellms.org/config/#openhuman" target="_blank" rel="noopener">OpenHuman</a> · <a href="https://freellms.org/config/#opencode" target="_blank" rel="noopener">OpenCode</a> · <a href="https://freellms.org/config/#openclaw" target="_blank" rel="noopener">OpenClaw</a> — configurationes uno clic in <a href="https://freellms.org/config/" target="_blank" rel="noopener">freellms.org/config/</a>.



## Initium celer — API gratuita intra XXX secundas utere

**Numquamne API usus es?** Facillima via est: ad <a href="https://console.groq.com/keys" target="_blank" rel="noopener">console.groq.com/keys</a> i, sola epistula electronica rationem crea (nulla charta creditoria), clavem gratuitam exscribe, et in quodlibet exemplum infra insere. Minus quam minuto operabitur.

Omnes praebitores infra **terminum cum OpenAI compatibilem** exhibent. Quodlibet instrumentum quod `baseURL` et `apiKey` accipit operatur: URL basem atque clavem tantum muta.
### Python (OpenAI SDK)

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.groq.com/openai/v1",  # gratuita, sine charta creditoria
    api_key="GROQ_API_KEY",                     # accipe in console.groq.com/keys
)

response = client.chat.completions.create(
    model="llama-3.3-70b-versatile",            # vide tabulam optimorum modelorum infra
    messages=[{"role": "user", "content": "Salve!"}],
)
print(response.choices[0].message.content)
# Gradus gratuitus Groq: XXX RPM, XIV 400 RPD — largus ad usum personalem
```

### Codex CLI

```bash
export OPENAI_BASE_URL="https://api.groq.com/openai/v1"
export OPENAI_API_KEY="clavis-tua-groq"        # accipe in console.groq.com/keys
codex --model "llama-3.3-70b-versatile"
```

### Cursor

```
Optiones → Modela → Modelum adde
  Nomen modeli: llama-3.3-70b-versatile
  URL basis: https://api.groq.com/openai/v1
  Clavis API: clavis-tua-groq                  # accipe in console.groq.com/keys
```

### Claude Code

```bash
# Claude Code API cum Anthropic compatibilem requirit; OpenRouter utere
export ANTHROPIC_BASE_URL="https://openrouter.ai/api"
export ANTHROPIC_AUTH_TOKEN="sk-or-v1-your-key"  # openrouter.ai/keys
export ANTHROPIC_API_KEY=""                       # must be empty
# Nota: modela Anthropic OpenRouter munus unicum decem dollariorum requirunt
```

### Aliis instrumentis uteris?

Plurima instrumenta evolutionis IA terminos API proprios accipiunt. Ea ad quemvis praebitorem superiorem dirige, deinde clavem gratuitam accipe:

- **Claude Code** — pone `ANTHROPIC_BASE_URL` et `ANTHROPIC_AUTH_TOKEN`. <a href="https://freellms.org/config/#claude-code" target="_blank" rel="noopener">Gradatim →</a>
- **Cursor** — Optiones → Modela → Modelum adde. <a href="https://freellms.org/config/#cursor" target="_blank" rel="noopener">Gradatim →</a>
- **Codex CLI** — pone `OPENAI_BASE_URL` et `OPENAI_API_KEY`. <a href="https://freellms.org/config/#codex" target="_blank" rel="noopener">Gradatim →</a>
- **OpenHuman** — `config.toml` edita. <a href="https://freellms.org/config/#openhuman" target="_blank" rel="noopener">Gradatim →</a>
- **Aider** — `.aider.conf.yml` edita. <a href="https://freellms.org/config/#aider" target="_blank" rel="noopener">Gradatim →</a>
- **Cline** (VS Code) — optiones praebitoris API. <a href="https://freellms.org/config/#cline" target="_blank" rel="noopener">Gradatim →</a>
- **Open WebUI** — Optiones → Coniunctiones. <a href="https://freellms.org/config/#open-webui" target="_blank" rel="noopener">Gradatim →</a>

Plures configurationes paratae ad exscribendum in <a href="https://freellms.org/config/" target="_blank" rel="noopener"><strong>freellms.org/config/</strong></a>.

> **Omnes praebitores, URL bases, et nexus clavium API** in [Indice celere](#index-celer--url-bases-et-claves-api) infra sunt.


---

## Index praebitorum

### ⚡ Gradus gratuiti perpetui

Hi praebitores **gradum gratuitum perpetuum** offerunt; plerique chartam creditoriam non requirunt.

<!-- BEGIN_PERMANENT_FREE -->
| Praebitor | Modela gratuita | Charta creditoria? | Contextus maximus | Modalitates | Clavem API accipe |
|---|---|---|---|---|---|
| NVIDIA NIM | 123 | Confirmatio telephonica | 1M | audio, embedding, image, reasoning, rerank, text, video, vision | <a href="https://build.nvidia.com/settings/api-keys" target="_blank" rel="noopener">→</a> |
| ModelScope | 55 | Adscriptio | 1M | audio, image, reasoning, text, video, vision | <a href="https://modelscope.cn/my/myaccesstoken" target="_blank" rel="noopener">→</a> |
| Cloudflare Workers AI | 39 | Non | 10M | code, image, reasoning, text, video | <a href="https://dash.cloudflare.com/profile/api-tokens" target="_blank" rel="noopener">→</a> |
| GitHub Models | 16 | Non | 1M | image, pdf, reasoning, text | <a href="https://github.com/marketplace/models" target="_blank" rel="noopener">→</a> |
| Google Gemini | 15 | Non | 1M | audio, image, pdf, reasoning, text, video, vision | <a href="https://aistudio.google.com/app/apikey" target="_blank" rel="noopener">→</a> |
| LLM7.io | 15 | Non | 1M | audio, code, image, pdf, reasoning, text, video, vision | <a href="https://token.llm7.io" target="_blank" rel="noopener">→</a> |
| OVHcloud AI Endpoints | 14 | Adscriptio | 262K | audio, code, image, reasoning, text, video | <a href="https://www.ovhcloud.com/en/public-cloud/ai-endpoints/catalog/" target="_blank" rel="noopener">→</a> |
| Groq | 12 | Non | 262K | image, reasoning, text | <a href="https://console.groq.com/keys" target="_blank" rel="noopener">→</a> |
| Mistral AI | 12 | Non | 256K | code, image, text | <a href="https://console.mistral.ai/api-keys" target="_blank" rel="noopener">→</a> |
| Cohere | 12 | Non | 436K | image, text | <a href="https://dashboard.cohere.com/api-keys" target="_blank" rel="noopener">→</a> |
| Kilo Code | 12 | Non | 1M | audio, code, image, reasoning, text, video | <a href="https://kilo.ai" target="_blank" rel="noopener">→</a> |
| Ollama Cloud | 9 | Adscriptio | 1M | code, image, reasoning, text, video | <a href="https://ollama.com/settings/keys" target="_blank" rel="noopener">→</a> |
| OpenCode Zen | 9 | Adscriptio | 1M | audio, reasoning, vision | <a href="https://opencode.ai/auth" target="_blank" rel="noopener">→</a> |
| Cerebras | 8 | Non | 131K | image, reasoning, text | <a href="https://cloud.cerebras.ai/" target="_blank" rel="noopener">→</a> |
| Aion Labs | 7 | Adscriptio | 131K | text | <a href="https://www.aionlabs.ai" target="_blank" rel="noopener">→</a> |
| Hugging Face | 7 | Non | 131K | code, text | <a href="https://huggingface.co/settings/tokens" target="_blank" rel="noopener">→</a> |
| Agnes AI | 5 | Adscriptio | 256K | image, text, video, vision | <a href="https://platform.agnes-ai.com/settings/apiKeys" target="_blank" rel="noopener">→</a> |
| Alibaba Cloud Model Studio | 5 | Adscriptio | 1M | code, image, text | <a href="https://bailian.console.alibabacloud.com/?apiKey=1" target="_blank" rel="noopener">→</a> |
| Z AI (Zhipu AI) | 4 | Non | 200K | image, reasoning, text, video | <a href="https://open.bigmodel.cn/usercenter/apikeys" target="_blank" rel="noopener">→</a> |
| SambaNova | 4 | Adscriptio | 128K | image, reasoning, text | <a href="https://cloud.sambanova.ai/apis" target="_blank" rel="noopener">→</a> |
| SiliconFlow | 3 | Adscriptio | 131K | text | <a href="https://cloud.siliconflow.cn/account/ak" target="_blank" rel="noopener">→</a> |
| xAI | 3 | Adscriptio | 2M | text | <a href="https://console.x.ai" target="_blank" rel="noopener">→</a> |
| Chutes.ai | 2 | Adscriptio | 131K | reasoning, text | <a href="https://chutes.ai/" target="_blank" rel="noopener">→</a> |
| Glhf.chat | 2 | Adscriptio | 131K | text | <a href="https://glhf.chat/" target="_blank" rel="noopener">→</a> |
| Grok (xAI) | 2 | Adscriptio | 131K | text | <a href="https://console.x.ai/" target="_blank" rel="noopener">→</a> |
| AI21 Labs | 2 | Adscriptio | 256K | text | <a href="https://studio.ai21.com/account/api-key" target="_blank" rel="noopener">→</a> |
| DeepSeek | 2 | Adscriptio | 128K | text | <a href="https://platform.deepseek.com/api_keys" target="_blank" rel="noopener">→</a> |
| Nscale | 2 | Adscriptio | 128K | text | <a href="https://console.nscale.com/" target="_blank" rel="noopener">→</a> |
| Nebius | 1 | Adscriptio | 128K | text | <a href="https://studio.nebius.com/settings/api-keys" target="_blank" rel="noopener">→</a> |
<!-- END_PERMANENT_FREE -->

### 💰 Credita renovabilia

Praebitores qui credita gratuita temporibus certis renovant.

<!-- BEGIN_RENEWABLE -->
| Praebitor | Modela gratuita | Modus crediti | Contextus maximus | Modalitates | Clavem API accipe |
|---|---|---|---|---|---|
| OpenRouter | 22 | Gradus gratuitus + $10 topup → 1K RPD | 1M | audio, code, embeddings, image, reasoning, rerank, speech, text, video | <a href="https://openrouter.ai/workspaces/default/keys" target="_blank" rel="noopener">→</a> |
<!-- END_RENEWABLE -->

## Index celer — URL bases et claves API

<!-- BEGIN_QUICK_REF -->
| Praebitor | URL basis | Clavem API accipe | Charta creditoria? |
|---|---|---|---|
| NVIDIA NIM | `https://integrate.api.nvidia.com/v1` | <a href="https://build.nvidia.com/settings/api-keys" target="_blank" rel="noopener">Clavem accipe →</a> | Confirmatio telephonica |
| ModelScope | `https://api-inference.modelscope.cn/v1` | <a href="https://modelscope.cn/my/myaccesstoken" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Cloudflare Workers AI | `https://api.cloudflare.com/client/v4/accounts/{account_id}/ai/run` | <a href="https://dash.cloudflare.com/profile/api-tokens" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| OpenRouter | `https://openrouter.ai/api/v1` | <a href="https://openrouter.ai/workspaces/default/keys" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| GitHub Models | `https://models.github.ai/inference` | <a href="https://github.com/marketplace/models" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Google Gemini | `https://generativelanguage.googleapis.com/v1beta` | <a href="https://aistudio.google.com/app/apikey" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| LLM7.io | `https://api.llm7.io/v1` | <a href="https://token.llm7.io" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| OVHcloud AI Endpoints | `https://oai.endpoints.kepler.ai.cloud.ovh.net/v1` | <a href="https://www.ovhcloud.com/en/public-cloud/ai-endpoints/catalog/" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Groq | `https://api.groq.com/openai/v1` | <a href="https://console.groq.com/keys" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Mistral AI | `https://api.mistral.ai/v1` | <a href="https://console.mistral.ai/api-keys" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Cohere | `https://api.cohere.com/v2` | <a href="https://dashboard.cohere.com/api-keys" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Kilo Code | `https://api.kilo.ai/api/gateway` | <a href="https://kilo.ai" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Ollama Cloud | `https://api.ollama.com` | <a href="https://ollama.com/settings/keys" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| OpenCode Zen | `https://opencode.ai/zen/v1` | <a href="https://opencode.ai/auth" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Cerebras | `https://api.cerebras.ai/v1` | <a href="https://cloud.cerebras.ai/" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Aion Labs | `https://api.aionlabs.ai/v1` | <a href="https://www.aionlabs.ai" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Hugging Face | `https://router.huggingface.co/v1` | <a href="https://huggingface.co/settings/tokens" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| Agnes AI | `https://apihub.agnes-ai.com/v1` | <a href="https://platform.agnes-ai.com/settings/apiKeys" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Alibaba Cloud Model Studio | `https://dashscope-intl.aliyuncs.com/compatible-mode/v1` | <a href="https://bailian.console.alibabacloud.com/?apiKey=1" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Z AI (Zhipu AI) | `https://open.bigmodel.cn/api/paas/v4` | <a href="https://open.bigmodel.cn/usercenter/apikeys" target="_blank" rel="noopener">Clavem accipe →</a> | Non |
| SambaNova | `https://api.sambanova.ai/v1` | <a href="https://cloud.sambanova.ai/apis" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| SiliconFlow | `https://api.siliconflow.cn/v1` | <a href="https://cloud.siliconflow.cn/account/ak" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| xAI | `https://api.x.ai/v1` | <a href="https://console.x.ai" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Chutes.ai | `https://api.chutes.ai/v1` | <a href="https://chutes.ai/" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Glhf.chat | `https://glhf.chat/api/openai/v1` | <a href="https://glhf.chat/" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Grok (xAI) | `https://api.x.ai/v1` | <a href="https://console.x.ai/" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| AI21 Labs | `https://api.ai21.com/studio/v1` | <a href="https://studio.ai21.com/account/api-key" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| DeepSeek | `https://api.deepseek.com/v1` | <a href="https://platform.deepseek.com/api_keys" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Nscale | `https://inference.api.nscale.com/v1` | <a href="https://console.nscale.com/" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
| Nebius | `https://api.studio.nebius.com/v1` | <a href="https://studio.nebius.com/settings/api-keys" target="_blank" rel="noopener">Clavem accipe →</a> | Adscriptio |
<!-- END_QUICK_REF -->

## Optima modela gratuita per praebitorem

<!-- BEGIN_BEST_MODELS -->
| Praebitor | Optimum modelum gratuitum | ID modeli | Contextus maximus | Limes celeritatis |
|---|---|---|---|---|
| NVIDIA NIM | <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-2/" target="_blank" rel="noopener">z-ai/glm-5.2</a> | `z-ai/glm-5.2` | 1M | Usque ad 40 RPM |
|  | <a href="https://freellms.org/models/nvidia-nim/poolside-laguna-xs-2-1/" target="_blank" rel="noopener">poolside/laguna-xs-2.1</a> | `poolside/laguna-xs-2.1` | 262K | Usque ad 40 RPM |
|  | <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-1/" target="_blank" rel="noopener">z-ai/glm-5.1</a> | `z-ai/glm-5.1` | 202K | Usque ad 40 RPM |
| ModelScope | <a href="https://freellms.org/models/modelscope/minimax-minimax-m2-5/" target="_blank" rel="noopener">MiniMax-M2.5-highspeed</a> | `MiniMax/MiniMax-M2.5` | 204K | Vide praebitorem |
|  | <a href="https://freellms.org/models/modelscope/qwen-qwen3-5-35b-a3b/" target="_blank" rel="noopener">Qwen/Qwen3.5-35B-A3B</a> | `qwen-qwen3-5-35b-a3b` | 131K | 2,000 RPD in summa; <=500 .. |
|  | <a href="https://freellms.org/models/modelscope/qwen-qwen3-5-27b/" target="_blank" rel="noopener">Qwen/Qwen3.5-27B</a> | `qwen-qwen3-5-27b` | 131K | 2,000 RPD in summa; <=500 .. |
| Cloudflare Workers AI | <a href="https://freellms.org/models/cloudflare-workers-ai/mistral-mistral-7b-instruct-v0-1/" target="_blank" rel="noopener">Mistral 7B</a> | `@cf/mistral/mistral-7b-instruct-v0.1` | 32K | Vide praebitorem |
|  | <a href="https://freellms.org/models/cloudflare-workers-ai/qwen-qwen1-5-7b-chat/" target="_blank" rel="noopener">Qwen 1.5 7B</a> | `@cf/qwen/qwen1.5-7b-chat` | 32K | Vide praebitorem |
|  | <a href="https://freellms.org/models/cloudflare-workers-ai/cf-meta-llama-3-3-70b-instruct-fp8-fast/" target="_blank" rel="noopener">@cf/meta/llama-3.3-70b-instruct-fp8-fast</a> | `@cf/meta/llama-3.3-70b-instruct-fp8-fast` | 131K | 10K neuronae/die (communis) |
| OpenRouter | <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-ultra-550b-a55b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Ultra (gratuitum)</a> | `nvidia/nemotron-3-ultra-550b-a55b:free` | 1M | Vide praebitorem |
|  | <a href="https://freellms.org/models/openrouter/poolside-laguna-m-1/" target="_blank" rel="noopener">Poolside: Laguna M.1 (gratuitum)</a> | `poolside/laguna-m.1:free` | 262K | Vide praebitorem |
|  | <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-super-120b-a12b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Super (gratuitum)</a> | `nvidia/nemotron-3-super-120b-a12b:free` | 262K | Vide praebitorem |
| GitHub Models | <a href="https://freellms.org/models/github-models/phi-4/" target="_blank" rel="noopener">Phi-4</a> | `Phi-4` | 131K | Vide praebitorem |
|  | <a href="https://freellms.org/models/github-models/mistral-large-2411/" target="_blank" rel="noopener">Mistral Large (24.11)</a> | `Mistral-large-2411` | 131K | Vide praebitorem |
|  | <a href="https://freellms.org/models/github-models/ai21-jamba-1-5-large/" target="_blank" rel="noopener">AI21 Jamba 1.5 Large</a> | `AI21-Jamba-1.5-Large` | 256K | Vide praebitorem |
| Google Gemini | <a href="https://freellms.org/models/google-gemini/gemini-3-6-flash/" target="_blank" rel="noopener">Gemini 3.6 Flash</a> | `gemini-3.6-flash` | 1M | 15 RPM, 1,500 RPD |
|  | <a href="https://freellms.org/models/google-gemini/gemini-3-5-flash/" target="_blank" rel="noopener">Gemini 3.5 Flash</a> | `gemini-3.5-flash` | 1M | 15 RPM, 1,500 RPD |
|  | <a href="https://freellms.org/models/google-gemini/gemini-3-5-flash-lite/" target="_blank" rel="noopener">Gemini 3.5 Flash-Lite</a> | `gemini-3.5-flash-lite` | 1M | 30 RPM, 1,500 RPD |
| LLM7.io | <a href="https://freellms.org/models/llm7-io/deepseek-r1-0528/" target="_blank" rel="noopener">deepseek-r1-0528</a> | `deepseek-r1-0528` | 131K | 30 RPM (120 cum tessera) |
|  | <a href="https://freellms.org/models/llm7-io/deepseek-v3-0324/" target="_blank" rel="noopener">deepseek-v3-0324</a> | `deepseek-v3-0324` | 131K | 30 RPM (120 cum tessera) |
|  | <a href="https://freellms.org/models/llm7-io/gpt-4o-mini/" target="_blank" rel="noopener">gpt-4o-mini</a> | `gpt-4o-mini` | 131K | 30 RPM (120 cum tessera) |
| OVHcloud AI Endpoints | <a href="https://freellms.org/models/ovhcloud-ai-endpoints/qwen3-5-397b-a17b/" target="_blank" rel="noopener">Qwen3.5-397B-A17B</a> | `qwen3.5-397b-a17b` | 131K | 2 RPM (anonymus) |
|  | <a href="https://freellms.org/models/ovhcloud-ai-endpoints/meta-llama-3-3-70b-instruct/" target="_blank" rel="noopener">Meta-Llama-3_3-70B-Instruct</a> | `meta-llama-3_3-70b-instruct` | 131K | 2 RPM (anonymus) |
|  | <a href="https://freellms.org/models/ovhcloud-ai-endpoints/qwen3-6-27b/" target="_blank" rel="noopener">Qwen3.6-27B</a> | `qwen3.6-27b` | 131K | 2 RPM (anonymus) |
| Groq | <a href="https://freellms.org/models/groq/moonshotai-kimi-k2-instruct/" target="_blank" rel="noopener">Moonshot Kimi K2</a> | `moonshotai/kimi-k2-instruct` | 131K | Vide praebitorem |
|  | <a href="https://freellms.org/models/groq/moonshotai-kimi-k2-instruct-0905/" target="_blank" rel="noopener">Moonshot Kimi K2 0905</a> | `moonshotai/kimi-k2-instruct-0905` | 131K | Vide praebitorem |
|  | <a href="https://freellms.org/models/groq/groq-compound/" target="_blank" rel="noopener">groq/compound</a> | `groq/compound` | 131K | 30 RPM, 250 RPD |
| Mistral AI | <a href="https://freellms.org/models/mistral-ai/open-mistral-7b/" target="_blank" rel="noopener">Mistral 7B</a> | `open-mistral-7b` | 32K | Vide praebitorem |
|  | <a href="https://freellms.org/models/mistral-ai/open-mixtral-8x7b/" target="_blank" rel="noopener">Mixtral 8x7B</a> | `open-mixtral-8x7b` | 32K | Vide praebitorem |
|  | <a href="https://freellms.org/models/mistral-ai/mistral-medium-3-5-128b/" target="_blank" rel="noopener">Mistral Medium 3.5 (128B)</a> | `mistral-medium-3-5-128b` | 256K | ~1 RPS, 500K TPM |
| Cohere | <a href="https://freellms.org/models/cohere/command-a-218b/" target="_blank" rel="noopener">Command A+ (218B)</a> | `command-a-218b` | 436K | 20 RPM |
|  | <a href="https://freellms.org/models/cohere/command-a-111b/" target="_blank" rel="noopener">Command A (111B)</a> | `command-a-111b` | 288K | 20 RPM |
|  | <a href="https://freellms.org/models/cohere/command-r/" target="_blank" rel="noopener">Command R+</a> | `command-r` | 128K | 20 RPM |
| Kilo Code | <a href="https://freellms.org/models/kilo-code/nvidia-nemotron-3-ultra-550b-a55b-free/" target="_blank" rel="noopener">nvidia/nemotron-3-ultra-550b-a55b:free</a> | `nvidia/nemotron-3-ultra-550b-a55b:free` | 1M | ~200 req/hr |
|  | <a href="https://freellms.org/models/kilo-code/stepfun-step-3-7-flash-free/" target="_blank" rel="noopener">stepfun/step-3.7-flash:free</a> | `stepfun/step-3.7-flash:free` | 262K | ~200 req/hr |
|  | <a href="https://freellms.org/models/kilo-code/nvidia-nemotron-3-super-120b-a12b-free/" target="_blank" rel="noopener">nvidia/nemotron-3-super-120b-a12b:free</a> | `nvidia/nemotron-3-super-120b-a12b:free` | 262K | ~200 req/hr |
| Ollama Cloud | <a href="https://freellms.org/models/ollama-cloud/minimax-m3/" target="_blank" rel="noopener">minimax-m3</a> | `minimax-m3` | 1M | Limites sessionis vel hebdomadales (.. |
|  | <a href="https://freellms.org/models/ollama-cloud/gpt-oss-20b/" target="_blank" rel="noopener">gpt-oss:20b</a> | `gpt-oss:20b` | 131K | Limites sessionis vel hebdomadales (.. |
|  | <a href="https://freellms.org/models/ollama-cloud/nemotron-3-ultra/" target="_blank" rel="noopener">nemotron-3-ultra</a> | `nemotron-3-ultra` | 262K | Limites sessionis vel hebdomadales (.. |
| OpenCode Zen | <a href="https://freellms.org/models/opencode/big-pickle/" target="_blank" rel="noopener">big-pickle</a> | `big-pickle` | 0 |  |
|  | <a href="https://freellms.org/models/opencode/deepseek-v4-flash-free/" target="_blank" rel="noopener">DeepSeek V4 Flash</a> | `deepseek-v4-flash-free` | 1M |  |
|  | <a href="https://freellms.org/models/opencode/mimo-v2-5-free/" target="_blank" rel="noopener">MiMo-V2.5</a> | `mimo-v2.5-free` | 1M |  |
| Cerebras | <a href="https://freellms.org/models/cerebras/llama3-1-70b/" target="_blank" rel="noopener">Llama 3.1 70B</a> | `llama3.1-70b` | 131K | Vide praebitorem |
|  | <a href="https://freellms.org/models/cerebras/gpt-oss-120b/" target="_blank" rel="noopener">gpt-oss-120b</a> | `gpt-oss-120b` | 131K | 5 RPM, 30K TPM, 1M TPD |
|  | <a href="https://freellms.org/models/cerebras/zai-glm-4-7-deprecated-aug-2026/" target="_blank" rel="noopener">zai-glm-4.7 (deprecated Aug 2026)</a> | `zai-glm-4.7` | 131K | 5 RPM, 30K TPM, 1M TPD |
| Aion Labs | <a href="https://freellms.org/models/aion-labs/aion-2-5/" target="_blank" rel="noopener">Aion 2.5</a> | `aion-2-5` | 128K | 15 RPM, 20K TPD |
|  | <a href="https://freellms.org/models/aion-labs/aion-2-0/" target="_blank" rel="noopener">Aion 2.0</a> | `aion-2-0` | 128K | 15 RPM, 20K TPD |
|  | <a href="https://freellms.org/models/aion-labs/aion-rp-1-0-8b/" target="_blank" rel="noopener">Aion-RP 1.0 (8B)</a> | `aion-rp-1-0-8b` | 32K | 15 RPM, 20K TPD |
| Hugging Face | <a href="https://freellms.org/models/hugging-face/meta-llama-3-1-8b-instruct/" target="_blank" rel="noopener">Meta-Llama-3.1-8B-Instruct</a> | `meta-llama-3-1-8b-instruct` | 128K | Creditis mensuratum |
|  | <a href="https://freellms.org/models/hugging-face/gemma-3-4b-it/" target="_blank" rel="noopener">gemma-3-4b-it</a> | `gemma-3-4b-it` | 131K | Creditis mensuratum |
|  | <a href="https://freellms.org/models/hugging-face/qwen2-5-coder-7b-instruct/" target="_blank" rel="noopener">Qwen2.5-Coder-7B-Instruct</a> | `qwen2-5-coder-7b-instruct` | 131K | Creditis mensuratum |
| Agnes AI | <a href="https://freellms.org/models/agnes-ai/agnes-1-5-flash/" target="_blank" rel="noopener">agnes-1.5-flash</a> | `agnes-1.5-flash` | 256K | 30 RPM |
|  | <a href="https://freellms.org/models/agnes-ai/agnes-2-0-flash/" target="_blank" rel="noopener">agnes-2.0-flash</a> | `agnes-2.0-flash` | 256K | 30 RPM |
|  | <a href="https://freellms.org/models/agnes-ai/agnes-image-2-0-flash/" target="_blank" rel="noopener">agnes-image-2.0-flash</a> | `agnes-image-2.0-flash` | 4K | 30 RPM (1K) |
| Alibaba Cloud Model Studio | <a href="https://freellms.org/models/alibaba-cloud-model-studio/qwen3-max/" target="_blank" rel="noopener">Qwen3-Max</a> | `qwen3-max` | 128K | Pro gradu et regione |
|  | <a href="https://freellms.org/models/alibaba-cloud-model-studio/qwen3-plus/" target="_blank" rel="noopener">Qwen3-Plus</a> | `qwen3-plus` | 1M | Pro gradu et regione |
|  | <a href="https://freellms.org/models/alibaba-cloud-model-studio/qwen3-vl-plus/" target="_blank" rel="noopener">Qwen3-VL-Plus</a> | `qwen3-vl-plus` | 128K | Pro gradu et regione |
| Z AI (Zhipu AI) | <a href="https://freellms.org/models/z-ai-zhipu-ai/glm-4-7-flash/" target="_blank" rel="noopener">GLM-4.7-Flash</a> | `glm-4.7` | 200K | 1 petitio simul |
|  | <a href="https://freellms.org/models/z-ai-zhipu-ai/glm-4-5-flash/" target="_blank" rel="noopener">GLM-4.5-Flash</a> | `glm-4.5` | 128K | 1 petitio simul |
|  | <a href="https://freellms.org/models/z-ai-zhipu-ai/glm-4-6v-flash/" target="_blank" rel="noopener">GLM-4.6V-Flash</a> | `glm-4.6` | 128K | 1 petitio simul |
| SambaNova | <a href="https://freellms.org/models/sambanova/deepseek-v3-1/" target="_blank" rel="noopener">DeepSeek-V3.1</a> | `deepseek-v3-1` | 128K | 20 RPM, 20 RPD, 200K TPD |
|  | <a href="https://freellms.org/models/sambanova/deepseek-v3-2-preview/" target="_blank" rel="noopener">DeepSeek-V3.2 (Praevisum)</a> | `deepseek-v3-2-preview` | 128K | 20 RPM, 20 RPD, 200K TPD |
|  | <a href="https://freellms.org/models/sambanova/minimax-m2-7/" target="_blank" rel="noopener">MiniMax-M2.7</a> | `minimax-m2-7` | 128K | 20 RPM, 20 RPD, 200K TPD |
| SiliconFlow | <a href="https://freellms.org/models/siliconflow/deepseek-ai-deepseek-r1-distill-qwen-7b/" target="_blank" rel="noopener">deepseek-ai/DeepSeek-R1-Distill-Qwen-7B</a> | `deepseek-ai-deepseek-r1-distill-qwen-7b` | 131K | 30 RPM, 60K TPM |
|  | <a href="https://freellms.org/models/siliconflow/abbreviation/" target="_blank" rel="noopener">Abbreviation</a> | `abbreviation` | 131K | Vide praebitorem |
|  | <a href="https://freellms.org/models/siliconflow/deepseek-ai-deepseek-ocr/" target="_blank" rel="noopener">deepseek-ai/DeepSeek-OCR</a> | `deepseek-ai-deepseek-ocr` | 131K | 30 RPM, 60K TPM |
| xAI | <a href="https://freellms.org/models/xai/grok-4-3/" target="_blank" rel="noopener">grok-4.3</a> | `grok-4-3` | 1M | Creditis fundatum |
|  | <a href="https://freellms.org/models/xai/grok-4-1-fast/" target="_blank" rel="noopener">grok-4.1-fast</a> | `grok-4-1-fast` | 2M | Creditis fundatum |
|  | <a href="https://freellms.org/models/xai/grok-3-mini/" target="_blank" rel="noopener">grok-3-mini</a> | `grok-3-mini` | 131K | Creditis fundatum |
| Chutes.ai | <a href="https://freellms.org/models/chutes-ai/deepseek-ai-deepseek-r1/" target="_blank" rel="noopener">DeepSeek-R1</a> | `deepseek-ai/DeepSeek-R1` | 131K | Communitate sustentatum, sine h... |
|  | <a href="https://freellms.org/models/chutes-ai/meta-llama-meta-llama-3-1-70b-instruct/" target="_blank" rel="noopener">Llama 3.1 70B</a> | `meta-llama/Meta-Llama-3.1-70B-Instruct` | 131K | Communitate sustentatum, sine h... |
| Glhf.chat | <a href="https://freellms.org/models/glhf-chat/meta-llama-meta-llama-3-1-70b-instruct-2/" target="_blank" rel="noopener">Llama 3.1 70B</a> | `meta-llama/Meta-Llama-3.1-70B-Instruct` | 131K | Sine limite pro modelis gratuitis |
|  | <a href="https://freellms.org/models/glhf-chat/mistralai-mixtral-8x7b-instruct-v0-1/" target="_blank" rel="noopener">Mixtral 8x7B</a> | `mistralai/Mixtral-8x7B-Instruct-v0.1` | 32K | Sine limite pro modelis gratuitis |
| Grok (xAI) | <a href="https://freellms.org/models/grok-(xai)/grok-2/" target="_blank" rel="noopener">Grok-2</a> | `grok-2` | 131K | 25 dollaria/mense credita gratuita,.. |
|  | <a href="https://freellms.org/models/grok-(xai)/grok-2-mini/" target="_blank" rel="noopener">Grok-2 Mini</a> | `grok-2-mini` | 131K | 25 dollaria/mense credita gratuita,.. |
| AI21 Labs | <a href="https://freellms.org/models/ai21-labs/jamba-large-1-7/" target="_blank" rel="noopener">Jamba Large 1.7</a> | `jamba-large-1-7` | 256K | 200 RPM, 10 RPS |
|  | <a href="https://freellms.org/models/ai21-labs/jamba-mini-2/" target="_blank" rel="noopener">Jamba Mini 2</a> | `jamba-mini-2` | 256K | 200 RPM, 10 RPS |
| DeepSeek | <a href="https://freellms.org/models/deepseek/deepseek-chat-v3-2/" target="_blank" rel="noopener">deepseek-chat (V3.2)</a> | `deepseek-chat-v3-2` | 128K | Dynamicum |
|  | <a href="https://freellms.org/models/deepseek/deepseek-reasoner-r1/" target="_blank" rel="noopener">deepseek-reasoner (R1)</a> | `deepseek-reasoner-r1` | 128K | Dynamicum |
| Nscale | <a href="https://freellms.org/models/nscale/llama-3-3-70b-instruct/" target="_blank" rel="noopener">Llama-3.3-70B-Instruct</a> | `llama-3-3-70b-instruct` | 128K | Usus aequus |
|  | <a href="https://freellms.org/models/nscale/deepseek-r1-distill-llama-70b/" target="_blank" rel="noopener">DeepSeek-R1-Distill-Llama-70B</a> | `deepseek-r1-distill-llama-70b` | 128K | Usus aequus |
| Nebius | <a href="https://freellms.org/models/nebius/qwen3-235b-a22b/" target="_blank" rel="noopener">Qwen3-235B-A22B</a> | `qwen3-235b-a22b` | 128K | Pro gradu |
<!-- END_BEST_MODELS -->



### 🖥️ Localia vel a se administrata (sine limite, privata, perpetuo gratuita)

| Instrumentum | Genus | Praecipua |
|---|---|---|
| <a href="https://ollama.com" target="_blank" rel="noopener">Ollama</a> | CLI + API | Plus quam 100 modela, acceleratio GPU, terminus cum OpenAI compatibilis |
| <a href="https://lmstudio.ai" target="_blank" rel="noopener">LM Studio</a> | GUI escritorio | Quodlibet modelum GGUF, navigator internus, sine conexu |
| <a href="https://github.com/ggerganov/llama.cpp" target="_blank" rel="noopener">llama.cpp</a> | Machina C/C++ | Quodlibet GGUF exsequitur, paucis dependentis |
| <a href="https://gpt4all.io" target="_blank" rel="noopener">GPT4All</a> | Applicatio escritorio | Solum CPU, GPU non requirit, fons apertus |
| <a href="https://jan.ai" target="_blank" rel="noopener">Jan.ai</a> | Applicatio escritorio | Privatum, ChatGPT substitutum omnino locale |
| <a href="https://github.com/LostRuins/koboldcpp" target="_blank" rel="noopener">KoboldCpp</a> | Exsecutabile unum | Ad scripturam creativam et GGUF optimizatum |

---

## Praecipua modela gratuita (usu hebdomadali)

Data ex freellms.org, cotidie per inspectionem API renovata.

<!-- BEGIN_TOP_MODELS -->
| Modelum | Praebitor | Contextus | Usus hebdomadalis |
|---|---|---|---|
| <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-2/" target="_blank" rel="noopener">z-ai/glm-5.2</a> | NVIDIA NIM | 1M | 2998B tokens |
| <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-ultra-550b-a55b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Ultra (gratuitum)</a> | OpenRouter | 1M | 2326B tokens |
| <a href="https://freellms.org/models/openrouter/poolside-laguna-m-1/" target="_blank" rel="noopener">Poolside: Laguna M.1 (gratuitum)</a> | OpenRouter | 262K | 768B tokens |
| <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-super-120b-a12b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Super (gratuitum)</a> | OpenRouter | 262K | 315B tokens |
| <a href="https://freellms.org/models/openrouter/cohere-north-mini-code/" target="_blank" rel="noopener">Cohere: North Mini Code (gratuitum)</a> | OpenRouter | 256K | 255B tokens |
| <a href="https://freellms.org/models/nvidia-nim/poolside-laguna-xs-2-1/" target="_blank" rel="noopener">poolside/laguna-xs-2.1</a> | NVIDIA NIM | 262K | 171B tokens |
| <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-1/" target="_blank" rel="noopener">z-ai/glm-5.1</a> | NVIDIA NIM | 202K | 158B tokens |
| <a href="https://freellms.org/models/openrouter/poolside-laguna-s-2-1/" target="_blank" rel="noopener">Poolside: Laguna S 2.1 (gratuitum)</a> | OpenRouter | 262K | 83B tokens |
| <a href="https://freellms.org/models/openrouter/poolside-laguna-xs-2-1/" target="_blank" rel="noopener">Poolside: Laguna XS 2.1 (gratuitum)</a> | OpenRouter | 262K | 81B tokens |
| <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-nano-30b-a3b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Nano 30B A3B (gratuitum)</a> | OpenRouter | 256K | 45B tokens |
<!-- END_TOP_MODELS -->

---

## Structura repositorii

```
freellms/
├── README.md              ← Index plenus praebitorum et exempla codicis
├── code-examples/          ← Fragmenta configurationis parata ad usum
│   ├── claude-code.md
│   ├── cursor.md
│   └── codex.md
└── LICENSE                 ← MIT
```

> Pro indice structo pleno cum 453 modelis et renovationibus cotidianis, **<a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a>** visita.

---

## Conlationes

Conlationes libenter accipimus!

- **Modelum gratuitum omissum adde** — Aperi <a href="https://github.com/freellms/freellms/issues" target="_blank" rel="noopener">quaestionem</a> aut PR mitte
- **Data falsa corrige** — Limites mutantur et praebitores gradus suos mutant. PR gratae sunt
- **Fragmentum configurationis adde** — Configurationem operantem habes? Ad `code-examples/` adde

### Norma inclusionis

Modelum huic indice pertinet si:
1. Praebitor explicite **gradum gratuitum** offert (non solum creditum probationis)
2. API est **publice accessibilis** (sine indice exspectationis, beta clausa, aut inversione technica)
3. Pro creditis probationis: clare signata sunt et valorem minimum unius dollarii habent

---

## Nexus

- 🌐 **Situs**: <a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a> — quaere, compara, experire et configura
- 🔑 **Index clavium API**: <a href="https://freellms.org/free-llm-api-keys/" target="_blank" rel="noopener">freellms.org/free-llm-api-keys/</a>
- ⚙️ **Configurator**: <a href="https://freellms.org/config/" target="_blank" rel="noopener">freellms.org/config/</a>
- 🎮 **Experimentum**: <a href="https://freellms.org/playground/" target="_blank" rel="noopener">freellms.org/playground/</a>
- 📊 **Modela compara**: <a href="https://freellms.org/compare/" target="_blank" rel="noopener">freellms.org/compare/</a>

## Licentia

MIT © <a href="https://github.com/freellms" target="_blank" rel="noopener">freellms</a>

---

<p align="center">
  <sub>Postrema renovatio: <!-- AUTO_LAST_UPDATED -->
2026-08-09
<!-- END_AUTO_LAST_UPDATED --></sub>
</p>
