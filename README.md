# Catnap — custom cats for ChatGPT Pets

Meet **Plush Catnap** and **Chonky Catnap**: two sleepy orange cats with tiny keyboards, made as custom companions for **ChatGPT Pets**. Choose the soft plush cat or the round cartoon cat, download its transparent sprite sheet, and add it through ChatGPT's Pets settings where the v2 format is supported.

Each cat includes nine animated states, sixteen head-and-eye gaze poses, and previews you can watch before downloading. The two upload files are linked below; no coding or build step is needed.

| Plush Catnap | Chonky Catnap |
| --- | --- |
| ![Plush Catnap breathing and blinking](pets/plush-catnap/previews/idle.gif) | ![Chonky Catnap breathing and blinking](pets/chonky-catnap/previews/idle.gif) |
| Soft plush texture, oversized sleepy head. | Round cartoon body, tiny tired head. |
| [Plush upload PNG](pets/plush-catnap/spritesheet.png) · [Watch all states](pets/plush-catnap/previews/all-states.gif) · [Browse Plush files](pets/plush-catnap/README.md) | [Chonky upload PNG](pets/chonky-catnap/spritesheet.png) · [Watch all states](pets/chonky-catnap/previews/all-states.gif) · [Browse Chonky files](pets/chonky-catnap/README.md) |

## Download and add a cat

1. **Get one cat:** open its upload PNG link above and use GitHub's raw download control. **Get both:** on the repository's main page, choose **Code → Download ZIP**, then unzip the download.
2. Open [ChatGPT Pets settings](https://chatgpt.com/settings/pets) while signed in.
3. Choose **Upload pet**, select the matching file below, and name it **Plush Catnap** or **Chonky Catnap**.
4. Save the pet and select it from your collection.

| Cat | File to upload from the downloaded folder |
| --- | --- |
| Plush Catnap | `pets/plush-catnap/spritesheet.png` |
| Chonky Catnap | `pets/chonky-catnap/spritesheet.png` |

Use the full sprite sheet. `design.png`, contact sheets, GIFs and videos are viewing or editing references.

**Compatibility:** these are eleven-row **Pets v2** sheets at **1536 × 2288**. Use an upload interface that supports v2. If your uploader only accepts the nine-row **1536 × 1872** size described in the [official Pets documentation](https://learn.chatgpt.com/docs/pets), keep these originals unchanged rather than resizing them.

## Versioned downloads

**[v1.0.1](https://github.com/laidoffjanitor/catnap-pets/releases/tag/v1.0.1)** contains the current Plush Catnap and Chonky Catnap collection with its CC0 license. The release offers a separate PNG for each cat, upload instructions, the license, and SHA-256 checksums. The ZIP includes both cats, instructions, the license, and checksums. Both PNGs are unchanged from v1.0.0.

Future added keyboard or cat variants can use minor versions such as `1.1.0`; fixes can use patch versions such as `1.0.2`. See the [changelog](CHANGELOG.md) for each release's changes.

## License

The pet artwork and repository content are offered under [CC0 1.0 Universal](LICENSE), to the extent of rights held by the contributors. You may use, modify, and share that material, including commercially, without requiring credit. This does not claim copyright in AI-generated portions or grant rights to third-party names, trademarks, or reference products.

## What's included

```text
pets/
  plush-catnap/
  chonky-catnap/
    spritesheet.png       final upload asset
    design.png            approved character design
    previews/             GIF, WebP, MP4 and four-state stills
    sources/              selected strips, prompts and source manifests
    qa/                   preserved validation reports and visual evidence
manifest.json             final artifact names, sizes and SHA-256 hashes
SHA256SUMS                 checksums for repository content
qa/                       packaging checks and browser smoke-test notes
SOURCES.md                 source selection and editing constraints
```

Both cat folders have the same structure. [Source notes](SOURCES.md) explain the selected materials and keyboard orientation.

<details>
<summary>Sprite format and state layout</summary>


Both upload assets are transparent RGBA PNGs with **8 columns × 11 rows**, **192 × 208 pixels per cell**, and **73 populated poses**. Unused cells remain transparent. Row numbers below start at zero; frames run left to right.

| Row | State name | Frames | Behavior |
| --- | --- | ---: | --- |
| 0 | `idle` | 6 | Sleepy breathing and blinking |
| 1 | `running-right` | 8 | Walk or waddle to the right |
| 2 | `running-left` | 8 | Walk or waddle to the left |
| 3 | `waving` | 4 | Tired paw wave |
| 4 | `jumping` | 5 | Lift and landing |
| 5 | `failed` | 8 | Forehead slump onto the keyboard |
| 6 | `waiting` | 6 | Expectant pause |
| 7 | `running` | 6 | Active work: seated keyboard typing |
| 8 | `review` | 6 | Inspecting completed work |
| 9 | `look-row-9` | 8 | 0°, 22.5°, 45°, 67.5°, 90°, 112.5°, 135°, 157.5° |
| 10 | `look-row-10` | 8 | 180°, 202.5°, 225°, 247.5°, 270°, 292.5°, 315°, 337.5° |

The gaze sequence runs clockwise from **up (0°)** through **screen-right (90°)**, **down (180°)** and **screen-left (270°)**. The head and eyes move while the seated body and keyboard stay anchored.

PNG and the transparent WebP previews preserve soft alpha edges. GIF and MP4 previews are composited against a neutral background for clean viewing; they are not upload masters. Source strips can still have chroma-key backgrounds because they precede extraction and cleanup.

</details>

[Validation notes](qa/README.md) · [Artifact manifest](manifest.json) · [File checksums](SHA256SUMS)

<details>
<summary>Verify downloaded repository files</summary>

From the downloaded repository folder on macOS or Linux:

```sh
shasum -a 256 -c SHA256SUMS
```

</details>
