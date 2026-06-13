# Contributing to MindCore

Thank you for your interest in contributing. MindCore is a cognitive memory architecture — it needs both algorithmic rigor and philosophical clarity.

## How to Contribute

1. **Fork** the repository
2. **Create a branch** for your feature or fix (`git checkout -b feature/your-feature`)
3. **Make your changes** with clear, descriptive commit messages
4. **Submit a Pull Request** with a detailed explanation of what and why

## Code Standards

- Python code follows PEP 8
- All memory operations must be thread-safe
- Boundary checks must use deterministic thresholds (no probabilistic "maybe" verdicts)
- New cognitions must trace back to their source trajectories
- The four-tier architecture (L0→L1→L2→L3) must not be bypassed

## Design Principles

When contributing, please respect the system's core invariants:

- **Trajectory = Boundary**: every rule hardened from experience
- **Cognition is causal**: no black-box decisions
- **Safety is structural**: boundaries live in the architecture, not in prompts
- **Evolution is continuous**: the system learns without retraining

## Security

This project implements AI safety at the architecture level:

- **Never introduce backdoors** or debug bypasses in boundary checking
- Maintain the **four-tier memory isolation**
- All new safety rules must use **deterministic numerical thresholds**
- KAIST pathway gating must respect competitive inhibition (no silent overrides)

## Discussion

For design philosophy discussions and architectural questions, open an Issue with the `discussion` label.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
