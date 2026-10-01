# Quality and completeness

The release sprite atlas is byte-identical to the installed pixel pet and to the original validated build artifact. Repacking for Petdex changes the ZIP layout only; no animation frames are removed or regenerated.

## Atlas contents

The transparent RGBA WebP atlas is 1536 × 2288 pixels: eight columns and eleven rows of 192 × 208 cells.

| Row, zero-based | State | Populated cells |
| :--- | :--- | ---: |
| 0 | idle | 7 |
| 1 | running-right | 8 |
| 2 | running-left | 8 |
| 3 | waving | 4 |
| 4 | jumping | 5 |
| 5 | failed | 8 |
| 6 | waiting | 6 |
| 7 | running (working) | 6 |
| 8 | review | 6 |
| 9 | look directions 0°–157.5° | 8 |
| 10 | look directions 180°–337.5° | 8 |

Populated cells describe stored artwork, not a promise that every host app plays exactly that many frames. In particular, the inspected Petdex state configuration uses six frames for idle, while this atlas preserves seven populated idle cells. The complete source atlas is retained.

## Verification

- The Petdex ZIP contains `pet.json` and `spritesheet.webp` directly at its root.
- The ZIP passes CRC verification and both files match the prepared source files byte for byte.
- The manifest declares sprite version 2 and uses a relative sprite filename.
- The image and GIF previews contain no EXIF, XMP, ICC profile, or comment metadata in the inspected files.
- The saved final atlas validation reports no errors or warnings, no remaining chroma fringe, and no hidden RGB residue under fully transparent pixels.
- All nine animation GIFs and the sixteen-direction GIF are included as previews.

## Saved build reviews and limitations

The reports in `quality-checks/` are historical evidence from the original build, with local paths and internal reviewer identifiers removed. They are not new reviews performed during publication preparation. Intermediate reports are retained and may show warnings that were assessed later in the build.

Directional review noted that some intermediate diagonal looks are subtle and that a few direction transitions are noticeable. These are preserved as limitations rather than described as perfect smooth motion.

Custom-pet loading behavior depends on the host application. This package does not claim to fix the previously observed initial top-to-bottom appearance of custom pets.

Only the final pixel version is included. Earlier character versions, rejected animation candidates, personal chat history, and local installation logs are not part of the public pet package.
