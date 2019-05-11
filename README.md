# `git add thor`

## DISCLAIMER

There's a `.gnupg` folder with the corresponding keyrings inside this project.
The keys in those keyrings are not considered safe, they just exist for
demonstration purposes and should never be used for anything serious.

## How to commit

In this project's root, issue: `export GNUPGHOME="$(PWD)/.gnupg"`
Add the following section to your `~/.gitconfig`

```
[alias]
  sif="commit --allow-empty --author='Sif <sif@asgard.com>' --gpg-sign=7367C9AFDDB049437879507FD15993C126C0F3A1 -v"
  thor="commit --allow-empty --author='Thor <thor@asgard.com>' --gpg-sign=4A7FD581E18B9BAEE35D392A34E1EB42F21C4D1D -v"
  loki="commit --allow-empty --author='Loki <loki@asgard.com>' --gpg-sign=C706845D50E41CBF49CA39A94CAF6CB747E8582C -v"
  odin="commit --allow-empty --author='Odin <odin@asgard.com>' --gpg-sign=A533C6BBB589A6357FE2AC03D8FDA063C656ABF0 -v"
  frey="commit --allow-empty --author='Frey <frey@asgard.com>' --gpg-sign=A533C6BBB589A6357FE2AC03D8FDA063C656ABF0 -v"
  eitri="commit --allow-empty --author='Eitri <eitri@svartalfheim.com>' --gpg-sign=167299A679CBA598D8B8E0286548E07F7B2C783C -v"
  brokk="commit --allow-empty --author='Brokk <brokk@svartalfheim.com>' --gpg-sign=E9AD679F274A592ECBC4A46F00CB15E36DB07365 -v"
  ivaldi="commit --allow-empty --author='Songs of Ivaldi <sons.of.ivaldi@svartalfheim.com>' --gpg-sign=856E856B9508BDFE5AFC09438322E3B84A3B9B64 -v"
```

You should be able to create a signed commit in Thor's name with the command:
`git thor`
