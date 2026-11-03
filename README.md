# App Delivery Acceptance — SPEX installation

Generated from [the complete source repository](https://github.com/yangbobo2021/app-delivery-acceptance/tree/525e92f29fe5c625a37669f701897596d04edfd6), commit `525e92f29fe5c625a37669f701897596d04edfd6`. Version **0.4.17**. The source commit, tree and Skill file digests are recorded in `meta.yaml` under `x-source`. Development, specs and regression tests remain in the source repository.

Install a published release from the SPEX app: open your project → Packages → Add… → Registry, search for `yangbobo2021/app-delivery-acceptance`, choose the release, and Add. Public releases need no registry sign-in, GitHub address or manual file copying. Publishing this generated directory is a separate explicit operation.

Git installation remains available as an alternative: choose Packages → Add… → Git.

| Field | Value |
| --- | --- |
| Package | yangbobo2021/app-delivery-acceptance |
| Git URL | https://github.com/yangbobo2021/app-delivery-acceptance-spex.git |
| Revision | main |
| Folder | Leave empty |

After installation enable acceptance-orchestrate and the child workflows needed for the task, bind distinct Players to roles, and configure your own Agent, model and login. The same installation exports the real app-delivery-acceptance Skill to that project for Codex. Start a new Codex turn in the project and use $app-delivery-acceptance. Its platform setup prepares verified runtime/dependencies in an independent cache; use the returned executable and package paths. No manual file copying or dependency installation inside SPEX-managed exports is required.

Installation does not prove business acceptance. Use the parent workflow for requirement-to-scenario and selected-scene execution, retaining independent review, permissions, leases, immutable inputs and evidence. See the source repository for actual validation scope and prerequisites.
