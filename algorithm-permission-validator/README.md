# algorithm-permission-validator

a validation framework that checks whether an algorithm is actually allowed to do what it's trying to do with user data- not just "does a permission exist" but "is this specific use of this specific field covered by what the user actually agreed to."

this is designed to run on data controller owned devices, using a multi-agentic system to analyze code both statically and at runtime, then cross-reference everything against each user's real consent records.

## sections

the design document is broken down into these parts:

- [overview](./overview.mdx) - what this is and why it's needed
- [inputs](./inputs.mdx) - what the validation framework expects before it can run
- [approach](./approach.mdx) - the multi-agentic system that powers the validation
- [deployment](./deployment.mdx) - how it runs locally, the cli workflow, and code signing
- [raw inputs](./raw.mdx) - the unedited inputs that were used to put this together, for transparency
