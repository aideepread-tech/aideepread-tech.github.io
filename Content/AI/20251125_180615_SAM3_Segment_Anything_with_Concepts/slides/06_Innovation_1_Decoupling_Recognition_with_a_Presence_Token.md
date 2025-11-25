# Innovation 1: Decoupling Recognition with a Presence Token

**Problem:** A single object query struggles to simultaneously recognize **(what)** and localize **(where)** an object, as recognition requires global context while localization is inherently local.

**Solution: The Presence Token**

*   We introduce a learned, global **presence token**.
*   **Responsibility:** Its sole job is to predict whether the target concept (noun phrase) is present *anywhere* in the image.
*   **Object Queries:** Freed from the recognition task, object queries can focus purely on the localization problem: `p(query is a match | concept is present)`.

This decoupling significantly improves detection accuracy, especially for challenging negative phrases.