# zed-fish

Fish language support in Zed. Includes syntax highlighting and [fish-lsp](https://github.com/ndonfris/fish-lsp) integration.

Prioritize using `fish-lsp` from PATH.

## fish-lsp Configuration

You can configure `fish-lsp` in zed's `settings.json`. Example:

```jsonc
{
    "lsp": {
        "fish-lsp": {
            "initialization_options": {
                "fish_lsp_diagnostic_disable_error_codes": [1004, 2002]
            }
        }
    }
}
```

For options, please refer to [fish-lsp#environment-variables](https://github.com/ndonfris/fish-lsp?tab=readme-ov-file#environment-variables)

If you want to disable `fish-lsp`:

```jsonc
{
    "languages": {
        "Fish": {
            "language_servers": []
        }
    }
}

// or

{
    "languages": {
        "Fish": {
            "enable_language_server": false
        }
    }
}
```

## Credits

- [vscode-fish](https://github.com/bmalehorn/vscode-fish)
- [tree-sitter-fish](https://github.com/ram02z/tree-sitter-fish)
- [fish-lsp](https://github.com/ndonfris/fish-lsp)
- forked from [hasit/zed-fish](https://github.com/hasit/zed-fish)
