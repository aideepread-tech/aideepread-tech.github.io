# Contribution 1: Optimizers as Learning Modules

NL reveals that well-known gradient-based optimizers are themselves learning modules.

---

*   **SGD with Momentum:** A 2-level system where the momentum term is a key-less associative memory that stores a history of gradients.
*   **Adam Optimizer:** Can be shown to be an optimal associative memory for the model's gradients.

### Building More Expressive Optimizers

This insight allows us to design better optimizers by enhancing the underlying memory module:

*   **More Expressive Association:** Use preconditioning (`P_i`) to give the memory meaningful values to associate with gradients.
*   **More Expressive Objectives:** Use L2 regression instead of dot-product similarity for the update rule (Delta Rule).
*   **More Expressive Memory:** Replace the linear momentum memory with a deep one (e.g., an MLP), resulting in **Deep Momentum Gradient Descent (DMGD)**.