# Innovation 2: Interactive Refinement with Image Exemplars

SAM 3 enhances interactivity beyond the visual prompts of SAM 1 & 2.

*   **Prompt Type:** Users can provide bounding boxes labeled as **positive** or **negative** examples.
*   **Function:** Unlike PVS where a prompt yields one mask, an exemplar prompt in PCS guides the model to find **all instances** that match the example.
    *   **Example:** Providing a positive box on one dog prompts the model to detect *all* dogs in the image.
*   **Use Case:** Ideal for resolving ambiguities or correcting errors (false positives/negatives) from an initial text prompt.
*   **Interactivity:** Exemplars can be added iteratively to refine the results.