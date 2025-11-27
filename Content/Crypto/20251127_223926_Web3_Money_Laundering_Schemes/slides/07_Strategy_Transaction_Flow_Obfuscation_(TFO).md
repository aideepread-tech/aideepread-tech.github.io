# Strategy: Transaction Flow Obfuscation (TFO)

**Goal:** To increase the complexity of the transaction graph, making forensic analysis difficult and error-prone.

**Core Method:** Moving illicit assets through a series of wallets controlled by the same actor to mimic legitimate transactional patterns.

### Common TFO Patterns:
- **Multi-hop Transfers:** Routing funds through numerous intermediary wallets to create long, confusing chains.
- **Peeling Chains:** Incrementally sending small amounts to a destination while returning the large remainder to a new, self-controlled address.
- **Distributing & Sweeping:** Splitting large sums into many small outputs or, conversely, consolidating many small inputs into a single large one.
- **Dusting & Address Poisoning:** Sending negligible amounts of crypto to thousands of wallets to disrupt analysis or trick users into sending funds to wrong addresses.