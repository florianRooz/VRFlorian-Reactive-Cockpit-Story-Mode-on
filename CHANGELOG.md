# Changelog

## 2.2.3 — Launcher feedback and Mission II clarity

- Added a full-window launcher working indicator, progress bar and wait cursor
  for slower operations.
- The launcher now appears before its initial Python, EDHM and Shipyard scan.
- Repeat clicks are blocked while work is in progress, with guaranteed cleanup
  after success or failure.
- Reduced unnecessary system rescans when the launcher regains focus.
- Added Florian's latest Bardin's Vice and Dewan spycraft objective guidance,
  matching Story Reader clues, Muni naming corrections and audio polish.
- Mission progress, media, cockpit assignments, configuration, logs and user
  data remain preserved.

## 2.2.2 — Live telemetry gate recovery

- Story Mode can recover after Reactive Cockpit is restarted during an active
  Elite Dangerous session.
- Fresh gameplay Journal events and meaningful post-baseline Status changes can
  release the startup gate.
- Gate-opening telemetry is delivered after runtime startup so its story
  trigger is not lost.
- Cached/menu telemetry remains blocked.
- Mission progress, graphs, story media, cockpit assignments, configuration,
  logs, and user data are preserved.

## 2.2.1 — Open-test polish and updater repair

- Corrected Aiabiko altitude-limited atmosphere music exit behaviour.
- Installed the final Mission 2 objective and audio polish.
- Repaired the PowerShell updater process check for future updates.
- Published a repaired clean installer for new players.

## 2.2.0 — Open test

- Clean first-time-player package with no Commander identity, cockpit
  assignments, machine paths, mission progress or gameplay logs.
- Reactive Cockpit 1.10.0-DISCO-TEST and launcher 0.7-OPEN-TEST.
- Story Mode ON with Living World, Mission 1 and Mission 2 selection.
- Player-facing Story Reader with one current clue, scanner state, operational
  windows and scan progress where relevant.
- Story Platform 0.12.2 live-location gate, preventing cached or menu-time
  location data from starting story audio.
- Florian's final Mission 1 and Mission 2 graphs for this release.
- Player-local story-assets map; old authoring and Story Director 4.0 paths are
  never used by the clean player.
- Launcher update checking and SHA-256-verified in-place installation.
- Ctrl+Shift+D Disco Mode with correct cockpit/story-state restoration.
- Complete Classic Elite cockpit and bundled cockpit-theme library.
