# Key Data Engine Features: AI Annotators and Verifiers

We delegate key annotation tasks to specialized AI models, dramatically increasing efficiency.

*   **AI Annotators (Proposers):**
    *   Leverage Multimodal LLMs to generate diverse and relevant **noun phrases (NPs)** for images.
    *   Propose **hard negatives** (adversarial phrases that are not in the image) to improve model robustness.

*   **AI Verifiers (Checkers):**
    *   Fine-tuned MLLMs that perform **Mask Verification (MV)** and **Exhaustivity Verification (EV)** with near-human accuracy.
    *   Automatically filter correctly labeled examples, focusing human effort on fixing complex errors.

**Impact:** The introduction of AI verifiers **doubled the data engine's throughput** compared to a human-only pipeline.