## Day 18 – Request Coalescing

Request Coalescing is a technique where multiple identical requests are combined into a single request to reduce duplicate work.

### Problem
When many users request the same data:
- Multiple identical requests hit backend
- Database load increases
- Performance drops

### Solution
Merge identical requests into one and share the response.

### Example
100 users request same data:
- Without coalescing → 100 DB calls
- With coalescing → 1 DB call + shared response

### Why it matters
- Reduces duplicate work
- Improves performance
- Saves backend resources
- Prevents traffic spikes

### Where used
- Caching systems
- API gateways
- CDN edge servers
- High traffic endpoints

### Key Idea
Process once, serve many.
![1pHvqA8MwontA9APdh26wjHYD8_gIOGNqWi20ECXDgq0HqhcRbn10wtjSybdo7FETvkhBgqjHA-d0jwMQswmg73P01aPLi72-sNTRNROindSkNq5Ofszu5jqoGOVAmR1PWRfoN3WFfZg4x9VXzfGnnvAR5B3rGVL6JaJy0CEwbokKw34nzMhOaixGLUPpW9T](https://github.com/user-attachments/assets/05d706cb-f375-444b-a706-f17cea987d21)
