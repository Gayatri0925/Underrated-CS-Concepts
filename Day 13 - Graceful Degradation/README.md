## Day 13 – Graceful Degradation

Graceful Degradation is a design approach where a system continues to function even when some components fail, but with reduced features.

### Problem
When a non-critical service fails, the entire application should not stop working.

Example:
- Recommendation service down
- Analytics service slow
- Notification service unavailable

Without graceful degradation, the whole system may fail.

### Solution
Continue core functionality while disabling optional features.

Example:
- Show products without recommendations
- Allow checkout without analytics
- Skip notifications but complete transaction

### Why it matters
- Improves user experience
- Prevents complete outages
- Keeps critical features available
- Works well with Bulkhead and Circuit Breaker

### Real-world examples
- Netflix streams video even if recommendations fail
- Amazon allows checkout even if reviews don't load
- Google shows results even if some services are unavailable

### Key Idea
Fail partially, not completely.
