# Ethereum Proof-of-Stake Consensus Spec Tests

This repository contains test vectors for the Ethereum [Proof-of-Stake Consensus Spec](https://github.com/ethereum/consensus-specs).
Other types of testing (network, fuzzing, benchmarking, etc.) are currently a work in progress, and will be hosted in separate repositories.
The intention of this repository is to provide a solid base for Ethereum proof-of-stake clients (aka "beacon nodes") to consume as part of their unit-testing efforts around spec behavior.

The tests are YAML files following the [general testing format](https://github.com/ethereum/consensus-specs/tree/master/tests/formats).

The generators that are responsible for generating all of the spec tests can be found in [ethereum/consensus-specs/test_generators](https://github.com/ethereum/consensus-specs/tree/master/tests/generators).

New tests can be added by creating a generator in the specs repository, or adding functionality to an existing generator.
Generators are small and easy to write, and can use the [pythonized-spec](https://github.com/ethereum/consensus-specs/tree/master/tests/core/pyspec) to build expected test outputs: 
[see documentation](https://github.com/ethereum/consensus-specs/tree/master/tests/generators#developing-a-generator)

Note that this repository is growing over time as the spec evolves, and more test-generation code is being added.
The YAML test-vectors are tracked using [Git LFS](https://git-lfs.github.com/), 
 to accommodate for large test vectors (Take execution-layer tests repository size as an example). 

## License

See [LICENSE](./LICENSE) file.
