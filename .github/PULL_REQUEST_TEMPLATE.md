<!--
Title: Conventional Commits, for example "fix(cli): handle an empty config".
It becomes the squash-merge commit message.
Security fixes don't go in a public pull request: report them through the repository's Security tab.
-->

## What and why

<!-- What changed, and why. Link the issue it fixes, for example "Fixes #12". -->

## How it was tested

<!-- The commands you ran and what they showed, so a reviewer can repeat them. -->

## Checklist

- [ ] Every commit is signed and has a `Signed-off-by:` line (`git commit -S -s`).
- [ ] CI passes.
- [ ] Documentation is updated where behaviour changed.
- [ ] No real host names, addresses, credentials or personal data in the change.
