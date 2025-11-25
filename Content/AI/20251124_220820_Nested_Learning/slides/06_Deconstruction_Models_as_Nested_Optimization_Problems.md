# Deconstruction: Models as Nested Optimization Problems

NL reveals that seemingly simple training processes are already multi-level optimization problems.

---

### Example 1: Training an MLP with Momentum

*   **Level 1 (Outer Loop):** The model weights `W` are updated.
*   **Level 2 (Inner Loop):** The momentum term `m` is itself an associative memory that compresses past gradients. It has its own, faster optimization process.

### Example 2: Linear Attention

*   **Level 1 (Outer Loop):** The projection matrices `W_k, W_q, W_v` are trained (slow updates).
*   **Level 2 (Inner Loop):** The attention matrix `M` is updated with each new token, acting as a fast memory that compresses key-value pairs.

This decomposition is based on **update frequency**, creating a hierarchy of learning speeds within the model.