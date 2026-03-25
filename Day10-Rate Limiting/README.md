# Day 10 — Rate Limiting

## Idea in one line
Control how many requests a client can make within a fixed time window.

## Why it matters
- Prevents server overload
- Protects against abuse
- Ensures fair usage
- Improves reliability

## Common Algorithms
- Fixed Window Counter
- Sliding Window Log
- Token Bucket
- Leaky Bucket

## Real-world usage
- API request limits
- Login attempt restrictions
- Payment system protection
- Messaging spam control

## Example
Allow 100 requests per minute.  
If limit exceeds → return HTTP 429 (Too Many Requests).

## When to use
When designing scalable APIs and distributed systems.

## Key takeaway
Rate limiting protects system stability during traffic spikes.
