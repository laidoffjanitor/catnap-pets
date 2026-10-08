# QA evidence

## Saved production checks

The original production reports are in [Plush QA](../pets/plush-catnap/qa/) and [Chonky QA](../pets/chonky-catnap/qa/). They were sanitized for portability, not rerun or rewritten as new approvals.

| Record | Scope |
| --- | --- |
| `atlas-validation.json` | PNG encoding, dimensions, grid, occupied cells, alpha and chroma checks |
| `review.json` | Original extracted animation-frame counts and geometry; intermediate frame files omitted |
| `pet-quality.json` | Jump lift/landing, gaze registration and retained quality warnings |
| `direction-semantics.json` | Visual direction judgments and reviewed warning explanations |
| `direction-blind-combined.json` | Combined votes from three independent direction reviewers |
| `direction-blind-validation.json` | Cardinal and direction consistency checks, including ambiguous diagonals |
| `look-continuity.json` | Gaze registration and adjacent-pose continuity warnings |
| `pets-preflight.json` | Saved Pets service validation response |

Both structural reports and both quality reports contain the approved final PNG SHA-256. Plush's preflight record also includes that hash; Chonky's saved preflight response contains dimensions and byte size but no artifact hash. The repository manifest and fresh packaging hash checks identify the packaged Chonky file without adding a hash claim to the original preflight response.

## Reviewed limitations

Both cats pass the four main cardinal directions. Near-horizontal diagonals can have a small vertical cue. Plush retains explicit direction warnings at 67.5° and 112.5°. Chonky retains warnings at 67.5°, 112.5°, 157.5°, 247.5° and 337.5°; the blind review found the downward component ambiguous in isolation at 112.5° and 247.5°.

Continuity heuristics also flagged silhouette gaps between the ears or feet. The saved visual reviews identify these as exterior background gaps, with additional flood-fill evidence for Plush. Plush's loop boundary has a larger final head-yaw step; Chonky's 135° → 157.5° bounds shift was reviewed as head motion with the body and keyboard anchored. The original warnings are preserved.

## Runtime and packaging

The [browser smoke-test note](runtime-smoke-test.md) records collection rendering, idle motion and selection behavior. It does not claim full live-state or gaze coverage.

The [packaging verification](packaging-verification.json) is a separate, newly executed local check: source-copy identity, exact final hashes, media decoding, v2 grid occupancy, preview frame counts, relative links, portable manifest references and private-metadata scanning. It does not replace the production visual judgments or browser tests.
