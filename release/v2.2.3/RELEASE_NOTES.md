# VRFlorian Reactive Cockpit V2.2.3 — launcher feedback and Mission II clarity

This small in-place update makes the launcher feel immediately responsive and
adds Florian's latest Mission II guidance refinements.

## What changed

- The launcher window appears before its initial Python, EDHM and Shipyard scan.
- Slower operations display a full-window **WORKING** indicator with the current
  task, an indeterminate progress bar and wait cursor.
- The working layer blocks repeat clicks and always clears after success or
  failure.
- Unnecessary system rescans when the launcher regains focus are reduced.
- Mission II includes clearer Bardin's Vice and Dewan spycraft objectives,
  matching Story Reader clues, Muni naming corrections and final audio polish.

Mission progress, story media, cockpit assignments, configuration, machine
paths, logs and user data are preserved. Existing Mission II progress remains
compatible because every graph node and edge identifier is unchanged.

Validation: 25 automated tests passed. The launcher behaviour was tested and
approved on Florian's Windows player installation before publication.

- Package size: 42,092 bytes
- SHA-256: `713E7BBC2C885683D61D07ABFB03808DB6AFEE28CC91BCBB7C4A4B51025D282A`
