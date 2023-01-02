## Blue Hour - Syntax Theme

Blue Hour is a syntax highlight theme for Visual Studio Code. It tries to highlight in mostly analogous, but still distinguishable colors from the blue-green region with a bit of orange for contrast. It was made for people who don't like overly colorful highlights and instead prefer a more uniform and muted color scheme.

![Preview image](https://raw.githubusercontent.com/nptr/blue-hour/master/images/preview.png)

The theme was inspired by the "Absent" theme from the ["rainglow"](https://github.com/rainglow/vscode) collection. In contrast, it is mainly a syntax theme and keeps the editors well-known default dark user interface mostly unchanged.

### Installation

**Automatically:** From the extensions tab within VSCode, search for and install 'Blue Hour Syntax Theme'. Once installed, themes can be switched using the menu item `File -> Preferences -> Color Theme` or via `Ctrl+K Ctrl+T`.

**Manually:** Copy or clone the repository into `~/.vscode/extensions/` and restart the editor.

---

### Advanced Modification

**Bracket Colorization:** VSCode supports different bracket colors based on nesting level. This theme disables that by using one color for all pairs.

* Change or remove the `editorBracketHighlight.foregroundX` key in `~/.vscode/extensions/themes/blue-hour-XXXX.json`

**Status Bar Color:** This theme changes the status bar color, which might not fit everybody.

* Change or remove the `statusBar.XXXX` keys in `~/.vscode/extensions/themes/blue-hour-XXXX.json`

**Editor Inlays:** VSCode can annotate your code with hints for certain languages. The default look is rather ugly with a strong background color. Without the background, distinction between inlay and actual code can be a bit hard. A custom font and/or font size can help here, but must be done in user settings:

* Press Ctrl+Shift+P, type _"user settings"_, select _"Preferences: Open User Settings (JSON)"_. The recommended settings are as follows, but can be changed to your liking.

```json
{
    // advanced inlay modification
    "editor.inlayHints.fontFamily": "Monospace",
    "editor.inlayHints.fontSize": 12,

    // ... other settings
}
```

For a better understanding on what it accomplishes, see the following image:

![Inlay demonstration](https://raw.githubusercontent.com/nptr/blue-hour/master/images/inlays.png)