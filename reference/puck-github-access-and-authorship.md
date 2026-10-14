# Puck — GitHub access and authorship

*Operational reference for Puck's accountable contributions to Inky Tech repositories. Updated 14 October 2026. This supersedes the old per-repository Review/Express Lane and VillageLink Issue #10 control instructions for Puck. Helen-Claude's separate operating arrangement is not changed.*

## First check: the central publication bus

**Control:** [InkyTech Issue #1](https://github.com/Inky-Tech-Pty-Ltd/InkyTech/issues/1).

**Implementation:** [InkyTech `.github/workflows/puck-publish.yml`](https://github.com/Inky-Tech-Pty-Ltd/InkyTech/blob/main/.github/workflows/puck-publish.yml).

**Attribution:** the Puck-GPT GitHub App publishes substantive contributions under **`puck-gpt[bot]`**, not the ordinary GitHub connector's identity.

**Important retrieval habit:** whenever asked to publish or comment on GitHub as Puck, inspect this document, InkyTech Issue #1, and the current central workflow *before* deciding how to proceed. Do not mistake the former VillageLink-local workflows for the current control bus.

The central bus currently allows targets `VillageLink`, `Cobble`, `information-is-life` and `InkyTech`. **InkyBooks is not yet on the allowlist.** The target must also be installed and authorised for the Puck-GPT App.

Only a command commented on Issue #1 by GitHub user `Joe-Rasmussen` activates publication. The App token is created inside GitHub Actions from the `PUCK_GPT_PRIVATE_KEY` secret in InkyTech; never request the private key in chat.

## Repository content publication (direct)

1. Prepare changes on target repository branch `puck-staging/direct/<short-name>` based on current `main`.
2. Tell Joe the exact target and staging branch.
3. Joe comments on [InkyTech Issue #1](https://github.com/Inky-Tech-Pty-Ltd/InkyTech/issues/1):

   ```text
   /puck-publish <repo> puck-staging/direct/<short-name>
   ```

   For InkyTech itself, the shorter `/puck-publish puck-staging/direct/<short-name>` is also supported.

4. The workflow verifies that staging is based on current `main`, recreates the change as a Puck-GPT-authored commit directly on `main`, removes the staging branch, and comments with its result on Issue #1.

GitHub commits and ordinary PRs remain available as review surfaces when warranted; the old dedicated `puck-staging/pr/*` review lane is **no longer the standard authorship path**. Do not publish Puck's substantive changes directly through the ordinary GitHub connector, bypassing attribution.

## GitHub Discussions (central; demonstrated 14 October 2026)

1. Stage a JSON request in the *destination repository*, on branch `puck-staging/discussion/<short-name>` based on its current `main`, at path `.puck/discussion-request.json`.
2. Current central workflow supports a **top-level comment** request of this exact shape:

   ```json
   {
     "operation": "comment",
     "discussion_number": 8,
     "body": "Markdown comment text"
   }
   ```

3. Joe comments on [InkyTech Issue #1](https://github.com/Inky-Tech-Pty-Ltd/InkyTech/issues/1):

   ```text
   /puck-discussion <repo> puck-staging/discussion/<short-name>
   ```

4. The central workflow validates the request and staging-base relationship, uses GitHub Discussions GraphQL with the Puck-GPT token to publish, reports the new comment URL on Issue #1, and removes the successful staging branch.

This central discussion workflow currently supports **`comment` only**. The older *VillageLink-local* workflow also implemented `create`, `edit-comment`, and `read`, but those operations are **not currently implemented in the central InkyTech workflow**. Do not promise them through the central command without first extending and checking the workflow.

### Demonstrated end-to-end example

On 14 October 2026, Puck retrieved [Cobble Discussion #8](https://github.com/Inky-Tech-Pty-Ltd/Cobble/discussions/8) through Cobble's `read_github_discussion` MCP tool, reading the archived discussion on McKay, not GitHub live. Puck staged a substantive response at:

`Cobble:puck-staging/discussion/reply-to-sankarshan-8`

Joe then invoked:

```text
/puck-discussion Cobble puck-staging/discussion/reply-to-sankarshan-8
```

The central workflow published and reported a `puck-gpt[bot]` comment in Discussion #8. This demonstrates the GitHub authorship and MCP retrieval paths; it does **not** prove graph-assisted retrieval or autonomous memory continuity.

## Safety and scope

- The GitHub connector can inspect repositories and stage proposed work; final Puck-GPT attribution must use the central publication bus.
- Verify the current workflow and allowlist rather than assuming all Inky Tech repositories are covered.
- Require Joe's explicit trigger for publication. Do not claim success until the workflow reports it and, where possible, the result is verified.
- A published Village Link or graph relationship is not necessarily true. Distinguish observations, assertions, and established facts.
- If the central workflow is missing a capability, **stage an enhancement for approval rather than bypassing the publication mechanism**.
