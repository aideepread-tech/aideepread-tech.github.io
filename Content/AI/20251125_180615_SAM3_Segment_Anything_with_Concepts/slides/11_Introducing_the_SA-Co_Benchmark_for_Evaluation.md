# Introducing the SA-Co Benchmark for Evaluation

To rigorously evaluate Promptable Concept Segmentation, we created the **Segment Anything with Concepts (SA-Co) Benchmark**.

**Key Statistics:**
*   **207,000** unique concept phrases
*   **121,000** images and **1,700** videos
*   **>50x more concepts** than existing benchmarks like LVIS.
*   Exhaustive masks and a high volume of hard negative labels.

**Evaluation Splits:**
*   **SA-Co/Gold:** Highest quality, with 3 independent annotations per sample to measure human performance and handle ambiguity.
*   **SA-Co/Silver, Bronze, Bio:** Cover a wide range of 10+ domains (e.g., driving, medical, robotics).
*   **SA-Co/VEval:** Dedicated split for video evaluation.