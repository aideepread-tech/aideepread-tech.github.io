# Ablation Studies: What Makes SAM 3 Effective?

We conducted extensive ablations to validate our design choices.

**Key Findings:**
*   **Presence Head:** Decoupling recognition and localization boosts `cgF1` by **+1.5 points** by significantly improving image-level recognition (IL_MCC).

*   **Hard Negatives:** Training with adversarial negative phrases is crucial for classification, improving IL_MCC from **0.44 to 0.68**.

*   **Training Data:**
    *   Our high-quality human-in-the-loop data (**SA-Co/HQ**) provides the biggest performance lift.
    *   Large-scale synthetic data (**SA-Co/SYN**) also provides significant gains over external datasets.