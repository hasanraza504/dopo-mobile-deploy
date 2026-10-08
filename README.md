# dopo-mobile build workflows

Public build harness only. Private source: `InstaFarms/dopo-mobile`.

The koha-dev staging coordinator pins the source commit, runs CI, then dispatches Linux Android and macOS iOS builds. Signing credentials and a read-only source deploy key are encrypted GitHub secrets. Signed binaries and checksums are uploaded to private storage; no application source or binaries are committed here. Store submissions run on koha-dev.

Web deployment runs separately on koha-dev from the same checked commit.
