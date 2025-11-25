# Defining the Task: Promptable Concept Segmentation (PCS)

**Objective:** Given an image or video, detect, segment, and track all instances of a visual concept.

**Allowed Prompts:**

1.  **Text:** A short noun phrase (NP) describing the concept (e.g., "red apple", "striped cat").
2.  **Image Exemplars:** Bounding boxes on specific frames, marked as positive or negative examples.
3.  **Combination:** Use both text and image exemplars for refinement.

**Output:** Instance masks and unique tracking IDs for every object matching the concept prompt, preserving identity across video frames.