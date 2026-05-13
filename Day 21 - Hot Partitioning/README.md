## Day 21 – Hot Partitioning

Hot Partitioning occurs when one partition receives significantly more traffic than others in a distributed system.

### Problem
Evenly distributed systems can still fail if:
- One partition becomes overloaded
- Traffic concentrates on specific data

### Example
Millions of users access:
- Same viral post
- Same hashtag
- Same product during flash sale

One partition becomes overloaded while others stay idle.

### Effects
- High latency
- Uneven load distribution
- Resource exhaustion
- Scalability bottlenecks

### Solutions
- Better partition keys
- Randomized sharding
- Dynamic rebalancing
- Caching hot data

### Key Idea
Uneven traffic distribution creates bottlenecks in distributed systems.
<img width="1400" height="740" alt="dBFSuHFJLAad6H5n9jlUMVpjVMHgW8C1_0im3JLJhkEfo1qxAMY4lDQykyztJfafu9Mkvc5sF4TcJoaoVpKopytuujy2nFv7UrW2MOAxi9gBVuxnux78GnAAhQJ7yQ3MWHGHQja4BxTvp5Hksyvkl5nLpup_zh9Vcou7OqCEbTs0srsjRJWPG45pydb4gFNu" src="https://github.com/user-attachments/assets/d5a6e1e3-4d30-4bd6-8258-9e92033c47d3" />
