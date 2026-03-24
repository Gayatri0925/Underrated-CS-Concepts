# Day 9 — Idempotency

## Idea in one line
Same request → same result, no duplicates.

## Why it’s interesting
- Prevents duplicate operations
- Reliable distributed systems
- Safe retries

## Where it's used
- Payment systems
- APIs
- Distributed services

## Example
Retrying payment should not charge twice.
