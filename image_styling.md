# Image styling syntax

## Quick Note about Inline Images

Inline images are broken by default due to how all images are centered. As a result, putting images with text will be displayed on their own line.

To fix this, you need to set the alt text to `inline`:

```md
![[example-image.png|inline|24]] and some text
```

Note that you cannot have any other alt text or spaces.

## Format and Captions

Modifications are placed after a `#` symbol followed by a space after the link. Remote images can also be modified, but follow a slightly different syntax and are a bit bugged in the current release.

Captions are placed after a `|` symbol. They cannot be used on remote images.

Local:

- `![[image.png# 1/2 left shadow|This is a caption.]]`
- `![[image.png# right|This is also a caption.|300]]` (300px using [default sizing](https://help.obsidian.md/How+to/Embed+files#Resize+images))

Remote:

- `![1/2 left shadow](https://example.com/image.png)`
- `![|400](https://example.com/image.png)` (400px using [default sizing](https://help.obsidian.md/How+to/Embed+files#Resize+images))

## Size

Specific custom sizes are supported.

These are provided in addition to the [default sizing](https://help.obsidian.md/How+to/Embed+files#Resize+images) and do not interfere.

| keyword         | description            |
| --------------- | ---------------------- |
| `1/4`           | Fit 25% of the screen  |
| `2/5`           | Fit 22% of the screen  |
| `1/3`           | Fit 33% of the screen  |
| `1/2`           | Fit 50% of the screen  |
| `3/5`           | Fit 60% of the screen  |
| `2/3`           | Fit 66% of the screen  |
| `3/4`           | Fit 75% of the screen  |
| `4/5`           | Fit 80% of the screen  |
| `1/1` or `full` | Fit 100% of the screen |

## Alignment

Left and Right are supported. Center is implied.

Not sure what you expect for the descriptions...

| keyword | description  |
| ------- | ------------ |
| `left`  | Aligns left  |
| `right` | Aligns right |

## Floating

Images can be floated over all other content. This is limited to Reading Mode due to issues with Live Preview.

Simply add `float` with the direction to have the images float.

| keyword       | description  |
| ------------- | ------------ |
| `float left`  | Floats left  |
| `float right` | Floats right |

## Fun

Various extra styles are included

| keyword  | description                              |
| -------- | ---------------------------------------- |
| `white`  | Adds a white background                  |
| `black`  | Adds a black background                  |
| `border` | Adds a border the same color as tables   |
| `shadow` | Adds a drop shadow                       |
| `blur`   | Adds a 5px blur that disappears on hover |
