# Day 2 — Consistent Hashing

## Idea in one line
Distribute data across servers **without reshuffling everything**.

## Why it’s interesting
- Scales easily
- Handles node failures
- Minimal data movement

## Where it's used
- Distributed caches
- Load balancers
- Microservices sharding

## How it works
Nodes and keys mapped to a hash ring.  
Each key assigned to nearest node.

## When to use
When servers dynamically join or leave.
