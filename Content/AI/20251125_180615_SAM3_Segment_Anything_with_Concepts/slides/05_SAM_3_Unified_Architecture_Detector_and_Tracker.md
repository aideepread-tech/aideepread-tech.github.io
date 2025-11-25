# SAM 3: Unified Architecture (Detector and Tracker)

SAM 3 employs a dual encoder-decoder transformer architecture built upon the SAM and DETR series.

**Core Components:**

*   **Shared Backbone (Perception Encoder - PE):** A single, powerful vision-language encoder that processes both image/video frames and text prompts.
*   **Detector (for Images):** A DETR-based model that performs open-vocabulary detection and segmentation based on concept prompts.
*   **Tracker (for Videos):** Inherits from SAM 2's architecture, responsible for propagating masks and maintaining object identities over time.

This decoupled design avoids task conflict, allowing the detector to be identity-agnostic while the tracker focuses on separating identities.