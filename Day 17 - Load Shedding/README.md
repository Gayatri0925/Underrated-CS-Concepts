## Day 17 – Load Shedding

Load Shedding is a technique where a system intentionally drops low-priority requests during overload to protect critical functionality.

### Problem
When traffic spikes:
- CPU usage increases
- Queues build up
- System slows down
- Eventually crashes

### Solution
Drop non-critical requests and serve important ones.

### Example
During heavy traffic:
- Checkout → allowed
- Login → allowed
- Recommendations → dropped
- Analytics → skipped

### Why it matters
- Prevents total system failure
- Protects critical services
- Improves stability
- Maintains user experience

### Where used
- API gateways
- Microservices
- Payment systems
- High traffic platforms

### Key Idea
Serve important requests first, drop the rest.
![twxLgMNkqyjwJmgM3IQYAZePyJ_wHScLpGsEAAq0gdEImdcHRZZb3R_4gfuSRUDO_yVTI2m22RpNykF0wcqjXat4yCNF86ylNan728N1tW3_YYDdpP1AIJOFBNh7lXnNXeuBHPYJk24NyeYKdz6IFkL_n6MqgRh4gEBOaJ44ZTxltMuRtjLPXi8rnobUBoe3](https://github.com/user-attachments/assets/20e8dbfc-a134-4ea2-a3f6-4d6f8e11f085)
