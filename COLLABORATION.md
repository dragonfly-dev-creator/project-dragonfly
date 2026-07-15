Project Dragonfly: Global Developer Recruitment & Core Contribution Guide

Project Dragonfly is an open-source, localized text-retrieval engine designed from the ground up for total user metadata isolation. We have established the high level system architecture, the directory layout, and the initial low-level Rust safeguards for amnesiac memory allocation.

We are actively recruiting a core team of software engineers, database architects, and systems developers to build out the alpha execution pipeline.

Open Engineering Roles

1. Lead Backend Systems Engineer (Rust)
Objective: Own the implementation of the memory mapped file pipeline (`mmap`) and optimize the custom memory allocation wrapping.
  Focus: Integrating the `zeroize` crate structures and managing heap to stack lifecycles.

2. Database Core Architect (LSM Tree Implementation)
Objective: Build the Log-Structured Merge-tree storage engine capable of sequentially indexing up to 3 TB of raw text.
Focus: Tuning Size Tiered compaction strategies to minimize write amplification and preserve consumer SSD hardware longevity.

3. P2P Network Protocol Engineer
Objective: Engineer the decentralized data ingestion pipeline.
  Focus: Abstracting socket transport layers to mandate Tor onion routing and I2P garlic proxies, using randomized timing jitter to break traffic analysis.

How to Join the Team
Project Dragonfly operates as a sovereign, collaborative open-source collective. If you have production-grade experience in systems languages, database theory, or network isolation, we invite you to review our specs in `DRAGONFLY_ARCHITECTURE.md`.

To apply for a core role or coordinate on development:
1. Open an Issue detailing your technical background.
2. Submit a Pull Request targeting open modules inside the `/src` tree.
3. Coordinate directly with the Product Architecture lead via repository management.
