# Phase 0 Model Routing System

Configuration layer for LLM routing and orchestration (EP1–EP10).

## Files
- models.yaml → model catalog (tiers, pricing, capabilities)
- providers.yaml → API providers + rate limits + env-based keys
- rules.yaml → routing logic (intent/keyword/agent rules)
- intents.yaml → intent taxonomy + tier mapping

## Notes
- Strict JSON Schema validation enabled (unknown keys rejected)
- No plaintext secrets (uses ${ENV_VAR})
- Supports tier-based routing: fast / standard / powerful

## Status
Phase 0 complete and schema validated.
