# New Metrics: Classification-gated F1 (cgF1)

Traditional metrics like Average Precision (AP) are not ideal for open-vocabulary tasks with vast label spaces and high class imbalance.

**We propose `cgF1` to better measure PCS performance:**

`cgF1 = 100 * pmF1 * IL_MCC`

*   **Localization (`pmF1` - positive micro F1):**
    *   Measures mask quality (F1 score) *only* on positive image-phrase pairs.

*   **Classification (`IL_MCC` - Image-Level Matthews Correlation Coefficient):**
    *   Measures the model's ability to correctly predict the *presence or absence* of a concept in an image, regardless of mask quality.

This composite metric rewards both accurate localization and correct recognition.