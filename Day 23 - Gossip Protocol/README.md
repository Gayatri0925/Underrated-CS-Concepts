## Day 23 – Gossip Protocol

Gossip Protocol is a communication mechanism where nodes spread information gradually across a distributed system.

### Problem
Large clusters cannot broadcast updates to every node directly.

Broadcasting creates:
- Network overhead
- Scalability issues
- High communication cost

### Solution
Spread information incrementally.

Example:
Node A → Node B  
Node B → Node C  
Node C → Node D  

Eventually all nodes receive the update.

### Where used
- Distributed databases
- Cluster membership
- Failure detection
- Service discovery

### Why it matters
- Scales efficiently
- Reduces network traffic
- Improves fault tolerance

### Key Idea
Information spreads through the cluster like rumors.
<img width="1152" height="608" alt="wUegYbStqwmGjSFgGfGJFqPwPVk5aGXBCblOG6Y5sVfNvlEWqw1S_mCoF6AMe3erjnHC_zE7-4HScawwgCaiZSxWN6aabhG10mX8WRCpW0rJvHkIgUiNpQcMOijNKB5CnvujN7TsILIoF1BaOSxa1QoBB2nZ8lgTd5Tg036EgIk" src="https://github.com/user-attachments/assets/4cb483af-b228-4786-9807-f9d024a137a6" />
