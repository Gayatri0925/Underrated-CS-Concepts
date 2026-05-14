## Day 22 – Split Brain Problem

Split Brain occurs when multiple nodes in a distributed system believe they are the leader simultaneously.

### Problem
Network partition breaks communication between nodes.

Both sides assume:
- "I am the leader"

This creates:
- Conflicting writes
- Data inconsistency
- Duplicate operations

### Example
Cluster:
- Node A → Leader
- Node B → Replica

Network partition occurs:
- A still acts as leader
- B promotes itself to leader

Now two leaders exist.

### Why it matters
- Corrupts distributed state
- Creates conflicting truths
- Dangerous in databases and clusters

### Solutions
- Quorum voting
- Consensus algorithms
- Leader election
- Fencing tokens

### Key Idea
Communication failure can create multiple conflicting leaders.

<img width="800" height="800" alt="ipTRamyGJJlFtmFZhRzt3f5lBVzqa2pxIzkNmD0MPgcuPvo81z7In7EfmEaqD0ESFKe0-0i9YsFVbHL8Rg1_s1T1UfnUY5p04TcB77Mb320Py2WofMlu4SDUqi2TpwPOonznhTW4q-6MG_UoaD2yb_fvoilgDr6lc2vNGe5mxX4" src="https://github.com/user-attachments/assets/068b78f3-f191-4ef6-9981-2e02bf300d25" />
