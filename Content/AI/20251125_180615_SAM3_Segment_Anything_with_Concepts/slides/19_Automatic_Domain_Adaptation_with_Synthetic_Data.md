# Automatic Domain Adaptation with Synthetic Data

**Challenge:** How to adapt SAM 3 to a new, specialized domain (e.g., "Food&Drink") without costly human annotation?

**Solution:** Use the data engine to generate **domain-specific synthetic data**.

*   The SAM 3 teacher model and AI verifiers, even without being trained on the new domain, can generate a large-scale, high-quality synthetic dataset (SA-Co/SYN-Food).

**Result:**
*   Fine-tuning on this synthetic data shows a **similar scaling behavior and performance** as fine-tuning on expensive, human-annotated data (SA-Co/HQ-Food).
*   This demonstrates a scalable path to improve performance on new data distributions with zero human annotation cost.