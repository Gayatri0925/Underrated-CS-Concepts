## Day 16 – Hedged Requests

Hedged Requests reduce tail latency by sending a duplicate request after a short delay.

### Problem
Sometimes one server is slow, causing high latency.

### Solution
Send a backup request to another server.
Use whichever response arrives first.

### Example
Request → Server A  
After delay → duplicate request → Server B  
Server B responds first → use response  
Ignore slower one  

### Why it matters
- Reduces tail latency
- Improves response time
- Handles unpredictable slow nodes
- Better user experience

### Where used
- Distributed databases
- Search systems
- Load balanced APIs
- Large-scale microservices

### Key Idea
Send a backup request to avoid waiting for slow responses.

<img width="1200" height="800" alt="1_v1G8I_sSx4zpDnuIqD4pSQ" src="https://github.com/user-attachments/assets/ae126ade-6f92-498e-8243-eff6ee19fdc9" />
