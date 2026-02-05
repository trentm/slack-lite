# How to "release" slack-lite

The current setup process is to *copy* the template file from this repo, so there aren't really "releases". However, to try to help a little bit there is a changelog and tags.

0.  Pick a version.

1.  Update:
    - CHANGELOG.md
    - the "Based on" ref in "slack-lite-template.yml"
    and commit.

2.  Tag the repo.

    ```
    VERSION=v1.2.3
    git tag -a "$VERSION" -m "version $VERSION ($(date -u '+%Y-%m-%d'))"
    git push origin "$VERSION"
    ```
