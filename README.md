---
title: Manifold Finance CircleCI Orb
description: CircleCI Orb 2.1
version: v.0.1.0
---

# Manifold CircleCI Orb

[![CircleCI Build Status](https://circleci.com/gh/manifoldfinance/circleci.svg?style=shield)](https://circleci.com/gh/manifoldfinance/circleci) [![CircleCI Orb Version](https://img.shields.io/badge/endpoint.svg?url=https://badges.circleci.io/orb/manifoldfinance/solidityci)](https://circleci.com/orbs/registry/orb/manifoldfinance/solidityci) [![GitHub License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://raw.githubusercontent.com/manifoldfinance/circleci/master/LICENSE) [![CircleCI Community](https://img.shields.io/badge/community-CircleCI%20Discuss-343434.svg)](https://discuss.circleci.com/c/ecosystem/orbs)


> Solidity CI Orb


### Supported tags and respective `Dockerfile` links

#{range $_, $v := .Versions}

#### #{$v.Version}

`#{range $_, $b := $v.Builds}`

 * `#{$b.Tag}`#{range $_, $t := $b.Base.AdditionalTags}, `#{$t}`#{end} [(#{$b.Base.Base}/Dockerfile)]($URL/#{$b.Base.Base}/Dockerfile)
#{end}#{end}

## API

Note: unlike `realpath(1)`, these functions take no options; **do not** use `--` to escape any arguments

| Function                          | Description
| --------------------------------- | -------------
| <pre>{{ container.Function}} </pre>          | {{ container.Description }}
| <pre>shell $PATH</pre>  | If `PATH` is a symlink, container `cli`
| <pre>mount:Volume</pre> | Mount file system to absolute path that `PATH` refers to, resolving any relative directories (`.`, `..`) in `PATH` and any symlinks in `PATH`'s ancestor directories





A starter template for orb projects. Build, test, and publish orbs automatically on CircleCI with [Orb-Tools](https://circleci.com/orbs/registry/orb/circleci/orb-tools).

Additional READMEs are available in each directory.

**Meta**: This repository is open for contributions! Feel free to open a pull request with your changes. Due to the nature of this repository, it is not built on CircleCI. The Resources and How to Contribute sections relate to an orb created with this template, rather than the template itself.

## Resources

[CircleCI Orb Registry Page](https://circleci.com/orbs/registry/orb/<namespace>/<project-name>) - The official registry page of this orb for all versions, executors, commands, and jobs described.
[CircleCI Orb Docs](https://circleci.com/docs/2.0/orb-intro/#section=configuration) - Docs for using and creating CircleCI Orbs.

### How to Contribute

We welcome [issues](https://github.com/<organization>/<project-name>/issues) to and [pull requests](https://github.com/<organization>/<project-name>/pulls) against this repository!

### How to Publish
* Create and push a branch with your new features.
* When ready to publish a new production version, create a Pull Request from fore _feature branch_ to `master`.
* The title of the pull request must contain a special semver tag: `[semver:<segement>]` where `<segment>` is replaced by one of the following values.

| Increment | Description|
| ----------| -----------|
| major     | Issue a 1.0.0 incremented release|
| minor     | Issue a x.1.0 incremented release|
| patch     | Issue a x.x.1 incremented release|
| skip      | Do not issue a release|

Example: `[semver:major]`

* Squash and merge. Ensure the semver tag is preserved and entered as a part of the commit message.
* On merge, after manual approval, the orb will automatically be published to the Orb Registry.


For further questions/comments about this or other orbs, visit the Orb Category of [CircleCI Discuss](https://discuss.circleci.com/c/orbs).

