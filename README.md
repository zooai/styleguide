# Zoo Style Guide

The conventions are shared across the estate and live in one place:

**[hanzoai/styleguide](https://github.com/hanzoai/styleguide)** — commits,
naming, comments, architecture, TypeScript, Go, whitespace.

Read those first. They are brand-neutral on purpose and they govern this org
unchanged. Nothing on this page repeats them; a rule written twice becomes two
rules the day one copy is edited.

What follows is only what is different about Zoo.

## Who we are

Zoo Labs Foundation, a 501(c)(3) non-profit building a decentralised network
that opens access to AI: distributed training, open frontier models, Byzantine-
robust agent coordination, and Proof of AI consensus over inference and
training work.

## Names and addresses

| | |
|---|---|
| GitHub org | `zooai` |
| Container registry | `ghcr.io/zooai` |
| Foundation | `zoo.ngo` |
| Chain | `zoo.network` |
| Models | `zenlm.ai` |

Never publish a Zoo image to another org's registry, and never show the Hanzo
or Lux mark on a Zoo surface. Shared infrastructure — identity, keys, gateway,
ingress — carries the brand of the domain it is serving, decided by hostname,
never by which repo the binary was built from.

## Proposals

A change to the network is a **ZIP**, in [`zooai/zips`](https://github.com/zooai/zips),
and it earns community agreement before it earns an implementation. A design
decision that outlives a release belongs in a ZIP, not in a comment and not in
a README.

## Papers

Research goes in [`zooai/papers`](https://github.com/zooai/papers) as LaTeX.
Never Markdown — a paper is typeset, and a format that cannot set an equation
is not a format for this work.

## Licence

`MIT OR Apache-2.0`, per [HIP-0137](https://github.com/hanzoai/hips/blob/main/HIPs/hip-0137-one-license.md).
