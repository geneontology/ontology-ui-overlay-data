# ontology-ui-overlay-data

## Overview

This repository contains ontology-related data that is not currently held in upstream ontologies (buty maybe should be) needed for some GO UIs. Specifically, some edge glyphs, colors, and labels. These are kept in a YAML file

This is meant to starting to dig ourselves out from some very very old decisions made for AmiGO that ended up getting adopted by early software for Noctua.  E.g. https://github.com/geneontology/noctua/issues/804 and https://github.com/geneontology/noctua/issues/801.

## Workflow

Requires NPM OTPs.

```
git clone https://github.com/geneontology/ontology-ui-overlay-data
cd ~/local/src/git/ontology-ui-overlay-data
docker run -v `pwd`:'/work' -w /work -i -t ubuntu:jammy /bin/bash
apt-get update && apt-get -u install npm nodejs
npm login
[make modifications]
npm publish
```

## Troubleshooting

TBD: how to sync or not sync from AmiGO `amigo2-instance-data`. Let's just see if this works first...
