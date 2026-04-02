## Day 14 – Backpressure

Backpressure is a mechanism where a system controls incoming traffic when it cannot handle more load.

### Problem
When incoming rate > processing capacity:
- Queue builds up
- Latency increases
- System crashes

### Solution
Apply backpressure:
- Reject extra requests
- Slow down producers
- Control flow rate

### Where used
- Kafka, streaming systems
- APIs under load
- Reactive programming

### Key Idea
Never accept more load than you can process.

![1_ZQWlVVyCANAmgUKJU9xUlw](https://github.com/user-attachments/assets/98d98040-dadf-4746-b61a-ed96473c1ea5)

<img width="1536" height="1024" alt="ChatGPT Image Apr 2, 2026, 06_38_03 PM" src="https://github.com/user-attachments/assets/7d9e31e7-7c7b-4bcc-8676-3d3a501d6d11" />

