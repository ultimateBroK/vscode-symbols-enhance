<div align="center">

<img src="https://raw.githubusercontent.com/ultimateBroK/vscode-symbols-enhance/main/symbols.png" width="140" />

# Symbols Enhance

A file icon theme for VS Code with folder open/closed states and no explorer arrows
(fork from [Symbols](https://github.com/miguelsolorio/vscode-symbols))

![Folder States Preview](/preview.png)

</div>

## Contributing

If you'd like to contribute to this extension, please take a look at the issues or create a new one. If you'd like to create a new icon, please reference the [Symbols - File Icon Figma file](https://www.figma.com/file/HYLMyRbIdSbIJQlqnd9pSN/Symbols---File-Icons?node-id=20521%3A84115&t=PyBzZOlVG5TXyEdx-1), you can make a copy or reference the styles used (tailwind). Please try to limit your colors to the ones used in existing icons before choosing a different color style.

When submitting a PR, please ensure you've tested the extension locally and ensure that your new icons appear correctly in the file tree view with your new file extension. Include a screenshot of your proposed icon in your PR.

## Generating Icon Previews

Before submitting a PR, please run the preview generation script to update the icon previews:

```bash
npm run generate-previews
```

This script will update the preview markdown files with your new icons. Make sure to commit these changes along with your PR.

## Configuration

You can configure the extension using the following settings:

### Hide Explorer Arrows

```json
"symbols-enhance.hidesExplorerArrows": true
```

Set to `true` to hide arrow icons in the explorer section.

### Default Associations

```json
"symbols-enhance.defaultAssociations": true
```

Allows you to use the default icons for files and folders or disable them and specify your own via the associations settings below.

### Folders

```json
"symbols-enhance.folders.associations": {
    "{folder name}": "{icon name}"
}
```

And here is an example using this setting:

```json
"symbols-enhance.folders.associations": {
    "entities": "folder-assets",
    "infra": "folder-app",
    "schemas": "folder-purple"
}
```

### Files

```json
"symbols-enhance.files.associations": {
    "{file name}": "{icon name}"
}
```

And here is an example:

```json
"symbols-enhance.files.associations": {
    "app.module.ts": "nest",
    "*.service.ts": "nest"
}
```

_Note: For file names, you can use `*` to match all files with a specific file extension._

## Icon Preview

You can preview the icons by reading the the [preview.md](./preview/preview.md) file.

## React Symbols
[Pablo Hdez](https://github.com/pheralb) has graciously created [React-Symbols](https://react-symbols.vercel.app) ([pheralb/react-symbols](https://github.com/pheralb/react-symbols)) to allow you to embed Symbol icons for your React projects.

<img src="https://raw.githubusercontent.com/pheralb/react-symbols/main/website/public/images/og.png">

## Zed Editor

If you're using the [Zed](https://zed.dev) editor, You can take a look at its maintenance here. [Symbols For Zed](https://github.com/sebastiandotdev/zed-symbols)
