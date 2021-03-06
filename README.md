# semantic-commit-hook
Git hook that enforces semantic commit messages.

## What is it
Semantic versioning automatically assigns version numbers on your code based on your commit messages.
This means that it recognizes hotfixes, refactors, breaking and non-breaking changes.
In my case, it automatically builds and creates a new release on Github based on the work  that has been done.

You can read more about it [here](https://github.com/semantic-release/semantic-release#how-does-it-work).

## How to use
Any commit to your local git repository will be rejected if the first line (the title) does not follow [the semantic versioning format](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#commit-message-format).

For releasing, I use [go-semantic-release](https://github.com/go-semantic-release/semantic-release).

## Installation
```curl --fail -o .git/hooks/commit-msg https://raw.githubusercontent.com/hazcod/semantic-commit-hook/master/commit-msg && chmod 500 .git/hooks/commit-msg```
