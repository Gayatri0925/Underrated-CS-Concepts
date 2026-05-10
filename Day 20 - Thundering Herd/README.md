## Day 20 – Thundering Herd Problem

The Thundering Herd Problem occurs when many clients or processes access the same resource simultaneously, causing sudden overload.

### Problem
Large numbers of requests wake up together:
- Cache expires
- Service recovers
- Retries triggered simultaneously

This creates:
- Traffic spikes
- Resource contention
- System overload

### Example
1000 clients retry together after timeout:
- Database flooded
- Latency spikes
- Cascading failures begin

### Solutions
- Exponential backoff
- Randomized delays
- Request coalescing
- Rate limiting
- Queueing

### Why it matters
- Prevents sudden overload
- Improves stability
- Protects backend systems

### Key Idea
Synchronized traffic spikes can overwhelm systems instantly.
<img width="1200" height="655" alt="RJkXSIwkdt13sb1mfFa8FwFOv6frR4ap3z4ZHEqz63AyAN3FMAyH7aA7UJzdnxbl9-O2m1vAH1fmUh46zVxGvuz7fB_n1f26n9bQwzCBhtpQPzuKmVZ4nLLkSQUc121WPjahP7F9eMmpY9LIQEkAeyhliXObO4AQmeTl3KyG52M" src="https://github.com/user-attachments/assets/9eaf1a31-4652-4aa3-982a-2da6fd3da6b4" />
