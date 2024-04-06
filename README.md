## otel-cf-workers broken reproduction

The issue: otel-cf-workers span doesn't get propagated correctly.

To reproduce:

```
pnpm install
pnpm dev

curl http://localhost:8787

# Verify in worker console output that you get `Active span context: undefined`
```
