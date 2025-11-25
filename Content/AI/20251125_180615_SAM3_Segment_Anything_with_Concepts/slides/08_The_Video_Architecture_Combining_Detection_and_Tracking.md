# The Video Architecture: Combining Detection and Tracking

SAM 3 processes videos by integrating its detector and tracker in a frame-by-frame loop:

1.  **Detect:** On the current frame `t`, the **detector** finds all new objects `O_t` matching the concept prompt.
2.  **Propagate:** The **tracker** takes the existing tracked masks (masklets) from the previous frame `M_{t-1}` and predicts their new locations `M_hat_t` on the current frame.
3.  **Match & Update:** A matching function associates the propagated masks `M_hat_t` with the new detections `O_t`.
    *   Matched objects are updated.
    *   Unmatched new detections spawn new masklets.

To handle ambiguities in crowded scenes, the system uses temporal disambiguation strategies and periodically re-prompts the tracker with high-confidence detections.