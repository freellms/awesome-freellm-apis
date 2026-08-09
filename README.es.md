<p align="center">
  <h1 align="center">freellms</h1>
  <!-- AUTO_STATS -->
  <p align="center"><strong>424+ API de LLM gratuitas de 30 proveedores</strong> — encuentra, compara y configura modelos gratuitos en segundos.</p>
<!-- END_AUTO_STATS -->
</p>

<p align="center">
  <a href="https://freellms.org" target="_blank" rel="noopener"><strong>🌐 Visita freellms.org</strong></a> —
  <a href="https://freellms.org/models/" target="_blank" rel="noopener">Explorar modelos</a> ·
  <a href="https://freellms.org/playground/" target="_blank" rel="noopener">Playground</a> ·
  <a href="https://freellms.org/config/" target="_blank" rel="noopener">Generador de configuración</a> ·
  <a href="https://freellms.org/free-llm-api-keys/" target="_blank" rel="noopener">Claves API</a>
</p>

<p align="center">
  <img alt="Logotipos de proveedores" src="assets/provider-logos-marquee.svg" width="100%" />
</p>

<!-- AUTO_UPDATE_BADGE -->
  <p align="center"><strong>🔄 Datos actualizados diariamente desde <a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a></strong> — Última actualización: 2026-08-09</p>
<!-- END_AUTO_UPDATE_BADGE -->

<p align="center">
  🌐 <a href="README.md">English</a> · <a href="README.zh-CN.md">简体中文</a> · <a href="README.zh-TW.md">繁體中文</a> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <strong>Español</strong> · <a href="README.la.md">Latine</a>
</p>

---

## Por qué existe este proyecto

Encontrar una API de LLM gratuita no debería requerir revisar decenas de README de GitHub, crear cuentas en varias plataformas o adivinar qué modelos todavía tienen un nivel gratuito.

Este repositorio es un **directorio estructurado y legible por máquinas** de API de LLM gratuitas: límites de velocidad, ventanas de contexto, fragmentos de configuración y enlaces directos para obtener claves API. Se actualiza a diario.

**Por qué este repositorio y <a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a>:**

- ✅ **Siempre actualizado** — datos renovados diariamente mediante supervisión automatizada, no una lista estática antigua
- ✅ **Transparencia sobre tarjetas** — indica qué proveedores requieren tarjeta, verificación telefónica o nada
- ✅ **Configuraciones en un clic** — fragmentos listos para Claude Code, Cursor, Codex, Aider y más de 10 herramientas
- ✅ **Comparación lado a lado** — compara ventanas de contexto, límites de velocidad y modalidades al instante

---

## Cómo usarlo — 3 pasos

1. **Elige un proveedor** — consulta el [Directorio de proveedores](#directorio-de-proveedores). Empieza con **Groq** (sin tarjeta de crédito y 30 RPM gratis).
2. **Obtén tu clave API** — pulsa cualquier enlace [Obtener clave →](#referencia-rápida--url-base-y-claves-api), regístrate (normalmente basta un correo) y copia la clave. Tarda menos de un minuto.
3. **Configúrala** — copia la URL base y el ID del modelo, y pégalos en los ejemplos de [Inicio rápido](#inicio-rápido--usa-cualquier-api-gratuita-en-30-segundos).

¿Quieres configurar una herramienta concreta? <a href="https://freellms.org/config/#claude-code" target="_blank" rel="noopener">Claude Code</a> · <a href="https://freellms.org/config/#cursor" target="_blank" rel="noopener">Cursor</a> · <a href="https://freellms.org/config/#codex" target="_blank" rel="noopener">Codex</a> · <a href="https://freellms.org/config/#openhuman" target="_blank" rel="noopener">OpenHuman</a> · <a href="https://freellms.org/config/#opencode" target="_blank" rel="noopener">OpenCode</a> · <a href="https://freellms.org/config/#openclaw" target="_blank" rel="noopener">OpenClaw</a> — configuraciones en un clic en <a href="https://freellms.org/config/" target="_blank" rel="noopener">freellms.org/config/</a>.



## Inicio rápido — Usa cualquier API gratuita en 30 segundos

**¿Nunca has usado una API?** La ruta más sencilla es abrir <a href="https://console.groq.com/keys" target="_blank" rel="noopener">console.groq.com/keys</a>, registrarte con un correo (sin tarjeta), copiar la clave gratuita y pegarla en cualquiera de los ejemplos. Estará funcionando en menos de un minuto.

Todos los proveedores siguientes exponen un **endpoint compatible con OpenAI**. Cualquier herramienta que acepte `baseURL` y `apiKey` funciona: basta sustituir la URL base y la clave.

### Python (OpenAI SDK)

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.groq.com/openai/v1",  # gratis, sin tarjeta
    api_key="GROQ_API_KEY",                     # obtener en console.groq.com/keys
)

response = client.chat.completions.create(
    model="llama-3.3-70b-versatile",            # consulta la tabla de mejores modelos
    messages=[{"role": "user", "content": "¡Hola!"}],
)
print(response.choices[0].message.content)
# Nivel gratuito de Groq: 30 RPM y 14.400 RPD, suficiente para uso personal
```

### Codex CLI

```bash
export OPENAI_BASE_URL="https://api.groq.com/openai/v1"
export OPENAI_API_KEY="tu-clave-groq"          # obtener en console.groq.com/keys
codex --model "llama-3.3-70b-versatile"
```

### Cursor

```
Ajustes → Modelos → Añadir modelo
  Nombre del modelo: llama-3.3-70b-versatile
  URL base: https://api.groq.com/openai/v1
  Clave API: tu-clave-groq                     # obtener en console.groq.com/keys
```

### Claude Code

```bash
# Claude Code necesita una API compatible con Anthropic; usa OpenRouter
export ANTHROPIC_BASE_URL="https://openrouter.ai/api"
export ANTHROPIC_AUTH_TOKEN="sk-or-v1-your-key"  # openrouter.ai/keys
export ANTHROPIC_API_KEY=""                       # must be empty
# Nota: los modelos Anthropic de OpenRouter requieren una recarga única de 10 USD
```

### ¿Usas otras herramientas?

La mayoría de herramientas de desarrollo con IA aceptan endpoints personalizados. Apúntalas a cualquiera de los proveedores anteriores y obtén su clave gratuita:

- **Claude Code** — define `ANTHROPIC_BASE_URL` y `ANTHROPIC_AUTH_TOKEN`. <a href="https://freellms.org/config/#claude-code" target="_blank" rel="noopener">Paso a paso →</a>
- **Cursor** — Ajustes → Modelos → Añadir modelo. <a href="https://freellms.org/config/#cursor" target="_blank" rel="noopener">Paso a paso →</a>
- **Codex CLI** — define `OPENAI_BASE_URL` y `OPENAI_API_KEY`. <a href="https://freellms.org/config/#codex" target="_blank" rel="noopener">Paso a paso →</a>
- **OpenHuman** — edita `config.toml`. <a href="https://freellms.org/config/#openhuman" target="_blank" rel="noopener">Paso a paso →</a>
- **Aider** — edita `.aider.conf.yml`. <a href="https://freellms.org/config/#aider" target="_blank" rel="noopener">Paso a paso →</a>
- **Cline** (VS Code) — ajustes del proveedor de API. <a href="https://freellms.org/config/#cline" target="_blank" rel="noopener">Paso a paso →</a>
- **Open WebUI** — Ajustes → Conexiones. <a href="https://freellms.org/config/#open-webui" target="_blank" rel="noopener">Paso a paso →</a>

Más configuraciones listas para copiar en <a href="https://freellms.org/config/" target="_blank" rel="noopener"><strong>freellms.org/config/</strong></a>.

> **Todos los proveedores, URL base y enlaces de claves API** están en la [Referencia rápida](#referencia-rápida--url-base-y-claves-api).


---

## Directorio de proveedores

### ⚡ Niveles gratuitos permanentes

Estos proveedores ofrecen un **nivel gratuito permanente**; la mayoría no requiere tarjeta de crédito.

<!-- BEGIN_PERMANENT_FREE -->
| Proveedor | Modelos gratuitos | ¿Tarjeta de crédito? | Contexto máximo | Modalidades | Obtener clave API |
|---|---|---|---|---|---|
| NVIDIA NIM | 123 | Verificación telefónica | 1M | audio, embedding, image, reasoning, rerank, text, video, vision | <a href="https://build.nvidia.com/settings/api-keys" target="_blank" rel="noopener">→</a> |
| ModelScope | 55 | Registro | 1M | audio, image, reasoning, text, video, vision | <a href="https://modelscope.cn/my/myaccesstoken" target="_blank" rel="noopener">→</a> |
| Cloudflare Workers AI | 39 | No | 10M | code, image, reasoning, text, video | <a href="https://dash.cloudflare.com/profile/api-tokens" target="_blank" rel="noopener">→</a> |
| GitHub Models | 16 | No | 1M | image, pdf, reasoning, text | <a href="https://github.com/marketplace/models" target="_blank" rel="noopener">→</a> |
| Google Gemini | 15 | No | 1M | audio, image, pdf, reasoning, text, video, vision | <a href="https://aistudio.google.com/app/apikey" target="_blank" rel="noopener">→</a> |
| LLM7.io | 15 | No | 1M | audio, code, image, pdf, reasoning, text, video, vision | <a href="https://token.llm7.io" target="_blank" rel="noopener">→</a> |
| OVHcloud AI Endpoints | 14 | Registro | 262K | audio, code, image, reasoning, text, video | <a href="https://www.ovhcloud.com/en/public-cloud/ai-endpoints/catalog/" target="_blank" rel="noopener">→</a> |
| Groq | 12 | No | 262K | image, reasoning, text | <a href="https://console.groq.com/keys" target="_blank" rel="noopener">→</a> |
| Mistral AI | 12 | No | 256K | code, image, text | <a href="https://console.mistral.ai/api-keys" target="_blank" rel="noopener">→</a> |
| Cohere | 12 | No | 436K | image, text | <a href="https://dashboard.cohere.com/api-keys" target="_blank" rel="noopener">→</a> |
| Kilo Code | 12 | No | 1M | audio, code, image, reasoning, text, video | <a href="https://kilo.ai" target="_blank" rel="noopener">→</a> |
| Ollama Cloud | 9 | Registro | 1M | code, image, reasoning, text, video | <a href="https://ollama.com/settings/keys" target="_blank" rel="noopener">→</a> |
| OpenCode Zen | 9 | Registro | 1M | audio, reasoning, vision | <a href="https://opencode.ai/auth" target="_blank" rel="noopener">→</a> |
| Cerebras | 8 | No | 131K | image, reasoning, text | <a href="https://cloud.cerebras.ai/" target="_blank" rel="noopener">→</a> |
| Aion Labs | 7 | Registro | 131K | text | <a href="https://www.aionlabs.ai" target="_blank" rel="noopener">→</a> |
| Hugging Face | 7 | No | 131K | code, text | <a href="https://huggingface.co/settings/tokens" target="_blank" rel="noopener">→</a> |
| Agnes AI | 5 | Registro | 256K | image, text, video, vision | <a href="https://platform.agnes-ai.com/settings/apiKeys" target="_blank" rel="noopener">→</a> |
| Alibaba Cloud Model Studio | 5 | Registro | 1M | code, image, text | <a href="https://bailian.console.alibabacloud.com/?apiKey=1" target="_blank" rel="noopener">→</a> |
| Z AI (Zhipu AI) | 4 | No | 200K | image, reasoning, text, video | <a href="https://open.bigmodel.cn/usercenter/apikeys" target="_blank" rel="noopener">→</a> |
| SambaNova | 4 | Registro | 128K | image, reasoning, text | <a href="https://cloud.sambanova.ai/apis" target="_blank" rel="noopener">→</a> |
| SiliconFlow | 3 | Registro | 131K | text | <a href="https://cloud.siliconflow.cn/account/ak" target="_blank" rel="noopener">→</a> |
| xAI | 3 | Registro | 2M | text | <a href="https://console.x.ai" target="_blank" rel="noopener">→</a> |
| Chutes.ai | 2 | Registro | 131K | reasoning, text | <a href="https://chutes.ai/" target="_blank" rel="noopener">→</a> |
| Glhf.chat | 2 | Registro | 131K | text | <a href="https://glhf.chat/" target="_blank" rel="noopener">→</a> |
| Grok (xAI) | 2 | Registro | 131K | text | <a href="https://console.x.ai/" target="_blank" rel="noopener">→</a> |
| AI21 Labs | 2 | Registro | 256K | text | <a href="https://studio.ai21.com/account/api-key" target="_blank" rel="noopener">→</a> |
| DeepSeek | 2 | Registro | 128K | text | <a href="https://platform.deepseek.com/api_keys" target="_blank" rel="noopener">→</a> |
| Nscale | 2 | Registro | 128K | text | <a href="https://console.nscale.com/" target="_blank" rel="noopener">→</a> |
| Nebius | 1 | Registro | 128K | text | <a href="https://studio.nebius.com/settings/api-keys" target="_blank" rel="noopener">→</a> |
<!-- END_PERMANENT_FREE -->

### 💰 Créditos renovables

Proveedores que renuevan periódicamente créditos gratuitos.

<!-- BEGIN_RENEWABLE -->
| Proveedor | Modelos gratuitos | Modelo de crédito | Contexto máximo | Modalidades | Obtener clave API |
|---|---|---|---|---|---|
| OpenRouter | 22 | Nivel gratuito + $10 topup → 1K RPD | 1M | audio, code, embeddings, image, reasoning, rerank, speech, text, video | <a href="https://openrouter.ai/workspaces/default/keys" target="_blank" rel="noopener">→</a> |
<!-- END_RENEWABLE -->

## Referencia rápida — URL base y claves API

<!-- BEGIN_QUICK_REF -->
| Proveedor | URL base | Obtener clave API | ¿Tarjeta de crédito? |
|---|---|---|---|
| NVIDIA NIM | `https://integrate.api.nvidia.com/v1` | <a href="https://build.nvidia.com/settings/api-keys" target="_blank" rel="noopener">Obtener clave →</a> | Verificación telefónica |
| ModelScope | `https://api-inference.modelscope.cn/v1` | <a href="https://modelscope.cn/my/myaccesstoken" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Cloudflare Workers AI | `https://api.cloudflare.com/client/v4/accounts/{account_id}/ai/run` | <a href="https://dash.cloudflare.com/profile/api-tokens" target="_blank" rel="noopener">Obtener clave →</a> | No |
| OpenRouter | `https://openrouter.ai/api/v1` | <a href="https://openrouter.ai/workspaces/default/keys" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| GitHub Models | `https://models.github.ai/inference` | <a href="https://github.com/marketplace/models" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Google Gemini | `https://generativelanguage.googleapis.com/v1beta` | <a href="https://aistudio.google.com/app/apikey" target="_blank" rel="noopener">Obtener clave →</a> | No |
| LLM7.io | `https://api.llm7.io/v1` | <a href="https://token.llm7.io" target="_blank" rel="noopener">Obtener clave →</a> | No |
| OVHcloud AI Endpoints | `https://oai.endpoints.kepler.ai.cloud.ovh.net/v1` | <a href="https://www.ovhcloud.com/en/public-cloud/ai-endpoints/catalog/" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Groq | `https://api.groq.com/openai/v1` | <a href="https://console.groq.com/keys" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Mistral AI | `https://api.mistral.ai/v1` | <a href="https://console.mistral.ai/api-keys" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Cohere | `https://api.cohere.com/v2` | <a href="https://dashboard.cohere.com/api-keys" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Kilo Code | `https://api.kilo.ai/api/gateway` | <a href="https://kilo.ai" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Ollama Cloud | `https://api.ollama.com` | <a href="https://ollama.com/settings/keys" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| OpenCode Zen | `https://opencode.ai/zen/v1` | <a href="https://opencode.ai/auth" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Cerebras | `https://api.cerebras.ai/v1` | <a href="https://cloud.cerebras.ai/" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Aion Labs | `https://api.aionlabs.ai/v1` | <a href="https://www.aionlabs.ai" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Hugging Face | `https://router.huggingface.co/v1` | <a href="https://huggingface.co/settings/tokens" target="_blank" rel="noopener">Obtener clave →</a> | No |
| Agnes AI | `https://apihub.agnes-ai.com/v1` | <a href="https://platform.agnes-ai.com/settings/apiKeys" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Alibaba Cloud Model Studio | `https://dashscope-intl.aliyuncs.com/compatible-mode/v1` | <a href="https://bailian.console.alibabacloud.com/?apiKey=1" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Z AI (Zhipu AI) | `https://open.bigmodel.cn/api/paas/v4` | <a href="https://open.bigmodel.cn/usercenter/apikeys" target="_blank" rel="noopener">Obtener clave →</a> | No |
| SambaNova | `https://api.sambanova.ai/v1` | <a href="https://cloud.sambanova.ai/apis" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| SiliconFlow | `https://api.siliconflow.cn/v1` | <a href="https://cloud.siliconflow.cn/account/ak" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| xAI | `https://api.x.ai/v1` | <a href="https://console.x.ai" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Chutes.ai | `https://api.chutes.ai/v1` | <a href="https://chutes.ai/" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Glhf.chat | `https://glhf.chat/api/openai/v1` | <a href="https://glhf.chat/" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Grok (xAI) | `https://api.x.ai/v1` | <a href="https://console.x.ai/" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| AI21 Labs | `https://api.ai21.com/studio/v1` | <a href="https://studio.ai21.com/account/api-key" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| DeepSeek | `https://api.deepseek.com/v1` | <a href="https://platform.deepseek.com/api_keys" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Nscale | `https://inference.api.nscale.com/v1` | <a href="https://console.nscale.com/" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
| Nebius | `https://api.studio.nebius.com/v1` | <a href="https://studio.nebius.com/settings/api-keys" target="_blank" rel="noopener">Obtener clave →</a> | Registro |
<!-- END_QUICK_REF -->

## Mejores modelos gratuitos por proveedor

<!-- BEGIN_BEST_MODELS -->
| Proveedor | Mejor modelo gratuito | ID del modelo | Contexto máximo | Límite de velocidad |
|---|---|---|---|---|
| NVIDIA NIM | <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-2/" target="_blank" rel="noopener">z-ai/glm-5.2</a> | `z-ai/glm-5.2` | 1M | Hasta 40 RPM |
|  | <a href="https://freellms.org/models/nvidia-nim/poolside-laguna-xs-2-1/" target="_blank" rel="noopener">poolside/laguna-xs-2.1</a> | `poolside/laguna-xs-2.1` | 262K | Hasta 40 RPM |
|  | <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-1/" target="_blank" rel="noopener">z-ai/glm-5.1</a> | `z-ai/glm-5.1` | 202K | Hasta 40 RPM |
| ModelScope | <a href="https://freellms.org/models/modelscope/minimax-minimax-m2-5/" target="_blank" rel="noopener">MiniMax-M2.5-highspeed</a> | `MiniMax/MiniMax-M2.5` | 204K | Ver proveedor |
|  | <a href="https://freellms.org/models/modelscope/qwen-qwen3-5-35b-a3b/" target="_blank" rel="noopener">Qwen/Qwen3.5-35B-A3B</a> | `qwen-qwen3-5-35b-a3b` | 131K | 2,000 RPD en total; <=500 .. |
|  | <a href="https://freellms.org/models/modelscope/qwen-qwen3-5-27b/" target="_blank" rel="noopener">Qwen/Qwen3.5-27B</a> | `qwen-qwen3-5-27b` | 131K | 2,000 RPD en total; <=500 .. |
| Cloudflare Workers AI | <a href="https://freellms.org/models/cloudflare-workers-ai/mistral-mistral-7b-instruct-v0-1/" target="_blank" rel="noopener">Mistral 7B</a> | `@cf/mistral/mistral-7b-instruct-v0.1` | 32K | Ver proveedor |
|  | <a href="https://freellms.org/models/cloudflare-workers-ai/qwen-qwen1-5-7b-chat/" target="_blank" rel="noopener">Qwen 1.5 7B</a> | `@cf/qwen/qwen1.5-7b-chat` | 32K | Ver proveedor |
|  | <a href="https://freellms.org/models/cloudflare-workers-ai/cf-meta-llama-3-3-70b-instruct-fp8-fast/" target="_blank" rel="noopener">@cf/meta/llama-3.3-70b-instruct-fp8-fast</a> | `@cf/meta/llama-3.3-70b-instruct-fp8-fast` | 131K | 10K neuronas/día (compartido) |
| OpenRouter | <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-ultra-550b-a55b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Ultra (gratuito)</a> | `nvidia/nemotron-3-ultra-550b-a55b:free` | 1M | Ver proveedor |
|  | <a href="https://freellms.org/models/openrouter/poolside-laguna-m-1/" target="_blank" rel="noopener">Poolside: Laguna M.1 (gratuito)</a> | `poolside/laguna-m.1:free` | 262K | Ver proveedor |
|  | <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-super-120b-a12b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Super (gratuito)</a> | `nvidia/nemotron-3-super-120b-a12b:free` | 262K | Ver proveedor |
| GitHub Models | <a href="https://freellms.org/models/github-models/phi-4/" target="_blank" rel="noopener">Phi-4</a> | `Phi-4` | 131K | Ver proveedor |
|  | <a href="https://freellms.org/models/github-models/mistral-large-2411/" target="_blank" rel="noopener">Mistral Large (24.11)</a> | `Mistral-large-2411` | 131K | Ver proveedor |
|  | <a href="https://freellms.org/models/github-models/ai21-jamba-1-5-large/" target="_blank" rel="noopener">AI21 Jamba 1.5 Large</a> | `AI21-Jamba-1.5-Large` | 256K | Ver proveedor |
| Google Gemini | <a href="https://freellms.org/models/google-gemini/gemini-3-6-flash/" target="_blank" rel="noopener">Gemini 3.6 Flash</a> | `gemini-3.6-flash` | 1M | 15 RPM, 1,500 RPD |
|  | <a href="https://freellms.org/models/google-gemini/gemini-3-5-flash/" target="_blank" rel="noopener">Gemini 3.5 Flash</a> | `gemini-3.5-flash` | 1M | 15 RPM, 1,500 RPD |
|  | <a href="https://freellms.org/models/google-gemini/gemini-3-5-flash-lite/" target="_blank" rel="noopener">Gemini 3.5 Flash-Lite</a> | `gemini-3.5-flash-lite` | 1M | 30 RPM, 1,500 RPD |
| LLM7.io | <a href="https://freellms.org/models/llm7-io/deepseek-r1-0528/" target="_blank" rel="noopener">deepseek-r1-0528</a> | `deepseek-r1-0528` | 131K | 30 RPM (120 con token) |
|  | <a href="https://freellms.org/models/llm7-io/deepseek-v3-0324/" target="_blank" rel="noopener">deepseek-v3-0324</a> | `deepseek-v3-0324` | 131K | 30 RPM (120 con token) |
|  | <a href="https://freellms.org/models/llm7-io/gpt-4o-mini/" target="_blank" rel="noopener">gpt-4o-mini</a> | `gpt-4o-mini` | 131K | 30 RPM (120 con token) |
| OVHcloud AI Endpoints | <a href="https://freellms.org/models/ovhcloud-ai-endpoints/qwen3-5-397b-a17b/" target="_blank" rel="noopener">Qwen3.5-397B-A17B</a> | `qwen3.5-397b-a17b` | 131K | 2 RPM (anónimo) |
|  | <a href="https://freellms.org/models/ovhcloud-ai-endpoints/meta-llama-3-3-70b-instruct/" target="_blank" rel="noopener">Meta-Llama-3_3-70B-Instruct</a> | `meta-llama-3_3-70b-instruct` | 131K | 2 RPM (anónimo) |
|  | <a href="https://freellms.org/models/ovhcloud-ai-endpoints/qwen3-6-27b/" target="_blank" rel="noopener">Qwen3.6-27B</a> | `qwen3.6-27b` | 131K | 2 RPM (anónimo) |
| Groq | <a href="https://freellms.org/models/groq/moonshotai-kimi-k2-instruct/" target="_blank" rel="noopener">Moonshot Kimi K2</a> | `moonshotai/kimi-k2-instruct` | 131K | Ver proveedor |
|  | <a href="https://freellms.org/models/groq/moonshotai-kimi-k2-instruct-0905/" target="_blank" rel="noopener">Moonshot Kimi K2 0905</a> | `moonshotai/kimi-k2-instruct-0905` | 131K | Ver proveedor |
|  | <a href="https://freellms.org/models/groq/groq-compound/" target="_blank" rel="noopener">groq/compound</a> | `groq/compound` | 131K | 30 RPM, 250 RPD |
| Mistral AI | <a href="https://freellms.org/models/mistral-ai/open-mistral-7b/" target="_blank" rel="noopener">Mistral 7B</a> | `open-mistral-7b` | 32K | Ver proveedor |
|  | <a href="https://freellms.org/models/mistral-ai/open-mixtral-8x7b/" target="_blank" rel="noopener">Mixtral 8x7B</a> | `open-mixtral-8x7b` | 32K | Ver proveedor |
|  | <a href="https://freellms.org/models/mistral-ai/mistral-medium-3-5-128b/" target="_blank" rel="noopener">Mistral Medium 3.5 (128B)</a> | `mistral-medium-3-5-128b` | 256K | ~1 RPS, 500K TPM |
| Cohere | <a href="https://freellms.org/models/cohere/command-a-218b/" target="_blank" rel="noopener">Command A+ (218B)</a> | `command-a-218b` | 436K | 20 RPM |
|  | <a href="https://freellms.org/models/cohere/command-a-111b/" target="_blank" rel="noopener">Command A (111B)</a> | `command-a-111b` | 288K | 20 RPM |
|  | <a href="https://freellms.org/models/cohere/command-r/" target="_blank" rel="noopener">Command R+</a> | `command-r` | 128K | 20 RPM |
| Kilo Code | <a href="https://freellms.org/models/kilo-code/nvidia-nemotron-3-ultra-550b-a55b-free/" target="_blank" rel="noopener">nvidia/nemotron-3-ultra-550b-a55b:free</a> | `nvidia/nemotron-3-ultra-550b-a55b:free` | 1M | ~200 req/hr |
|  | <a href="https://freellms.org/models/kilo-code/stepfun-step-3-7-flash-free/" target="_blank" rel="noopener">stepfun/step-3.7-flash:free</a> | `stepfun/step-3.7-flash:free` | 262K | ~200 req/hr |
|  | <a href="https://freellms.org/models/kilo-code/nvidia-nemotron-3-super-120b-a12b-free/" target="_blank" rel="noopener">nvidia/nemotron-3-super-120b-a12b:free</a> | `nvidia/nemotron-3-super-120b-a12b:free` | 262K | ~200 req/hr |
| Ollama Cloud | <a href="https://freellms.org/models/ollama-cloud/minimax-m3/" target="_blank" rel="noopener">minimax-m3</a> | `minimax-m3` | 1M | Límites de sesión o semanales (.. |
|  | <a href="https://freellms.org/models/ollama-cloud/gpt-oss-20b/" target="_blank" rel="noopener">gpt-oss:20b</a> | `gpt-oss:20b` | 131K | Límites de sesión o semanales (.. |
|  | <a href="https://freellms.org/models/ollama-cloud/nemotron-3-ultra/" target="_blank" rel="noopener">nemotron-3-ultra</a> | `nemotron-3-ultra` | 262K | Límites de sesión o semanales (.. |
| OpenCode Zen | <a href="https://freellms.org/models/opencode/big-pickle/" target="_blank" rel="noopener">big-pickle</a> | `big-pickle` | 0 |  |
|  | <a href="https://freellms.org/models/opencode/deepseek-v4-flash-free/" target="_blank" rel="noopener">DeepSeek V4 Flash</a> | `deepseek-v4-flash-free` | 1M |  |
|  | <a href="https://freellms.org/models/opencode/mimo-v2-5-free/" target="_blank" rel="noopener">MiMo-V2.5</a> | `mimo-v2.5-free` | 1M |  |
| Cerebras | <a href="https://freellms.org/models/cerebras/llama3-1-70b/" target="_blank" rel="noopener">Llama 3.1 70B</a> | `llama3.1-70b` | 131K | Ver proveedor |
|  | <a href="https://freellms.org/models/cerebras/gpt-oss-120b/" target="_blank" rel="noopener">gpt-oss-120b</a> | `gpt-oss-120b` | 131K | 5 RPM, 30K TPM, 1M TPD |
|  | <a href="https://freellms.org/models/cerebras/zai-glm-4-7-deprecated-aug-2026/" target="_blank" rel="noopener">zai-glm-4.7 (deprecated Aug 2026)</a> | `zai-glm-4.7` | 131K | 5 RPM, 30K TPM, 1M TPD |
| Aion Labs | <a href="https://freellms.org/models/aion-labs/aion-2-5/" target="_blank" rel="noopener">Aion 2.5</a> | `aion-2-5` | 128K | 15 RPM, 20K TPD |
|  | <a href="https://freellms.org/models/aion-labs/aion-2-0/" target="_blank" rel="noopener">Aion 2.0</a> | `aion-2-0` | 128K | 15 RPM, 20K TPD |
|  | <a href="https://freellms.org/models/aion-labs/aion-rp-1-0-8b/" target="_blank" rel="noopener">Aion-RP 1.0 (8B)</a> | `aion-rp-1-0-8b` | 32K | 15 RPM, 20K TPD |
| Hugging Face | <a href="https://freellms.org/models/hugging-face/meta-llama-3-1-8b-instruct/" target="_blank" rel="noopener">Meta-Llama-3.1-8B-Instruct</a> | `meta-llama-3-1-8b-instruct` | 128K | Medido por créditos |
|  | <a href="https://freellms.org/models/hugging-face/gemma-3-4b-it/" target="_blank" rel="noopener">gemma-3-4b-it</a> | `gemma-3-4b-it` | 131K | Medido por créditos |
|  | <a href="https://freellms.org/models/hugging-face/qwen2-5-coder-7b-instruct/" target="_blank" rel="noopener">Qwen2.5-Coder-7B-Instruct</a> | `qwen2-5-coder-7b-instruct` | 131K | Medido por créditos |
| Agnes AI | <a href="https://freellms.org/models/agnes-ai/agnes-1-5-flash/" target="_blank" rel="noopener">agnes-1.5-flash</a> | `agnes-1.5-flash` | 256K | 30 RPM |
|  | <a href="https://freellms.org/models/agnes-ai/agnes-2-0-flash/" target="_blank" rel="noopener">agnes-2.0-flash</a> | `agnes-2.0-flash` | 256K | 30 RPM |
|  | <a href="https://freellms.org/models/agnes-ai/agnes-image-2-0-flash/" target="_blank" rel="noopener">agnes-image-2.0-flash</a> | `agnes-image-2.0-flash` | 4K | 30 RPM (1K) |
| Alibaba Cloud Model Studio | <a href="https://freellms.org/models/alibaba-cloud-model-studio/qwen3-max/" target="_blank" rel="noopener">Qwen3-Max</a> | `qwen3-max` | 128K | Por nivel y región |
|  | <a href="https://freellms.org/models/alibaba-cloud-model-studio/qwen3-plus/" target="_blank" rel="noopener">Qwen3-Plus</a> | `qwen3-plus` | 1M | Por nivel y región |
|  | <a href="https://freellms.org/models/alibaba-cloud-model-studio/qwen3-vl-plus/" target="_blank" rel="noopener">Qwen3-VL-Plus</a> | `qwen3-vl-plus` | 128K | Por nivel y región |
| Z AI (Zhipu AI) | <a href="https://freellms.org/models/z-ai-zhipu-ai/glm-4-7-flash/" target="_blank" rel="noopener">GLM-4.7-Flash</a> | `glm-4.7` | 200K | 1 solicitud simultánea |
|  | <a href="https://freellms.org/models/z-ai-zhipu-ai/glm-4-5-flash/" target="_blank" rel="noopener">GLM-4.5-Flash</a> | `glm-4.5` | 128K | 1 solicitud simultánea |
|  | <a href="https://freellms.org/models/z-ai-zhipu-ai/glm-4-6v-flash/" target="_blank" rel="noopener">GLM-4.6V-Flash</a> | `glm-4.6` | 128K | 1 solicitud simultánea |
| SambaNova | <a href="https://freellms.org/models/sambanova/deepseek-v3-1/" target="_blank" rel="noopener">DeepSeek-V3.1</a> | `deepseek-v3-1` | 128K | 20 RPM, 20 RPD, 200K TPD |
|  | <a href="https://freellms.org/models/sambanova/deepseek-v3-2-preview/" target="_blank" rel="noopener">DeepSeek-V3.2 (Vista previa)</a> | `deepseek-v3-2-preview` | 128K | 20 RPM, 20 RPD, 200K TPD |
|  | <a href="https://freellms.org/models/sambanova/minimax-m2-7/" target="_blank" rel="noopener">MiniMax-M2.7</a> | `minimax-m2-7` | 128K | 20 RPM, 20 RPD, 200K TPD |
| SiliconFlow | <a href="https://freellms.org/models/siliconflow/deepseek-ai-deepseek-r1-distill-qwen-7b/" target="_blank" rel="noopener">deepseek-ai/DeepSeek-R1-Distill-Qwen-7B</a> | `deepseek-ai-deepseek-r1-distill-qwen-7b` | 131K | 30 RPM, 60K TPM |
|  | <a href="https://freellms.org/models/siliconflow/abbreviation/" target="_blank" rel="noopener">Abbreviation</a> | `abbreviation` | 131K | Ver proveedor |
|  | <a href="https://freellms.org/models/siliconflow/deepseek-ai-deepseek-ocr/" target="_blank" rel="noopener">deepseek-ai/DeepSeek-OCR</a> | `deepseek-ai-deepseek-ocr` | 131K | 30 RPM, 60K TPM |
| xAI | <a href="https://freellms.org/models/xai/grok-4-3/" target="_blank" rel="noopener">grok-4.3</a> | `grok-4-3` | 1M | Basado en créditos |
|  | <a href="https://freellms.org/models/xai/grok-4-1-fast/" target="_blank" rel="noopener">grok-4.1-fast</a> | `grok-4-1-fast` | 2M | Basado en créditos |
|  | <a href="https://freellms.org/models/xai/grok-3-mini/" target="_blank" rel="noopener">grok-3-mini</a> | `grok-3-mini` | 131K | Basado en créditos |
| Chutes.ai | <a href="https://freellms.org/models/chutes-ai/deepseek-ai-deepseek-r1/" target="_blank" rel="noopener">DeepSeek-R1</a> | `deepseek-ai/DeepSeek-R1` | 131K | Impulsado por la comunidad, sin h... |
|  | <a href="https://freellms.org/models/chutes-ai/meta-llama-meta-llama-3-1-70b-instruct/" target="_blank" rel="noopener">Llama 3.1 70B</a> | `meta-llama/Meta-Llama-3.1-70B-Instruct` | 131K | Impulsado por la comunidad, sin h... |
| Glhf.chat | <a href="https://freellms.org/models/glhf-chat/meta-llama-meta-llama-3-1-70b-instruct-2/" target="_blank" rel="noopener">Llama 3.1 70B</a> | `meta-llama/Meta-Llama-3.1-70B-Instruct` | 131K | Ilimitado para modelos gratuitos |
|  | <a href="https://freellms.org/models/glhf-chat/mistralai-mixtral-8x7b-instruct-v0-1/" target="_blank" rel="noopener">Mixtral 8x7B</a> | `mistralai/Mixtral-8x7B-Instruct-v0.1` | 32K | Ilimitado para modelos gratuitos |
| Grok (xAI) | <a href="https://freellms.org/models/grok-(xai)/grok-2/" target="_blank" rel="noopener">Grok-2</a> | `grok-2` | 131K | 25 USD/mes en créditos gratuitos,.. |
|  | <a href="https://freellms.org/models/grok-(xai)/grok-2-mini/" target="_blank" rel="noopener">Grok-2 Mini</a> | `grok-2-mini` | 131K | 25 USD/mes en créditos gratuitos,.. |
| AI21 Labs | <a href="https://freellms.org/models/ai21-labs/jamba-large-1-7/" target="_blank" rel="noopener">Jamba Large 1.7</a> | `jamba-large-1-7` | 256K | 200 RPM, 10 RPS |
|  | <a href="https://freellms.org/models/ai21-labs/jamba-mini-2/" target="_blank" rel="noopener">Jamba Mini 2</a> | `jamba-mini-2` | 256K | 200 RPM, 10 RPS |
| DeepSeek | <a href="https://freellms.org/models/deepseek/deepseek-chat-v3-2/" target="_blank" rel="noopener">deepseek-chat (V3.2)</a> | `deepseek-chat-v3-2` | 128K | Dinámico |
|  | <a href="https://freellms.org/models/deepseek/deepseek-reasoner-r1/" target="_blank" rel="noopener">deepseek-reasoner (R1)</a> | `deepseek-reasoner-r1` | 128K | Dinámico |
| Nscale | <a href="https://freellms.org/models/nscale/llama-3-3-70b-instruct/" target="_blank" rel="noopener">Llama-3.3-70B-Instruct</a> | `llama-3-3-70b-instruct` | 128K | Uso razonable |
|  | <a href="https://freellms.org/models/nscale/deepseek-r1-distill-llama-70b/" target="_blank" rel="noopener">DeepSeek-R1-Distill-Llama-70B</a> | `deepseek-r1-distill-llama-70b` | 128K | Uso razonable |
| Nebius | <a href="https://freellms.org/models/nebius/qwen3-235b-a22b/" target="_blank" rel="noopener">Qwen3-235B-A22B</a> | `qwen3-235b-a22b` | 128K | Por nivel |
<!-- END_BEST_MODELS -->



### 🖥️ Local o autoalojado (ilimitado, privado y gratuito para siempre)

| Herramienta | Tipo | Características |
|---|---|---|
| <a href="https://ollama.com" target="_blank" rel="noopener">Ollama</a> | CLI + API | Más de 100 modelos, aceleración GPU, endpoint compatible con OpenAI |
| <a href="https://lmstudio.ai" target="_blank" rel="noopener">LM Studio</a> | Interfaz de escritorio | Cualquier modelo GGUF, navegador integrado, sin conexión |
| <a href="https://github.com/ggerganov/llama.cpp" target="_blank" rel="noopener">llama.cpp</a> | Motor C/C++ | Ejecuta cualquier GGUF, dependencias mínimas |
| <a href="https://gpt4all.io" target="_blank" rel="noopener">GPT4All</a> | Aplicación de escritorio | Solo CPU, no requiere GPU, código abierto |
| <a href="https://jan.ai" target="_blank" rel="noopener">Jan.ai</a> | Aplicación de escritorio | Enfocada en privacidad, alternativa a ChatGPT 100% local |
| <a href="https://github.com/LostRuins/koboldcpp" target="_blank" rel="noopener">KoboldCpp</a> | Ejecutable único | Optimizado para escritura creativa y GGUF |

---

## Modelos gratuitos principales (por uso semanal)

Datos de freellms.org, actualizados diariamente mediante supervisión de API.

<!-- BEGIN_TOP_MODELS -->
| Modelo | Proveedor | Contexto | Uso semanal |
|---|---|---|---|
| <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-2/" target="_blank" rel="noopener">z-ai/glm-5.2</a> | NVIDIA NIM | 1M | 2998B tokens |
| <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-ultra-550b-a55b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Ultra (gratuito)</a> | OpenRouter | 1M | 2326B tokens |
| <a href="https://freellms.org/models/openrouter/poolside-laguna-m-1/" target="_blank" rel="noopener">Poolside: Laguna M.1 (gratuito)</a> | OpenRouter | 262K | 768B tokens |
| <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-super-120b-a12b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Super (gratuito)</a> | OpenRouter | 262K | 315B tokens |
| <a href="https://freellms.org/models/openrouter/cohere-north-mini-code/" target="_blank" rel="noopener">Cohere: North Mini Code (gratuito)</a> | OpenRouter | 256K | 255B tokens |
| <a href="https://freellms.org/models/nvidia-nim/poolside-laguna-xs-2-1/" target="_blank" rel="noopener">poolside/laguna-xs-2.1</a> | NVIDIA NIM | 262K | 171B tokens |
| <a href="https://freellms.org/models/nvidia-nim/z-ai-glm-5-1/" target="_blank" rel="noopener">z-ai/glm-5.1</a> | NVIDIA NIM | 202K | 158B tokens |
| <a href="https://freellms.org/models/openrouter/poolside-laguna-s-2-1/" target="_blank" rel="noopener">Poolside: Laguna S 2.1 (gratuito)</a> | OpenRouter | 262K | 83B tokens |
| <a href="https://freellms.org/models/openrouter/poolside-laguna-xs-2-1/" target="_blank" rel="noopener">Poolside: Laguna XS 2.1 (gratuito)</a> | OpenRouter | 262K | 81B tokens |
| <a href="https://freellms.org/models/openrouter/nvidia-nemotron-3-nano-30b-a3b/" target="_blank" rel="noopener">NVIDIA: Nemotron 3 Nano 30B A3B (gratuito)</a> | OpenRouter | 256K | 45B tokens |
<!-- END_TOP_MODELS -->

---

## Estructura del repositorio

```
freellms/
├── README.md              ← Directorio completo de proveedores y ejemplos de código
├── code-examples/          ← Fragmentos de configuración listos para usar
│   ├── claude-code.md
│   ├── cursor.md
│   └── codex.md
└── LICENSE                 ← MIT
```

> Para consultar el conjunto de datos estructurado completo, con 453 modelos y actualizaciones diarias, visita **<a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a>**.

---

## Contribuir

¡Las contribuciones son bienvenidas!

- **Añadir un modelo gratuito que falte** — Abre una <a href="https://github.com/freellms/freellms/issues" target="_blank" rel="noopener">incidencia</a> o envía un PR
- **Corregir datos inexactos** — Los límites cambian y los proveedores actualizan sus planes. Aceptamos PR
- **Añadir un fragmento de configuración** — ¿Tienes una configuración para una herramienta no cubierta? Añádela a `code-examples/`

### Criterios de inclusión

Un modelo pertenece a esta lista si:
1. El proveedor ofrece explícitamente un **nivel gratuito** (no solo crédito de prueba)
2. La API es **públicamente accesible** (sin lista de espera, beta cerrada ni ingeniería inversa)
3. En el caso de créditos de prueba: están claramente indicados y valen al menos 1 USD

---

## Enlaces

- 🌐 **Sitio web**: <a href="https://freellms.org" target="_blank" rel="noopener">freellms.org</a> — buscar, comparar, probar y generar configuraciones
- 🔑 **Directorio de claves API**: <a href="https://freellms.org/free-llm-api-keys/" target="_blank" rel="noopener">freellms.org/free-llm-api-keys/</a>
- ⚙️ **Generador de configuración**: <a href="https://freellms.org/config/" target="_blank" rel="noopener">freellms.org/config/</a>
- 🎮 **Playground**: <a href="https://freellms.org/playground/" target="_blank" rel="noopener">freellms.org/playground/</a>
- 📊 **Comparar modelos**: <a href="https://freellms.org/compare/" target="_blank" rel="noopener">freellms.org/compare/</a>

## Licencia

MIT © <a href="https://github.com/freellms" target="_blank" rel="noopener">freellms</a>

---

<p align="center">
  <sub>Última actualización: <!-- AUTO_LAST_UPDATED -->
2026-08-09
<!-- END_AUTO_LAST_UPDATED --></sub>
</p>
