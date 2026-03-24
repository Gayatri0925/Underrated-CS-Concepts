# Day 1 — Bloom Filter

## Idea in one line
Check if something **probably exists** using almost no memory.

## Why it’s interesting
- Extremely space efficient
- Fast membership checks
- No storage of actual values

## Where it's used
- Database query filtering
- Web cache systems
- Spam detection

## How it works
Multiple hash functions mark positions in a bit array.  
Query checks those positions.

## Complexity
Time: O(k)  
Space: O(m)

## When to use
When you need **fast existence checks** for huge datasets.
