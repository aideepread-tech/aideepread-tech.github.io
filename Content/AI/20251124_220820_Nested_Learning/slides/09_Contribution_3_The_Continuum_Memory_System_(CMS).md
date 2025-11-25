# Contribution 3: The Continuum Memory System (CMS)

CMS generalizes the traditional binary view of long-term vs. short-term memory.

---

Instead of one fast working memory (attention) and one slow persistent memory (MLP), CMS proposes a **chain of memory modules**, each operating at a different frequency.

`y_t = MLP^(f_k)(...MLP^(f_1)(x_t)...)`

*   Each MLP block `MLP^(f_l)` is associated with a specific update frequency `f_l`.
*   Faster-frequency blocks (like `f_1`) are updated more often, capturing recent context.
*   Slower-frequency blocks (like `f_k`) are updated infrequently, capturing more abstract, long-term knowledge.

This creates a spectrum of memory persistence and abstraction within the model.