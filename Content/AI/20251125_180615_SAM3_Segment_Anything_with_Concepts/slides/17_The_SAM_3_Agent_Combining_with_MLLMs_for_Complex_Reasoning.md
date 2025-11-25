# The SAM 3 Agent: Combining with MLLMs for Complex Reasoning

To handle queries beyond simple noun phrases, we use SAM 3 as a tool within a larger agentic system.

**How it Works:**
1.  An **MLLM (e.g., Gemini, Llama) acts as the 'brain'**.
2.  It receives a complex user query (e.g., "the car door the owner is least likely to use").
3.  The MLLM breaks the problem down and proposes simple **noun phrase queries** to SAM 3.
4.  SAM 3 executes the query and returns masks.
5.  The MLLM analyzes the masks and iterates until the user's goal is met.

**Performance:** This **SAM 3 Agent** achieves new **zero-shot SOTA** results on reasoning segmentation benchmarks like **ReasonSeg** and **OmniLabel**.