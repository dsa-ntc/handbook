# Contributing to the Handbook

This is plain language explanation of how to contribute to the handbook. It is meant to reflect the more formal expression of rules laid out in the [National Tech Committee Handbook Content Governance Policy](https://github.com/dsausa/gov-docs/blob/main/handbook-content-governance-policy.md).

Want to make a contribution to the handbook? It's easy! Just follow these simple steps.

1. Fork the handbook to a new branch.
2. Make your changes to that branch.
3. Push your commit to the `dev` repo and initiate a pull request.
4. Publicize your contribution on the NTC Slack and request feedback from your peer contributors.
5. The Handbook Content Governance team will review your contribution. They may ask questions or make suggestions. You should feel free to engage with them and try to get your contribution to a state that will pass their approval process.
6. Once your contribution pass approval it will be merged by the HCG team into the master branch.


## Visualization
```mermaid
graph TD;
change-needed([Changes needed to NTC handbook])
--fork main branch-->make-changes[Amend docs to reflect desired changes]
-->merge-request[Make merge request against dev branch]
-->review[NTC members comment, ask questions, or propose changes <br> Content Governance members review, comment, ask questions, or propose changes]
-->approval{Content Goverance org approves changes?}
--no-->steering[Steering Committee determines approval]
-->|approved|merge
approval--yes-->merge[Content Governance org merges changes into dev branch]
-->check[Check for merge conflicts]
--> final_merge([Merge into main branch])

```