# App Delivery Acceptance — SPEX installation

Base package generated from [the complete source repository](https://github.com/yangbobo2021/app-delivery-acceptance/tree/c6b27e4d5aeee45ddf0fd9def984bef100683ba6), commit `c6b27e4d5aeee45ddf0fd9def984bef100683ba6`, version **0.4.15**. This development branch adds distribution-only native SPEX fixes, recorded in [DISTRIBUTION-PATCH.json](DISTRIBUTION-PATCH.json). The original `x-source`, `SOURCE.json` and Skill digests remain historical generation records; they do not claim that the patched native files are unchanged upstream exports. The original Skill repository and exported Skill are unchanged.

In SPEX choose a project → 规程 → 从 Git 添加:

| Field | Value |
| --- | --- |
| Package | yangbobo2021/app-delivery-acceptance |
| Git URL | https://github.com/yangbobo2021/app-delivery-acceptance-spex.git |
| Revision | main |
| Folder | Leave empty |

After installation enable acceptance-orchestrate and the child workflows needed for the task, bind distinct Players to roles, and configure your own Agent, model and login. The same installation exports the real app-delivery-acceptance Skill to that project for Codex. Start a new Codex turn in the project and use $app-delivery-acceptance. Its platform setup prepares verified runtime/dependencies in an independent cache; use the returned executable and package paths. No manual file copying or dependency installation inside SPEX-managed exports is required.

Installation does not prove business acceptance. Use the parent workflow for requirement-to-scenario and selected-scene execution, retaining independent review, permissions, leases, immutable inputs and evidence. See the source repository for actual validation scope and prerequisites.


Native SPEX users can enter ordinary text in the selected project:

```text
/acceptance-orchestrate 请按项目书面需求生成场景，正式执行选中的一个场景，独立复审并保存覆盖率、报告和展示视图。
```

The workflow receives the project directory through SPEX's public `cwd` option and creates its own task/request identities. Explicit programmatic JSON delegations remain supported. Required child workflows and distinct Players must be enabled and bound in SPEX.

The [native acceptance record](docs/native-spex-acceptance-20261103.md) documents the selected Mac path, preserved failures and limits. This is a development patch, not a release or an upstream Skill change. Installing the published base again can replace local candidate edits.

Run the focused regressions against an installed native artifact, whose official runtime dependencies are provided by SPEX:

```sh
node tests/native-entry.integration.mjs /absolute/installed/package/playbooks/en/acceptance-orchestrate
node tests/view-progress.integration.mjs /absolute/installed/package/playbooks/en/acceptance-orchestrate
```
