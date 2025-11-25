# Experimental Validation

To test its effectiveness, HOPE was evaluated against strong baselines on a range of standard benchmarks.

---

### Tasks:
1.  **Language Modeling:**
    *   WikiText-103 (ppl ↓)
    *   LAMBADA (ppl ↓, acc ↑)
2.  **Common-Sense Reasoning:**
    *   PIQA, HellaSwag, WinoGrande, ARC, SIQA, BoolQ (acc ↑)

### Baselines:
*   Transformer++
*   Modern RNNs: RetNet, DeltaNet, Samba, Titans

### Scales:
Models were compared at multiple parameter counts: 340M, 760M, and 1.3B.