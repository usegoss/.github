# Organization GitHub defaults

This public repository holds the GitHub files that apply across the Goss organization's repositories. It is not a template repository and it does not run CI for other repositories.

## Who this is for

- **Goss team members:** change a default here only when the change should apply to every repository. For anything else, work in the repository that owns the surface; those changes cannot be made from here.
- **Everyone else:** this repository is not a support channel and Goss does not accept outside contributions. Email <support@usegoss.com> for product help, read [SUPPORT.md](SUPPORT.md), and use [SECURITY.md](SECURITY.md) for vulnerabilities. Do not open an issue unless a team member asks you to.

## What is inherited

| File | Inherited by other repositories? | Notes |
| --- | --- | --- |
| `SECURITY.md` | Yes | A repository with its own security policy overrides this one |
| `SUPPORT.md` | Yes | A repository with its own support file overrides this one |
| `.github/ISSUE_TEMPLATE/` | Yes, if the repository has no local `.github/ISSUE_TEMPLATE` | A local directory, even one containing only `config.yml`, disables all defaults |
| `.github/PULL_REQUEST_TEMPLATE.md` | Yes | The default template; a local pull request template overrides it |

The following paths are for this repository only and are not inherited:

- `profile/README.md` is the public organization profile.
- `.github/workflows/validate.yml` and `.yamllint.yml` lint the YAML and workflows in this repository.
- `README.md` documents this repository.
