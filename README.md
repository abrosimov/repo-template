# repo-template

The template new repositories of `abrosimov` are generated from, by
[gh-repo-settings](https://github.com/abrosimov/gh-repo-settings). In a generated repository,
replace this file with the project's own README.

What a generated repository starts with:

- `renovate.json5` — the shared Renovate preset, pinned to a tag; Renovate moves the tag. The
  repository's own rules go below `extends`.
- `.github/workflows/ci.yml` — CI exposing the `required` check the baseline ruleset demands once
  the repository has the topic `ci-gated`. Add the project's jobs and list each in `required`'s
  `needs`.
- `.gitignore` — local state of AI coding agents and other tools, secrets files, OS and IDE files.
  Language-specific entries are added in the repository.
- `LICENSE` — Apache-2.0.

Changes here reach only repositories generated afterwards.
