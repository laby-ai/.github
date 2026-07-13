# LabY project directory

StoneAI source is managed as four engineering repositories plus two public
product repositories. The organization `.github` repository contains shared
policy and templates and is not a product repository.

## Engineering repositories

| Repository | Visibility | Owner boundary | Gitee reference |
| --- | --- | --- | --- |
| [stoneai-admin-web](https://github.com/laby-ai/stoneai-admin-web) | Private | Account administration frontend | `zhiqi-admin-vue3` |
| [stoneai-studio-web](https://github.com/laby-ai/stoneai-studio-web) | Private | Official site and shared Studio web shell | `zhiqi-studio-web` |
| [stoneai-ai-python](https://github.com/laby-ai/stoneai-ai-python) | Private | Python AI services and integration tools | `zhiqi-ai-python` |
| [stoneai-admin-backend](https://github.com/laby-ai/stoneai-admin-backend) | Private | Account, authorization and billing backend | `zhiqi-admin-backend` |

## Product repositories

| Repository | Visibility | Product boundary |
| --- | --- | --- |
| [knowtrail](https://github.com/laby-ai/knowtrail) | Public | Lingbi research workspace and grounded products |
| [sceneweave](https://github.com/laby-ai/sceneweave) | Public | Huiying film, canvas, media and generation workflow |

## Reference and migration rules

- The four Gitee repositories are read-only references. Source without an
  explicit compatible license is never copied.
- Alignment means adopting request, auth, API, health, logging, metrics, task,
  CI, release and rollback contracts in StoneAI-owned code.
- A language in a reference repository does not justify an empty rewrite. The
  admin backend remains Python until a separately tested migration proves value.
- `stoneai-official` and `account-entitlement` are temporary migration-source
  repositories. They may be retired only after production remotes, CI, release
  source commits and rollback evidence point to the split repositories.
- Every source fix uses a branch, Conventional Commit, pull request, CI and
  merged commit before production promotion.
