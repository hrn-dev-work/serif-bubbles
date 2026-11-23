# Make speech-bubble images to paste into note articles

[![日本語](https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9E-0969da?style=for-the-badge)](./README.md) [![English](https://img.shields.io/badge/English-0969da?style=for-the-badge)](./README.en.md)

note has no speech-bubble feature. This tool turns a conversation between two speakers into images you can paste into an article. The default names are 「わたし」 and 「メェ助」, and either name can be changed.

Open `index.html` in a browser. There is nothing to install and no account to create.

## Who it is for

People who write on note and want the two voices as images in the article.

## What you can do

- Add one line at a time, reorder lines, and delete lines
- Paste lines that start with 「わたし：」 or 「メェ助：」 and import them together. After a rename, the new names are the line prefixes
- Check the bubbles on screen before saving
- Save one PNG per line, or one PNG of the whole conversation
- Choose a transparent background or a pale green one
- Crop icon images into circles and keep them for the next time you open the page

## What it does not do

- Send the script or the icons to an external server
- Post to note for you
- Keep more than 80 characters in one line (the extra characters are cut off)

## Start here

1. Open `index.html` in a browser
2. Check the two names, then choose icons. The defaults are わたし and メェ助
3. Type the lines, or paste them in bulk
4. Check the preview and save the PNG files

The steps are in [Usage](docs/en/usage.md). Colors, width, and file names are in the [design notes](docs/en/design.md).

## The PNG files

Each image is 800 pixels wide. The dialogue text is 30 pixels.

| Content | Example file name |
| --- | --- |
| First line from the left speaker (default メェ助) | `serif_01_meesuke.png` |
| Second line from the right speaker (default わたし) | `serif_02_watashi.png` |
| Whole conversation | `serif_all.png` |

When the background is transparent, the checkerboard in the preview only marks the transparency. It is not part of the PNG.

## Type and license

Zen Maru Gothic is embedded in the file under the SIL Open Font License 1.1. The full license is at the bottom of the page. If that font cannot be read, the page uses Hiragino Maru Gothic, Yu Gothic, then Meiryo.

Notes for agents (AI) are in English only. See `CONTEXT.md` and `docs/agents/`.
