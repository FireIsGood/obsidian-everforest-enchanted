# Everforest Enchanted

![Static Badge](https://img.shields.io/badge/Downloads-3776-7c3aed?style=plastic&logo=obsidian)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/FireIsGood/obsidian-everforest-enchanted/main?style=plastic)

An Obsidian port of the [Everforest](https://github.com/sainnhe/everforest) theme family. Heavily inspired by [another project of a similar name](https://github.com/0xGlitchbyte/obsidian_everforest) with my custom additions.

I had some issues with the styling of the other project, but the codebase was very different to what the semantics of the official theme area, so I decided to remake the entire thing from scratch.

You can get extra customization through the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin.

![](asssets/theme%20screenshots.png)

## Features

- [Everforest](https://github.com/sainnhe/everforest) style color palette
- Light and Dark themes (Hard and Soft respectively)
- Different colors for internal and external links
- [Image styling](image_styling.md) based on ID
  - Alt text as image captions
  - Image grids for multiple images placed inline
- [Embed styling](embed_styling.md) based on alt text
- Improved and custom callouts
- Code block Language Labels
- [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) for extra features
  - [Custom background images](custom_background_image.md) with support for external and local images
  - [Custom stacked panes](custom_stacked_panes.md) based on count rather than pixels
- Custom CSS classes
  - Customized Dashboard *(Inspired by the [Dashboard++ snippet](https://github.com/TfTHacker/DashboardPlusPlus))*

### Themes

|                 Dark                  |                 Light                  |
| :-----------------------------------: | :------------------------------------: |
|     ![](asssets/theme%20dark.png)     |     ![](asssets/theme%20light.png)     |
| ![](asssets/theme%20dark%20image.png) | ![](asssets/theme%20light%20image.png) |

### Image styling

A full list of styles can be found at [image styling](image_styling.md).

|              Dark              |              Light              |
| :----------------------------: | :-----------------------------: |
| ![](asssets/images%20dark.png) | ![](asssets/images%20light.png) |

### Embed Styling

A full list of styles can be found at [embed styling](embed_styling.md).

|              Dark              |              Light              |
| :----------------------------: | :-----------------------------: |
| ![](asssets/embeds%20dark.png) | ![](asssets/embeds%20light.png) |

### Improved and Custom Callouts

|               Dark               |               Light               |
| :------------------------------: | :-------------------------------: |
| ![](asssets/callouts%20dark.png) | ![](asssets/callouts%20light.png) |

### Code block Language Labels

|                Dark                |                Light                |
| :--------------------------------: | :---------------------------------: |
| ![](asssets/codeblocks%20dark.png) | ![](asssets/codeblocks%20light.png) |

## Custom Background Images

External and local images can be used. More information can be found at [custom background images](custom_background_image.md).

The opacity has been lowered to 50% for these examples, by default it is 85%. To get these images in your own vault, see the link above for the image urls.

> ![](asssets/theme%20dark%20image.png)
> Photo by Pixabay from Pexels: <https://www.pexels.com/photo/green-tree-268533/>
<!-- markdownlint-disable-next-line no-blanks-blockquote -->

> ![](asssets/theme%20light%20image.png)
> Photo by Alissa Nabiullina: <https://www.pexels.com/photo/selective-focus-photography-of-white-petaled-flower-plant-997567/>

### CSS Classes

Add them to the YAML frontmatter to activate custom features.

<!-- markdownlint-disable-next-line fenced-code-language -->
```
---
cssclass: some-class, another-class
---
```

Implemented CSS Classes:

| Class        | Effect                                                                    |
| ------------ | ------------------------------------------------------------------------- |
| `full-width` | Makes the note full width                                                 |
| `wide-width` | Makes the note a bit wider (Customizable in Style Settings)               |
| `columns`    | Converts ordered lists into columns                                       |
| `dashboard`  | Converts the page into a dashboard, turning level 1 list items into cards |

## Installation

### Obsidian Marketplace (Recommended)

1. Open `Settings -> Appearance` in your vault
2. Click `Manage` next to the themes dropdown
3. Filter to `Everforest Enchanted`
4. Click `Install and use`

### Manual Download

1. Download this repo
2. Move `theme.css` file into your `/.obsidian/themes/` folder
3. Rename the file to `Everforest Enchanted.css` so it has a unique name
4. Open `Settings -> Appearance` in your vault
5. Select the theme under the Themes dropdown

## Contributing

If you find a bug or have a feature you want added, feel free to add it as an issue or pull request.
