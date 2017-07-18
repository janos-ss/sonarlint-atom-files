# SonarLint for Atom files

Binaries required by SonarLint for Atom.

This is a throw-away repository until we find a better way to bundle the binaries.

## Clone

Clone without the tags, to avoid downloading the binaries in tagged commits:

    git clone --single-branch https://SonarSource/sonarlint-atom-files

## Update the versions of the embedded files

`master` doesn't have the binaries, so that cloning can stay light and clean.

**Do not commits binaries in `master`.**

1. Create a new branch: `git checkout -b v-SEMVER`
2. Update the URLs in `lib/files.js`
3. Run `npm install` to download the files
4. `git add files`
5. `git commit -m 'Add files'`
6. `git tag SEMVER`
7. `git push --tags`

