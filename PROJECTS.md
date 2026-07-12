# LabY project directory

StoneAI is managed as four product repositories. The organization `.github`
repository contains shared policy and templates and is not a fifth product.

## Product repositories

| Domain | Repository | Visibility | Runtime owner |
| --- | --- | --- | --- |
| Website | [stoneai-official](https://github.com/laby-ai/stoneai-official) | Private | Public site and product entry points |
| Account and billing | [account-entitlement](https://github.com/laby-ai/account-entitlement) | Private | Identity, tenant/member, RBAC, billing and audit |
| Lingbi | [knowtrail](https://github.com/laby-ai/knowtrail) | Public | Research workspace and grounded products |
| Huiying | [sceneweave](https://github.com/laby-ai/sceneweave) | Public | Film, canvas, media, provider tasks and composition |

## Gitee engineering references

`zhiqi-admin-vue3`, `zhiqi-studio-web`, `zhiqi-ai-python` and
`zhiqi-admin-backend` are read-only references. LabY adopts their request,
authentication, API, health, logging, metrics, task-isolation, CI and release
contracts inside the four product repositories. Their source is not copied and
no empty repository is created merely to match a language or directory name.

Each product README must link its `docs/engineering-alignment.md`, which records
the product owner boundary, reference mapping, required checks and rollout
contract.

## Repository lifecycle

- New product repositories require a real runtime owner and consumer.
- Experiments remain in a product branch or documented sandbox until promoted.
- Duplicate repositories are retired only after production remotes and source
  commits prove they are unused, and a recoverable bundle is retained.
- Every source fix uses branch, commit, pull request, CI and merged commit
  traceability before release.
