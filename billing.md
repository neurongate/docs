# Billing & Payments Guide

NeuronGate uses a prepaid balance model. No subscriptions, no surprise bills.

## How It Works

1. **Create account** — Free, no card required
2. **Top up balance** — Send crypto to your unique deposit address
3. **Use the API** — Each request deducts from your balance in real-time
4. **Balance hits $0** — API returns `402 Insufficient Balance` (no debt, no overage)

## Supported Payment Methods

| Currency | Network | Min Top-up | Confirmation Time |
|----------|---------|-----------|-------------------|
| **USDT** | TRC-20 | $5 | ~1 minute |
| **USDT** | ERC-20 | $5 | ~3 minutes |
| **USDC** | ERC-20 | $5 | ~3 minutes |
| **ETH** | Ethereum | $5 | ~3 minutes |
| **BTC** | Bitcoin | $10 | ~10-30 minutes |

### Why Crypto?

- **No KYC** for standard access — sign up and start immediately
- **Global access** — no banking restrictions
- **Privacy** — we don't collect payment card details
- **Low fees** — especially on TRC-20 (USDT)

## Checking Your Balance

### Dashboard
Visit [neurongate.net/dashboard](https://neurongate.net/dashboard) for a real-time balance overview.

### API
Your balance is included in the dashboard stats endpoint after authentication.

### NavBar
When logged in, your current balance is always visible in the top-right corner.

## Usage Tracking

Every API request is logged with:
- **Timestamp**
- **Model used**
- **Input/output tokens**
- **Cost** (calculated at time of request)
- **Latency** (tokens per second)
- **Status** (success/error)
- **API key used**

View detailed logs at [neurongate.net/usage](https://neurongate.net/usage).

## Invoices

Invoices are generated automatically for every payment. Each invoice includes:
- Invoice number (e.g., `NG-2026-00035`)
- Payment amount and currency
- Transaction date
- Running balance

View and download invoices at [neurongate.net/invoices](https://neurongate.net/invoices).

Invoices are available as printable HTML pages — use your browser's print function or save as PDF.

## Cost Estimation

### Formula
```
Cost = (input_tokens × input_price) + (output_tokens × output_price)
```

### Example
Using `openai/gpt-4o`:
- Input: $2.50 / 1M tokens
- Output: $10.00 / 1M tokens

A typical request (500 input + 200 output tokens):
```
Cost = (500 × $0.0000025) + (200 × $0.00001) = $0.00325
```

That's **$0.003** per request — about **300 requests per dollar**.

### Cost Calculator
Use the interactive pricing calculator at [neurongate.net/#pricing](https://neurongate.net/#pricing).

## Low Balance Alerts

When your balance drops below $1, you'll see a warning in the dashboard. We recommend keeping a minimum buffer to avoid service interruption.

## FAQ

**Q: What happens when my balance hits $0?**
A: API requests return HTTP 402. No debt is incurred. Top up to resume.

**Q: Can I get a refund?**
A: Unused balance can be refunded. Contact support@neurongate.net.

**Q: Is there a minimum usage?**
A: No. Use as much or as little as you want. No monthly minimums.

**Q: Do you offer volume discounts?**
A: For usage over $1,000/month, contact us for enterprise pricing.
