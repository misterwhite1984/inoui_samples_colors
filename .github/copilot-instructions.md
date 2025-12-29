# Copilot Instructions for inoui_samples_colors

## Project Overview
This is a VS Code color theme extension specifically designed for Kontakt Script Processor (KSP) syntax highlighting. The theme is based on VS Code's Dark (Visual Studio) theme, with customized colors for KSP-specific token scopes to improve readability and efficiency in KSP coding.

## Key Files
- `package.json`: Extension manifest defining the theme contribution.
- `themes/inoui-color-theme.json`: The color theme definition file containing UI colors and token color mappings.

## Architecture
- No code; purely a JSON-based theme extension.
- Contributes a single dark theme named "inoui".
- Token colors are defined for standard scopes plus KSP-specific scopes (e.g., `comment.block.ksp`, `keyword.control.ksp`).

## Development Workflow
- Edit `themes/inoui-color-theme.json` directly for color changes.
- Press F5 in VS Code to launch Extension Development Host and test the theme.
- Changes to the theme file are automatically applied in the host window.
- Use `Developer: Inspect Editor Tokens and Scopes` (Ctrl+Shift+P) to examine token scopes in open files.

## KSP-Specific Patterns
- KSP token scopes end with `.ksp` (e.g., `string.quoted.double.ksp`).
- Custom colors for KSP elements:
  - Comments: #969896
  - Strings: #b9f7de
  - Variables: #de9c5f
  - Types: #5e74c1
  - Sections: #424e70
  - Control keywords: #73f0be
  - Operators: #5e74c1
  - Commands: #73f0be
- Ensure new KSP scopes follow this naming convention and use colors from the existing palette.

## Packaging and Publishing
- Use `vsce package` to create a .vsix file for distribution.
- Exclude files listed in `.vscodeignore` (e.g., `.vscode/`, `vsc-extension-quickstart.md`).
- Publish via VS Code Marketplace; the extension is hosted at https://marketplace.visualstudio.com/items?itemName=nmalleus-inouisamples.kspsyntax (companion syntax extension).

## Conventions
- Theme name in package.json: "inoui"
- Base theme: "vs-dark"
- Icon: `resources/Dark_inoui Square.png`
- Repository: https://github.com/nmalleus/inoui_samples_colors</content>
<parameter name="filePath">c:\Users\dusti\Documents\GitHub\inoui_samples_colors\.github\copilot-instructions.md