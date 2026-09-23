# Update release policy

This policy applies to every VRFlorian Reactive Cockpit launcher update.

## One-step updates

- The newest update package must be cumulative from the current public clean
  installer, not merely incremental from the immediately preceding update.
- It must contain the latest version of every required product file changed by
  any update since that clean-installer baseline. Superseded version-specific
  notes do not need to be carried forward.
- Any supported older installation must be able to install the newest package
  directly. Players must never need to install intermediate updates.
- When the public clean installer is refreshed, that release becomes the new
  baseline for subsequent cumulative packages.

## Version labels

- Treat the current product release and the clean-installer version as two
  separate values.
- Every release updates the current-version wording on the website and in the
  repository README.
- Never relabel an older clean-installer ZIP as a newer version. Until a new
  full installer is built and verified, explain that the launcher brings the
  clean installer up to the current release.

## Player data

An update must preserve player-owned state, including configuration, cockpit
assignments, mission progress, Living World state, checkpoints, user data and
logs. Release validation must confirm this by comparing protected files before
and after installation.

## Release validation

Before publication:

1. Apply the candidate package to a copy of the current clean installer.
2. Apply the same package to a copy of the immediately preceding public
   version.
3. Run the complete automated test suite and graph/media validation.
4. Verify package size and SHA-256 against the manifest.
5. Upload and independently download-verify the package before switching the
   live manifest.
6. Publish the manifest last so players can never be directed to an incomplete
   or unverified package.

## Release notes and spoilers

- The launcher-facing manifest message is always generic and spoiler-free by
  default: "There is a new update ready for you, making Reactive Cockpit and
  Story Mode even better. Update now?"
- Launcher-facing notes must not name story locations, characters, clues,
  objectives, events or unreleased mechanics.
- Package-internal release notes are maintained separately. Their contents are
  included only after Florian explicitly specifies or approves them for that
  release.
