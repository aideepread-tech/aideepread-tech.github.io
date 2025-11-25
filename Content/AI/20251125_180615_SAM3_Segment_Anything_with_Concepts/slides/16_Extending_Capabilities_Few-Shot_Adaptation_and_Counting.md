# Extending Capabilities: Few-Shot Adaptation and Counting

SAM 3 demonstrates strong transfer learning and extended abilities.

*   **Few-Shot Object Detection:**
    *   Evaluated on diverse, in-the-wild datasets (ODinW13, RF100-VL).
    *   Achieves **state-of-the-art 10-shot performance**, surpassing specialized detection models like gDino and in-context learning with Gemini.

*   **Object Counting:**
    *   Evaluated on CountBench and PixMo-Count.
    *   Achieves excellent accuracy, outperforming several MLLMs (e.g., Gemini 2.5 Pro, Qwen2-VL-72B).
    *   A key advantage: SAM 3 provides not just the count, but also the segmentation masks for each counted object.