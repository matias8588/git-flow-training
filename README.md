# Git-flow training

A simple repo to test git-flow features: branching, releasing, hotfixes

# Version

v0.0.2

## Acknowledgements

- [git-flow cheatsheet](https://danielkummer.github.io/git-flow-cheatsheet/)

## Installation

- `git flow init` and set the values as default. If you need something custom you can change it. e.g., release prefix

## Features

- Starting a new feature based on develop branch `git flow feature start <FEATURE NAME>`
- Finishing a feature `git flow feature finish <FEATURE NAME`

## Releases

- Starting a new release `git flow release start <RELEASE>`
- After creating a release it's the time to update the `package.json` file with the new version number and commit that change
- Publishing a release `git flow release publish` and create the PR so the other collaborators can check or even push their hotfix to that branch
- Create a tag `git tag x.x.x` and push them `git push origin --tags`
- Finish the release `git flow release finish <RELEASE>`
- Now that you're in develop branch do a `git push` and then checkout to main and do the same
