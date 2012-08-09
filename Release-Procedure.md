---
title: Release Procedure
layout: default
---


## To make a new release:
vX.Y.P denotes the previous version, vX.Y.Z denotes the new version.

1. Ensure the branch builds
2. Update src/version.sh
3. Commit src/version.sh
4. `git tag vX.Y.Z`
5. `git push --tags`
6. `git archive vX.Y.Z --prefix inspircd/ | bzip2 > InspIRCd-X.Y.Z.tar.bz2`
7. Upload the tarball to [GitHub](https://github.com/inspircd/inspircd)
8. Generate a changelog for the [website](https://github.com/inspircd/inspircd.github.com) using `git shortlog --no-merges --pretty=short vX.Y.P..vX.Y.Z`
9. Create a new post on the [website](https://github.com/inspircd/inspircd.github.com) using `rake post`
10. Commit the new post
11. Update topic in [#InspIRCd](irc://irc.chatspike.net/inspircd)
