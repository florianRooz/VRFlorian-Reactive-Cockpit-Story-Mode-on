# VRFlorian Reactive Cockpit V2.2.2 — gate recovery update

This small in-place update fixes Story Mode remaining paused when Reactive
Cockpit is restarted while Elite Dangerous is already running.

## What changed

- Any genuinely new gameplay Journal event can confirm that Elite is live.
- A meaningful post-baseline `Status.json` change can also confirm live play.
- The event that opens the gate is delivered after the story runtime starts, so
  triggers such as `StartJump` are not lost.
- The Journal tail is armed before cached world hydration, closing a startup
  race without replaying old telemetry.
- Cached state, timestamp-only status rewrites, main-menu music, and session
  lifecycle records remain blocked.

Mission progress, mission graphs, story media, cockpit assignments, machine
configuration, logs, and user data are preserved.

Validation: 25 automated tests passed, including the captured Mission 2
restart state at the Muni/spycraft fork.

- Package size: 17,959 bytes
- SHA-256: `65C632812B4317845E0ECA09F8C50CB1A7F94BC83DEC3774AC5C19F577EF9DD2`
