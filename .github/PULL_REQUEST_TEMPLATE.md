---
name: Pull Request
about: Submit a pull request
# Conventional Commits title. The title drives the release version in repos
# using release-please: feat=minor, fix=patch, chore...=no bump.
title: 'feat(scope): <short description>'
labels: ''
assignees: ''
---

**Description**
Brief description of the change and the issue it addresses.

**Type of Change** (determines the release version where release-please is used)
- [ ] New feature → `feat(...)` → **minor**
- [ ] Bug fix → `fix(...)` → **patch**
- [ ] Breaking change → `feat!` / `BREAKING CHANGE` → **major**
- [ ] Refactor / tooling / docs / CI → `chore`/`refactor`/`docs`/`ci` → **no version bump**

**Testing**
Describe how the change was tested (commands, environment, results).

**Checklist**
- [ ] PR title and commit type are Conventional Commits
- [ ] CI is green (tests, lint, build)
- [ ] No secrets, credentials or real customer data added (use dummy MSISDN)
- [ ] Documentation updated where behaviour changed

**Screenshots / Evidence**
If applicable, add screenshots or command output.