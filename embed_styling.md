# Embed styling syntax

## Format

Modifications are placed after a `|` symbol with spaces between modifications. This is different from [image styling](image_styling.md) because the ID (as in `link#some text`) is used to link to headers in notes.

As an example:

- `![[some file|clean]]`
- `![[some file#some header|no-title clean]]`

## Modifications

| keyword    | description                                  |
| ---------- | -------------------------------------------- |
| `clean`    | Removes the background, padding, and borders |
| `no-title` | Removes the first title                      |
| `no-link`  | Removes the embed link icon                  |
