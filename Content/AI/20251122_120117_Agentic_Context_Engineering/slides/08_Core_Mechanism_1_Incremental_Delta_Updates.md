# Core Mechanism 1: Incremental Delta Updates

To prevent context collapse, ACE avoids monolithic rewrites. Instead, it uses **incremental delta updates**.

- **Structured Context:** The context is not a single block of text, but a collection of structured, itemized bullets (e.g., a strategy, a concept, a failure mode).
- **Localized Edits:** The Reflector proposes changes as a small `delta context` containing only new or modified bullets.
- **Deterministic Merge:** The Curator uses lightweight, non-LLM logic to merge these deltas into the main context.

This ensures that past knowledge is preserved while new insights are steadily appended, enabling scalability and preventing information loss.