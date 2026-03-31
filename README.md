# Xcode Inspired Dark Theme

A Visual Studio Code theme that recreates the dark Xcode coding experience, including the familiar blue focus states, soft gutter contrast, and vibrant syntax hues.

## Prerequisites
- [Node.js](https://nodejs.org/) 18+
- [vsce](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) (`npm install -g vsce`)

## Local Development
1. Install dependencies: `npm install`
2. Launch VS Code and press `F5` to open a new Extension Development Host window.
3. In the new window, switch to the **Xcode Inspired Dark** theme from the Command Palette (`Ctrl/Cmd+K Ctrl/Cmd+T`).

## Packaging & Publishing
- `npm run package` creates a `.vsix` file under the project root.
- `npm run publish` uploads the package (requires `vsce login` and a real `publisher` name in `package.json`).

## Customizing the Palette
1. Map any tweaks in `docs/palette.md` so the design language stays consistent.
2. Update `themes/xcode-inspired-dark-color-theme.json` to mirror the new hex values across both `"colors"` and `"tokenColors"`.
3. Reload the Extension Development Host (`Developer: Reload Window`) after saving to see the adjustments instantly.

## Testing Checklist
- Run `npm install` once so `vsce` is available for packaging.
- Launch the Extension Development Host with `F5` and enable **Xcode Inspired Dark** via `Ctrl/Cmd+K Ctrl/Cmd+T`.
- Inspect editors, terminals, peek views, SCM diff, and markdown previews to confirm contrast ratios.
- Validate syntax coverage by opening a mix of languages (JS/TS, Swift, Markdown, JSON) and adjusting `tokenColors` gaps as needed.

See `docs/palette.md` for the reference color palette before tweaking token colors.
