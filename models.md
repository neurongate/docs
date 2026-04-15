# Model Reference

Complete list of models available through NeuronGate, organized by provider.

> **Live pricing and availability:** [neurongate.net/models](https://neurongate.net/models)

---

## OpenAI

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `openai/gpt-5` | Chat | 128K | Most capable, complex reasoning |
| `openai/gpt-4o` | Chat + Vision | 128K | General purpose, multimodal |
| `openai/gpt-4.1` | Chat | 1M | Long-context, code generation |
| `openai/gpt-4.1-nano` | Chat | 1M | Fast, cheap, high-volume |
| `openai/gpt-4o-mini` | Chat | 128K | Budget-friendly, simple tasks |
| `openai/o3` | Reasoning | 200K | Math, logic, analysis |
| `openai/o3-mini` | Reasoning | 200K | Fast reasoning |

## Anthropic

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `anthropic/claude-opus-4.6` | Chat | 200K | Most capable, deep analysis |
| `anthropic/claude-sonnet-4.6` | Chat | 200K | Balanced speed + quality |
| `anthropic/claude-haiku-4.5` | Chat | 200K | Fast, cheap, simple tasks |
| `anthropic/claude-haiku-4` | Chat | 200K | Legacy, very cheap |

## Google

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `google/gemini-2.5-pro` | Chat + Vision | 1M | Deep analysis, long context |
| `google/gemini-2.5-flash` | Chat + Vision | 1M | Fast, cheap, multimodal |

## Meta

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `meta/llama-4-maverick` | Chat | 128K | Open-weight, versatile |
| `meta/llama-3.3-70b` | Chat | 128K | Strong open model |

## Mistral

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `mistral/mistral-large` | Chat | 128K | Enterprise, multilingual |
| `mistral/codestral` | Code | 32K | Code generation |

## DeepSeek

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `deepseek/deepseek-v3` | Chat | 64K | High quality, affordable |
| `deepseek/deepseek-r1` | Reasoning | 64K | Chain-of-thought reasoning |

## Cohere

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `cohere/command-r-plus` | Chat | 128K | RAG, enterprise search |
| `cohere/embed-english-v3.0` | Embedding | 512 | Vector embeddings |

## xAI

| Model | Type | Context | Best For |
|-------|------|---------|----------|
| `xai/grok-3` | Chat | 128K | Real-time knowledge |
| `xai/grok-3-mini` | Chat | 128K | Fast, affordable |

---

## Choosing a Model

### By Use Case

| Use Case | Recommended | Why |
|----------|-------------|-----|
| **General chat** | `openai/gpt-4o` | Best all-around |
| **Complex reasoning** | `anthropic/claude-opus-4.6` | Deepest analysis |
| **Code generation** | `openai/gpt-4.1` | 1M context, code-optimized |
| **Fast & cheap** | `openai/gpt-4o-mini` | $0.15/M input tokens |
| **Long documents** | `google/gemini-2.5-pro` | 1M token context |
| **Image analysis** | `openai/gpt-4o` | Best vision capabilities |
| **Embeddings** | `openai/text-embedding-3-small` | Best price/quality |

### By Budget

| Budget | Models | Input Cost |
|--------|--------|-----------|
| **Ultra-cheap** | gpt-4o-mini, Haiku 4.5, Gemini Flash | $0.10-0.25/M |
| **Balanced** | GPT-4o, Sonnet, Gemini Pro | $2-3/M |
| **Premium** | GPT-5, Opus, o3 | $10-15/M |

---

> All pricing is per-token, billed in real-time. Check [neurongate.net/models](https://neurongate.net/models) for exact current rates.
