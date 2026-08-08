# Contributing

These conventions apply across all Aveno Digital repositories. Individual projects may
add to them in their own `CONTRIBUTING.md`, but should not contradict them.

## Branches

- `main` is protected and always deployable.
- Work happens on short-lived branches: `feat/short-description`,
  `fix/short-description`, `chore/short-description`.
- Rebase onto `main` rather than merging `main` into your branch.

## Commits

Use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(auth): add password reset flow
fix(api): handle empty pagination cursor
chore(deps): bump vitest to 2.1
```

Types in use: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `perf`, `build`, `ci`.

## Pull requests

- One logical change per pull request. If it needs a "and also" in the title, split it.
- Fill out the pull request template — especially how you verified the change.
- CI must be green before review.
- At least one approval before merge. Squash-merge is the default.

## Code review

Reviewers look for correctness first, then clarity, then style. Style disagreements that
a linter could settle belong in the linter config, not in review comments.

## Local setup

Each repository's README documents how to install dependencies and run the project. If
those instructions are wrong or incomplete, fixing them is a valid pull request.
