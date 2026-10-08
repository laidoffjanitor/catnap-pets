# Source notes

This collection contains the two approved variants, Plush Catnap and Chonky Catnap. The final PNGs and approved designs were copied without re-encoding. The original production workspace and its archive ZIPs remain unchanged outside this repository.

## Editing constraints

The keyboard is inspired by a Keychron full-size board: dark frame, light and dark keys, and teal accents. It is an approximate design, not an exact replica.

**The keyboard faces the cat.** The spacebar sits closest to the belly, and the numpad is on the cat's right, which appears on **screen-left** in a frontal view. Preserve that asymmetry, the attached lap position and the folded ear identity. Generate or edit the leftward walk independently; horizontally mirroring the whole rightward strip would reverse the keyboard.

The retained generation manifests contain historical derivation and mirror-policy suggestions. Those describe the generation setup, not permission to reverse the approved design. The orientation constraint above governs future edits. Prompts also retain the approved keyboard orientation.

`running` means active work at the keyboard. The two directional `running-*` states mean walking. For gaze edits, use the approved design and each cat's [Plush mechanics](pets/plush-catnap/sources/look-mechanics.md) or [Chonky mechanics](pets/chonky-catnap/sources/look-mechanics.md). Preserve head-and-eye motion with the feet, body and keyboard anchored.

## Selected materials

Each `sources/` folder contains:

- Completed row-strip outputs for all nine animated states and both gaze rows.
- The completed cardinal reference strip, approved cardinal anchors, and registered first gaze row used during production.
- Original generation and retry prompts, layout guides, and sanitized `pet_request.json` and `imagegen-jobs.json` records.
- Gaze mechanics notes.

The base-pet output and duplicate canonical reference images were byte-identical to `design.png`; their manifest references now point to that single copy. The cardinal strip is a generation reference, not an extra upload row. Registered strips are intermediate sources, not interchangeable with the final cleaned atlas.

Failed drafts, superseded attempts, intermediate frame directories, duplicate archive ZIPs, pet registration records and account-linked records are excluded. This is a curated asset collection, not a complete executable reconstruction of the production pipeline. The final sprite sheet is the authoritative upload artifact.

## Record preservation

Paths in copied JSON and prompt records are relative to the **repository root**. Original result flags, measurements, warnings and artifact hashes are retained. Private identifier fields were removed. References to omitted intermediate files are null and listed in the record's `_packaging` note; the frame index, state and recorded metrics remain intact.

Each sanitized JSON record includes the SHA-256 hash of its original source record. Historical job notes may say a later review was pending; the saved final QA reports contain that later review. Packaging did not change those historical statements into new passing results.
