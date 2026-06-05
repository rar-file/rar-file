# free-tier maximalism

a love letter to running real workloads on free tiers.

## the stack

- **Groq** for inference (60 req/min free, fast)
- **SQLite** + sqlite-vss for storage and retrieval
- **Cloudflare Workers** for the API (100k req/day free)
- **R2** for static assets (10GB free)
- **localStorage** for client state

## why it works

- separation of concerns means each free tier is well-used
- you actually learn the *limits*, not just the happy path
- "what would I do if this ran out tomorrow" is a great design constraint

> the best engineering decision I made this year was assuming no budget.
