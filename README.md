# SonarLint for Atom files

Binaries required by SonarLint for Atom.

This is a throw-away repository until we find a better way to bundle the binaries.

## Update the versions of the embedded files

**Do not commits binaries in `master`.**

`master` doesn't have the binaries.

1. Create a new branch
2. Update the URLs in `lib/files.js`
3. Run `npm install` to download the files
4. `git add files`
5. `git commit -m 'Update X to Version Y'`
6. `git tag SEMVER`
7. `git push --tags`

