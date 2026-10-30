---
id: team/review-standards
title: Polygon team review standards
lenses: ["team/review-standards"]
categories: ["process"]
enabledByDefault: true
---

# Purpose

Apply the team's review standards to every change under review, in addition to
the language and risk lenses.

# Checks

- Prefer small, focused changes; flag drive-by refactors that obscure the
  behavioural delta.
- Require a test that exercises any new boundary the change introduces.
- Call out error handling that swallows failures or logs secrets.
- Flag public API changes that are not reflected in the changelog.
- Require that configuration defaults stay safe for production.

# False positives

- Do not demand a changelog entry for internal-only refactors.
- Do not flag generated files or vendored dependencies.
