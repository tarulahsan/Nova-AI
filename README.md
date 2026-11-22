# NOVA Frontier v0.4.3

Compact, scratch-initialized hybrid language/vision model research project with a permissioned agent runtime, provenance-aware memory, verifier-driven training and an operational self-model.

> **Status:** engineering research implementation, not a pretrained frontier model. No trained 1B checkpoint is included. A $30 Modal L4 pilot has not yet been run.

## Release artifacts

- [Complete source archive](releases/NOVA-Frontier-v0.4.3.zip)
- [Portable Git bundle with history and v0.4.3 tag](releases/NOVA-Frontier-v0.4.3.bundle)
- [SHA-256 checksums](releases/SHA256SUMS.txt)

The ZIP contains the committed source, configs, tests and documentation. The bundle can be cloned locally to recover the repository history and tag.

## Project facts

- Target: approximately 1B parameters; 3B is incompatible with the 150,000,000-byte package ceiling at one-bit raw weights.
- Package objective: <=150,000,000 bytes, non-ternary; actual trained binary-QAT export and quality retention are not yet validated.
- Modal compute ceiling: USD 30; first experiment is a bounded L4 feasibility/throughput pilot.
- Teacher-generated text/code/reasoning/agent data is allowed as optional supervision only when dataset/output terms and underlying source/record rights are documented. Teacher weights are not imported. Teacher targets are not ground truth.
- OpenCodeReasoning-2 blank questions require a pinned upstream question index.
- Long proof/agent records are chunked by message boundary with token-window fallback; default tokenization does not silently truncate.
- Orchard is retained as a candidate but held until the publisher restores its temporarily paused release.

## Reproducible checks

See the source archive for commands and reports. Release v0.4.3 passes 118 CPU tests, compilation, project/data/dataset validators, a tiny temporary CPU training/inference smoke and a package-wheel build. These checks do not establish L4 fit, production deployment, learned capabilities or frontier benchmark results.

## Safety, provenance and licensing

Do not commit API keys, private data, downloaded corpora, model checkpoints or raw teacher datasets to this repository. Every corpus retains its own license and attribution requirements. Dataset-card licenses do not automatically clear embedded repositories, source code, problem statements, GUI screenshots or other assets. Use pinned revisions and source-rights manifests.

NOVA's self-model is operational introspection of inspectable identity/configuration/checkpoint/tool/evaluation facts; it is not a claim of subjective consciousness.

## License

NOVA source code: Apache-2.0. Training datasets and embedded assets retain their respective upstream licenses and obligations.
