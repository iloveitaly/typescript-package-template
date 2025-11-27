## Package Readme Tags / Badges

```shell
[![Last version](https://img.shields.io/github/tag/USERNAME/REPO.svg?style=flat-square)](https://www.npmjs.org/package/better-node-inspect)
[![NPM Status](https://img.shields.io/npm/dm/REPO.svg?style=flat-square)](https://www.npmjs.org/package/REPO)
![GitHub CI Status](https://github.com/USERNAME/REPO/actions/workflows/build_and_publish.yml/badge.svg)
```

You can copy this template to your clipboard and fill it out using:

```shell
GH_USERNAME=$(gh repo view --json owner --jq '.owner.login' | tr -d '[:space:]')
GH_REPO=$(gh repo view --json name --jq '.name' | tr -d '[:space:]')
TEMPLATE=$(pbpaste)

TEMPLATE=${TEMPLATE//GHUSERNAME/$GH_USERNAME}
echo "${TEMPLATE//GHREPO/$GH_REPO}"
```
