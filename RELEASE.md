# Releasing Lektor

This documents how to release Lektor. Various steps in this document may
require privileged access to private systems, so this document is only
targeted at Lektor core members who have the ability to cut a release.

1. Checkout commit you intend to make a release from.

1. Create new branch named after the version you'll release (e.g. 3.1.0)

1. Bump version number in setup.py

1. Create binaries, e.g. dmg for Mac. If problems, fix them in this branch. Make sure to test these binaries manually. Successfully creating a Lektor.dmg file is not a guarantee that the outputed dmg works.

1. Commit any changes needed and push branch.

1. Tag release and push

    ```
    git tag X.Y.Z
    git push --tags
    ```

1. Go to https://github.com/lektor/lektor/releases and release what you’ve tagged, including any binaries made.

1. Upload new version to PyPI.

1. Verify all builds pass https://travis-ci.org/lektor/. In particular after a new release the lektor-website will be redeployed.

1. Pull release branch into master. Close the release branch.
