# The Data Engine: A Human-AI Loop for Scalable Annotation

Achieving high performance in PCS requires a massive, diverse dataset. We built an efficient data engine to create it.

**Core Principle:** A synergistic feedback loop that leverages the strengths of models and humans.

**Workflow:**
1.  **Propose:** AI models propose noun phrases (NPs) and candidate masks for a given image/video.
2.  **Verify:** A mix of AI and human verifiers check mask quality and exhaustivity (if all instances are found).
3.  **Correct:** Humans focus on correcting the difficult cases identified by the verifiers.
4.  **Train:** The corrected data is used to train the next version of SAM 3.
5.  **Iterate:** The improved SAM 3 is integrated back into the engine to propose better masks.

This virtuous cycle actively mines challenging data and continuously improves the model.