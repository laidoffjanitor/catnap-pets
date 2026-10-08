# Browser smoke test — 2026-10-08

Evidence supplied by the separate Firefox test run and recorded here during packaging. The packaging run did not operate the browser or change the active pet.

Observed:

- Plush Catnap and Chonky Catnap both render under their names in the pet collection.
- Both show multiple animated idle poses.
- Selecting Chonky Catnap and then returning to Plush Catnap works.

Not verified:

- Full live task-driven animation states.
- Pointer-driven gaze tracking.

The collection view provided no state controls, and pointer positioning encountered a window-coordinate error. These limits apply to runtime coverage; the encoded states, offline previews and saved Pets preflight had already passed their respective checks.
