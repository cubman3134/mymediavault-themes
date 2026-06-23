# My Media Vault — Themes

A community registry of colour themes for **My Media Vault**. Browse and install these from inside the
app: **Settings → Browse Themes…**

## Use it in the app
Paste this repo's raw `index.json` URL into the "Registry" box in **Browse Themes…**:

```
https://raw.githubusercontent.com/<your-user>/mymediavault-themes/main/index.json
```

## Contribute a theme
1. Add your theme JSON under `themes/` (and any background image / icons it references).
2. Add an entry to `index.json`:

   ```json
   {
     "name": "My Theme",
     "author": "you",
     "description": "One line about the look.",
     "file": "themes/MyTheme.json",
     "assets": ["themes/my-bg.png"]
   }
   ```
   - `file`     the theme JSON (downloaded into the app's `themes/` folder).
   - `assets`   any images the theme references (background, icons) — also downloaded into `themes/`.
3. Open a pull request.

### Theme file format
See `themes/Aurora.json` for a full example. Supported keys: `name`, `accentFollowsTab`, `accent`,
`neutralTab`, `tabColors`, `fontFamily`, `fontScale`, `cornerRadius`, `background`, `backgroundDim`,
`icons`, and `detail` (`image`: left/top/hidden, `imageWidth`, `order`).
