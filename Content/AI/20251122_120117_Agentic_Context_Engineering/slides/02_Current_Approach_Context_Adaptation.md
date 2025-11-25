# Current Approach: Context Adaptation

Context adaptation refers to methods that improve model behavior by constructing or modifying the inputs to an LLM, rather than altering its weights.

**Key Advantages:**
- **Interpretability:** Contexts are human-readable and explainable.
- **Agility:** Allows for rapid integration of new knowledge at runtime.
- **Modularity:** Can be shared across different models or systems.

**Common Methods:**
- Refining system prompts.
- Using in-context learning (ICL) with examples.
- Building an external memory of strategies (e.g., Dynamic Cheatsheet).
- Iterative optimization based on execution feedback (e.g., GEPA, Reflexion).