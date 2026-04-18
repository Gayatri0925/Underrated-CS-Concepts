## Day 15 – Retry with Exponential Backoff

Retry with Exponential Backoff is a technique where a system retries failed requests with increasing delay between attempts.

### Problem
When requests fail, immediate retries can overload the system.

Example:
- Thousands of clients retry instantly
- Traffic spikes
- System fails further

### Solution
Increase delay between retries.

Example delays:
- 1st retry → 1 second
- 2nd retry → 2 seconds
- 3rd retry → 4 seconds
- 4th retry → 8 seconds

### Why it matters
- Reduces retry storms
- Prevents cascading failures
- Gives system time to recover
- Improves reliability

### Where used
- API retries
- Microservices communications
- Cloud SDKs (AWS, GCP)
- Database connections

### Simple Example (Pseudo)
retry = 0
delay = 1

while retry < 5:
if request_success():
break
sleep(delay)
delay = delay * 2
retry += 1

### Key Idea
Retry intelligently, not immediately.
