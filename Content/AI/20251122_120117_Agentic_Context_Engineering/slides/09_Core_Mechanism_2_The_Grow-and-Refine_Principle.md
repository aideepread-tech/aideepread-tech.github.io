# Core Mechanism 2: The Grow-and-Refine Principle

ACE ensures contexts remain relevant and non-redundant through a **grow-and-refine** mechanism.

1.  **Grow:**
    - New insights (bullets) are appended to the context.
    - Existing bullets are updated in-place with new metadata (e.g., usage counters).

2.  **Refine:**
    - A de-duplication step periodically prunes redundancy by comparing bullets using semantic embeddings.

This process allows the context to expand adaptively while maintaining compactness and relevance, avoiding the variance of complete rewrites.