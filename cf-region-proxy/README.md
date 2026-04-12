# cf-region-proxy

a cloudflare workers-based regional proxy that routes requests through specific edge regions, monitors latency across all regions, and retries through alternative regions on failure.

born out of thinking about how cloudflare ai gateway handles retry logic at the region level- and realizing there's no native way to do programmable per-request region routing on cloudflare.

## sections

the design document is broken down into these parts:

- [why i thought of this idea](./why.mdx) - the origin story behind this, what made me think about it
- [the problem](./problem.mdx) - the actual problem, backed with some context
- [solution & requirements](./solution.mdx) - what the solution looks like and the exact requirements
- [technical design](./technical-design.mdx) - the architecture, how the system actually works under the hood
- [references](./references.mdx) - links and resources that were used or referenced
- [raw inputs](./raw.mdx) - the unedited inputs that were used to put this together, for transparency
