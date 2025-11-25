# The Core Challenge: Navigating Visual and Semantic Ambiguity

The open-vocabulary nature of PCS introduces significant ambiguity that the model must handle:

*   **Semantic Ambiguity:**
    *   **Polysemy:** Phrases with multiple meanings (e.g., "mouse" as an animal vs. a device).
    *   **Subjectivity:** Descriptors that are subjective (e.g., "large car", "cozy room").

*   **Visual Ambiguity:**
    *   **Boundary Definition:** Where does an object end (e.g., does a 'mirror' include its frame?).
    *   **Physical Factors:** Occlusion, blur, and lighting can obscure object boundaries.

**Our Approach:** We address this through multi-expert annotations, adapted evaluation metrics, and a dedicated ambiguity module in the model.