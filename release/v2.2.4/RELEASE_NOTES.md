# VRFlorian Reactive Cockpit V2.2.4 — Living World and dialogue playback

This cumulative in-place update expands Living World and hardens Mission II
playback for players who advance through dialogue quickly.

## What changed

- Added Mount Hagrass wind on HIP 87621 2 b b.
- Added the Hagrass stela soundscape for commanders approaching on foot or in
  an SRV.
- Added Mount Darwin on Col 359 Sector PN-Q c6-12 6 c.
- Reused `mountan wind.mp3` and `singer A.mp3` from the existing Story Assets
  folder; no new media payload is required.
- Moved Mission II spoken cues onto the shared `dialogue` layer. A newly
  triggered line now replaces the previous spoken line rather than overlapping
  it when the player advances quickly with CTRL+A.

The package is cumulative. It also carries the V2.2.2 live-telemetry resume
gate and all V2.2.3 launcher feedback, Story Reader and Mission II clarity
changes, ensuring a player can update directly from the V2.2.1 clean installer.

Mission progress, Living World state, story media, cockpit assignments,
configuration, machine paths, logs and user data are preserved. Mission II
node and edge identifiers remain unchanged, and Yggdrasil stays on graph
version 1.0.0 for state compatibility.

- Automated tests: 26 passed
- Package size: 59,759 bytes
- SHA-256: `8FB999B06C9455E005ED254D8729E6F81BDF5B89EE8E3155581C67622647F1ED`
