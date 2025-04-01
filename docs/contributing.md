# Contributing to the Handbook

This handbook is a [living document](https://en.wikipedia.org/wiki/Living_document). It’s likely that some processes will seem foggy, unresponsive or just poorly-documented. Other documentation will fall out of date. When you see something like this, please follow the steps in the [How to Contribute article](./contributing.md) to help us improve.

This is plain language explanation of how to contribute to the handbook. It is meant to reflect the more formal expression of rules laid out in the [National Tech Committee Handbook Content Governance Policy](https://github.com/dsausa/gov-docs/blob/main/handbook-content-governance-policy.md).

Want to make a contribution to the handbook? It's easy! Just follow these simple steps.

On any of the handbook pages, click the "Edit" icon in the top right of the article to jump directly to the GitHub editor for the Markdown document behind the page.

To get there manually:

1. Visit the GitHub repository at https://github.com/dsa-ntc/handbook.tech.dsausa.org
2. In the `docs/` folder, click on the document you want to edit.
3. Click the "edit" button in the top right.
4. Make your edits.
5. When you're done, click "Commit changes" and make a pull request.
6. We'll review your changes!

If you're in NTC, you can request direct write access to this repo.

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


> From the forum
>
> All Handbook pages are Wiki posts to empower NTC members to all contribute
> to actively documenting our practices, policies, projects, and any other
> knowledge that may need to be known. Members are responsible for ensuring
> Project documentation and any relevant Handbook pages for their practice
> area are kept up to date, under the direction of their Project’s Lead and
> Subcommittee liason.
>
> To edit a Handbook page, navigate to the Forum topic and click the :memo:
> Edit button at the bottom of each post. This will open up the Forum’s
> markdown editor screen where you can begin updating a document.
