## Day 19 – Cache Stampede

Cache Stampede occurs when multiple requests hit the backend simultaneously after a cache expires.

### Problem
When cache expires:
- All requests miss cache
- All hit database at once
- System overload

### Example
1000 users request same data after cache expiry:
- 1000 DB calls triggered

### Solutions
- Request coalescing
- Cache locking
- Staggered expiry
- Background refresh

### Why it matters
- Prevents traffic spikes
- Protects backend systems
- Improves stability

### Key Idea
Avoid simultaneous cache misses.
<img width="1290" height="860" alt="nfaH7Ag-qf6FjGRJryPCnd7DX1KpKLVrc5ZMwBBxVRqNleplt7qup8atHfycMP4YsRloHG7JVIVb22q65r2K8tr_-Swo4f0ItOYkzsyCJNea0CBoI0ZhIRiJcFOciHLyzkJMmejd2fQhyq4jp7Aylk85ZP_WiQxsiyQSSDK-qZ8" src="https://github.com/user-attachments/assets/160f6d28-9813-4b0e-bcf9-bf17a9185226" />
