# Everforest Enchanted

An Obsidian port of the [Everforest](https://github.com/sainnhe/everforest) theme family. Heavily inspired by [another project of a similar name](https://github.com/0xGlitchbyte/obsidian_everforest) with my custom additions.

I had some issues with the styling of the other project, but the codebase was very different to what the semantics of the official theme area, so I decided to remake the entire thing from scratch.

![](asssets/theme%20screenshots.png)

## Features

- [Everforest](https://github.com/sainnhe/everforest) style color palette
- Light and Dark themes
- Different colors for internal and external links
- [Image styling](image_styling.md) based on ID
  - Alt text as image captions
- Improved and custom callouts
- Code block Language Labels
- Custom CSS classes
  - Customized Dashboard (Inspired by the [Dashboard++ snippet](https://github.com/TfTHacker/DashboardPlusPlus))

### Themes

|             Dark              |             Light              |
|:-----------------------------:|:------------------------------:|
| ![](asssets/theme%20dark.png) | ![](asssets/theme%20light.png) |

### Image styling

|              Dark              |              Light              |
|:------------------------------:|:-------------------------------:|
| ![](asssets/images%20dark.png) | ![](asssets/images%20light.png) |

### Improved and Custom Callouts

|               Dark               |               Light               |
|:--------------------------------:|:---------------------------------:|
| ![](asssets/callouts%20dark.png) | ![](asssets/callouts%20light.png) |

### Code block Language Labels

|                Dark                |                Light                |
|:----------------------------------:|:-----------------------------------:|
| ![](asssets/codeblocks%20dark.png) | ![](asssets/codeblocks%20light.png) |

### CSS Classes

Add them to the YAML frontmatter to activate custom features.

```
---
cssclass: some-class, another-class
---
```

Implemented CSS Classes:

| Class        | Effect                                                                    |
| ------------ | ------------------------------------------------------------------------- |
| `full-width` | Makes the note full width                                                 |
| `wide-width` | Makes the note a bit wider                                                |
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

## Feedback

If you want to add more features, add it as an issue or pull request.
