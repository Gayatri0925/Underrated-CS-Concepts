## Day 11 – Circuit Breaker Pattern

The Circuit Breaker Pattern prevents cascading failures in distributed systems.

### States
- **Closed** → Requests flow normally  
- **Open** → Fail fast, block requests  
- **Half-Open** → Allow limited test requests  

### Why it matters
- Prevents system-wide outages  
- Improves resilience  
- Enables graceful degradation  
- Reduces latency during failures

- <img width="1024" height="1536" alt="ChatGPT Image Mar 26, 2026, 06_29_02 PM" src="https://github.com/user-attachments/assets/e041a2a1-c606-4884-8def-79134ed4a842" />
