# Adoption record

`kanon-e2e/e2e-deploy-rehearsal-42205052362-1` adopts Kanon. This is its adoption record (`K-LAYOUT-10`), started by `kanon init` on 2026-11-06. A section or choice it leaves out means its documented default.

## People

| Role | Who |
|---|---|
| Owner | `@kanon-e2e` |
| Maintainer | `@kanon-e2e` |
| Stakeholder | `@kanon-e2e` |

## Plan

`kanon-e2e/e2e-deploy-rehearsal-42205052362-1` is a **public repository on an organisation** (`K-ADOPT-2`). Of the platform features of `K-ADOPT-3`:

- **Rulesets:** available.
- **Merge queue:** available.
- **Environments:** the deploy lane deploys to the ones ## Deploy declares, each a GitHub environment.

## Bootstrap

`in bootstrap since 2026-11-06`

## Choices

- **Feature:** `review`
- **Review trigger:** `labelled`
- **Chat channel:** none yet

## Data

Whether this repository holds private or sensitive material, as declared at install. The lanes read the files and diffs their work needs either way.

- **Private or sensitive material:** `no`

## Deploy

The deploy lane's environments, in deploy order: each deploys only after the one before it succeeded on the same release, and the last is production. `kanon init` writes the deploy caller from this list; the reference deploy is the first environment's (`K-PROJ-11`).

- **Environments:** `staging`, `production`
- **Reference environment:** `staging`
- **Reference deploy workflow:** `deploy.yml`
- **Reference deploy job:** `staging / deploy`
