Releasing
========

Prerequisites
check `git remote -v` that `OpenAttribution/oa-android-sdk` is there. If you do not see it, add it:
`git remote add upstream https://github.com/OpenAttribution/oa-android-sdk.git`
    
1. Make sure `CHANGELOG.md` is up-to-date on `main` for the impeding release. Info under `X.Y.Z` will be used on the GitHub release page.
2. Update `libs.versions.toml` to use `X.Y.X`
3. Create pull request from your repo to OpenAttribution
4. Make a new tag: `git tag 0.0.6`
5. Push tag `git push upstream v0.0.6` (this triggers the publish to Maven Central)