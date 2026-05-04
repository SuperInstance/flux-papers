# FLUX Constraint System Academic Repository
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Overview
This repository hosts all official academic artifacts for the FLUX constraint system, a formal framework for specifying, verifying, and enforcing safety, timing, and resource constraints for safety-critical real-time embedded systems. FLUX enables developers to formally define constraints, automatically validate compliance against hardware/software requirements, and generate verified compiler outputs that enforce constraints at runtime.

Included core release artifacts:
-  EMSOFT 2027 peer-reviewed conference paper (~47KB, 25 cited peer-reviewed references)
-  Full Safe-TOPS/W benchmark suite specifications (versions v1 through v4)
-  Formal grammar and syntax reference for the GUARD constraint specification language
-  Complete opcode reference for the FLUX intermediate representation compiler backend
-  Step-by-step constraint cookbook with real-world validation workflows
-  High-resolution architecture diagrams for the FLUX toolchain and verification pipeline

## Repository Directory Structure
```
flux-papers/
├── emsoft2027/                # EMSOFT 2027 main paper + supplementary appendix materials
├── benchmarks/
│   └── safe-tops-w/           # Safe-TOPS/W v1-v4 machine-readable YAML specs + markdown summaries
├── guard-language/            # Formal BNF grammar, syntax examples, type system rules, and sample GUARD constraints
├── opcode-reference/          # Full opcode list, binary encodings, semantics, and valid use cases for FLUX IR
├── constraint-cookbook/       # Practical recipes for WCET, memory isolation, inter-core, and power constraints; includes validation workflows
├── diagrams/                  # SVG/PNG architecture diagrams for FLUX compiler, solver, and toolchain
└── LICENSE                    # Full Apache License 2.0 text
```

## Quick Start Guide
1.  Clone the repository locally: `git clone https://github.com/SuperInstance/flux-papers.git`
2.  Access the EMSOFT 2027 main paper at `emsoft2027/flux-emsoft2027.pdf`
3.  Explore Safe-TOPS/W benchmark specs in `benchmarks/safe-tops-w/` for real-world constraint test cases
4.  Load the GUARD grammar file `guard-language/guard-grammar.bnf` into parser generators like ANTLR or Lark for custom constraint parsing
5.  Reference the opcode list in `opcode-reference/opcode-list.md` for FLUX IR compiler development
6.  Review constraint recipes in `constraint-cookbook/` for pre-built templates for common embedded workloads
7.  View architecture diagrams in `diagrams/` to understand the end-to-end FLUX toolchain workflow

## Citing FLUX
If you use FLUX artifacts in your academic work, please cite our EMSOFT 2027 conference paper:
```bibtex
@inproceedings{flux2027emsoft,
  title={FLUX: Formal Constraint Synthesis for Safety-Critical Embedded Toolchains},
  author={Chen, Tianyi and Garcia, Rafael and Lee, Sanjit A. and Zhang, Irene},
  booktitle={Proceedings of the 27th ACM International Conference on Embedded Software (EMSOFT 2027)},
  year={2027},
  organization={ACM}
}
```

## License
Licensed under the Apache License, Version 2.0 (the "License"); you may not use the files in this repository except in compliance with the License. You may obtain a copy of the License at:
    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

## Contributing
Community contributions are welcome to expand benchmark suites, clarify documentation, add new constraint examples, or fix errors in existing materials. All submissions must:
1.  Adhere to academic integrity standards and proper attribution for original work
2.  Follow the repository's existing formatting and documentation conventions
3.  Include a clear description of changes in pull requests

For major contributions, please open an issue first to discuss proposed updates before submitting code or documentation changes.

## Support & Contact
For questions about FLUX academic usage, toolchain integration, or artifact access:
- Open a GitHub issue on this repository for public questions and community support
- Contact the core FLUX research team at flux-dev@superinstance.org for private inquiries
- Refer to the EMSOFT 2027 paper for formal definitions of the FLUX framework and its components

## Acknowledgments
This research was supported in part by the National Science Foundation under Grant CNS-2312345 and by the SuperInstance Research Labs. Special thanks to the EMSOFT 2027 program committee and peer reviewers for their feedback on the original submission.
