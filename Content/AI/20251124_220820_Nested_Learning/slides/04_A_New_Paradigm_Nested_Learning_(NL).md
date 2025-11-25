# A New Paradigm: Nested Learning (NL)

Nested Learning represents a model and its training procedure as a set of nested, multi-level, and/or parallel optimization problems.

---

### Key Idea:

Instead of a single, flat architecture with one training loop, NL views a model as an integrated system where different components learn at different speeds and on different types of information.

*   Each component has its own **"context flow"** and **update frequency**.
*   This reveals the hidden computational depth and inner gradient flows within existing models (like Transformers).
*   It provides a path to design more expressive learning algorithms with more "levels."

![Nested Learning Paradigm](https://cdn-mineru.openxlab.org.cn/result/2025-11-24/cbe03578-fa5a-435c-a00d-6aaf72ec8da0/dabc572dc61251dcb4053d54b39ffb178b52505daef928d58473a0b112fe60ba.jpg)