# Limitation 2: Context Collapse

A more severe issue is **context collapse**, where iterative rewriting of the context leads to a sudden and dramatic loss of information.

- **Cause:** When an LLM is tasked with rewriting a large, accumulated context, it often compresses it into a much shorter, less informative summary.
- **Case Study:** In one experiment, a context of **18,282 tokens** (66.7% accuracy) collapsed to just **122 tokens** in the next step, causing accuracy to plummet to 57.1%.
- **Risk:** This demonstrates that monolithic, end-to-end rewriting can abruptly erase valuable, accumulated knowledge.