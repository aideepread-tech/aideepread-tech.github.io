# Limitation 1: The Brevity Bias

Many current context adaptation methods suffer from a **brevity bias**.

- **Problem:** The optimization process tends to favor short, generic instructions over comprehensive, detailed ones.
- **Example:** An optimizer might repeatedly produce a simple prompt like `"Create unit tests"` while omitting domain-specific heuristics, failure modes, or complex tool-use guidelines.
- **Impact:** This sacrifices the very details and diversity needed for high performance in complex, knowledge-intensive domains like agentic systems or programming.