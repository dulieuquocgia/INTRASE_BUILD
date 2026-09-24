# INTRASE iOS build runner

Public GitHub Actions workflow for building INTRASE iOS on macOS/Xcode. The app source and backend are in the private `dulieuquocgia/INTRASE` repository. This repository contains no app source or production credentials.

Releases are dispatched by `deploy/release-testflight.sh` in the private repository. The workflow checks out the exact requested commit with a read-only deploy key, builds a signed IPA, uploads it to Apple and assigns the build to the internal TestFlight group.
