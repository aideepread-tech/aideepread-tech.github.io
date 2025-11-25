# Contribution 2: Self-Modifying Architectures

Taking advantage of NL's insights, the paper presents a novel sequence model that learns how to modify itself by learning its own update algorithm.

---

This builds on the idea that the update rules themselves can be parameterized and learned, rather than being fixed (like standard backpropagation).

The model becomes **self-referential**, where one part of the network learns the algorithm that another part of the network uses to update its weights.

This concept is embodied in architectures like **Titans**, which learn to memorize and adapt at test time.