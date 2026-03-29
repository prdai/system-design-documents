# algorithm-permission-validator

a validation framework that checks whether an algorithm is actually allowed to do what it's trying to do with user data- not just "does a permission exist" but "is this specific use of this specific field covered by what the user actually agreed to."

this is designed to run on data controller owned devices, using a multi-agentic system to analyze code both statically and at runtime, then cross-reference everything against each user's real consent records.

this is a component of the framework proposed in [technical framework to ensure data subject's rights in gdpr: a conceptual design](https://doi.org/10.1145/3727166.3727190) (najdi, athauda, bandara, luo - ACSW '25)- specifically addressing the algorithm validation limitation identified in section 4 of the paper.

## licensing

unlike the rest of this repository, this design document is **not** under agpl-3.0. this is view-only- you can read it, but you can't use, reproduce, or build on the ideas without explicit permission from the authors.

## sections

the design document is broken down into these parts:

- [overview](./overview.mdx) - what this is and why it's needed
- [inputs](./inputs.mdx) - what the validation framework expects before it can run
- [approach](./approach.mdx) - the multi-agentic system that powers the validation
- [deployment](./deployment.mdx) - how it runs locally, the cli workflow, and code signing
- [references](./references.mdx) - links and resources that were used or referenced
- [raw inputs](./raw.mdx) - the unedited inputs that were used to put this together, for transparency
