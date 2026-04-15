# Quickstart Guide

Get your first AI response in under 60 seconds.

## Step 1: Sign Up

Create a free account at [neurongate.net](https://neurongate.net/login?register=true).

## Step 2: Add Funds

Go to [Top Up](https://neurongate.net/topup) and add at least $5 with any supported crypto:

- USDT (TRC-20 / ERC-20)
- USDC (ERC-20)
- ETH
- BTC

## Step 3: Generate an API Key

Navigate to [API Keys](https://neurongate.net/keys) and click **Create Key**.

## Step 4: Install the OpenAI SDK

```bash
# Python
pip install openai

# Node.js
npm install openai
```

## Step 5: Make a Request

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://neurongate.net/v1",
    api_key="ng-your-api-key"
)

response = client.chat.completions.create(
    model="openai/gpt-4o",
    messages=[{"role": "user", "content": "Hello, NeuronGate!"}]
)

print(response.choices[0].message.content)
```

That's it. You're now routing through NeuronGate.

## Next Steps

- 📚 [Full API Documentation](./README.md)
- 💻 [Code Examples](https://github.com/neurongate/examples)
- 🧠 [Browse Models](https://neurongate.net/models)
- 💰 [Pricing Calculator](https://neurongate.net/#pricing)
