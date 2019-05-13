# VS Sharper VS Code Extension for C#

An extension to make developing C# projects in VS Code fun and productive.

## Features

### Add a New C# Class or Interface File

Creates a new class or interface file and generates an apropriate name for the namespace of the new file.

\!\[Create C# Class or Interface File\]\(images/feature-create-file.gif\)

Use the File Explorer's context menu to add a class or interface file.

> Tip: See below on how to change the generated namespace's name.

### Embed Current Line or Selection

Embeds the current line or selection in a code control block.

\!\[Create C# Class or Interface File\]\(images/feature-embed-selection.gif\)

Available code blocks:

* Block { ... }
* do { ... } while ();
* for (...) { ... }
* foreach (...) { ... }
* if (...) { ... }
* if (...) { ... } else { ... }
* lock (...) { ... }
* try { ... } catch { ... }
* try { ... } catch { ... } finally { ... }
* try { ... } finally { ... }
* using (...) { ... }
* while (...) { ... }

Keyboard shortcut: `CMD+I E` on macOS or `Ctrl+I E` on Windows and Linux

> Tip: The feature is also available in 'Quick fixes' and the code editor's context menu.

## Requirements

It is recommended to install the VS Code C# extension.

## Extension Settings

VS Sharper generates the name for the namespace of a new file from the project's folder structure. You can place a `vssharper.json` file in the projects root or any subfolder to overwrite the generated namespace name for this folder or any of its subfolders.

For example:

```
{
    "namespace": "MyProject"
}
```
The extension looks up the subfolders' chain for a `vssharper.json` file until it reaches the root of the project.

## Telemetry

This extension collects anonymous usage data like VS Code. You can use VS Code's telemetry setting to turn it off.

## Extension Commands

* Add a New C# Class File (`vsSharper.addCsharpClassFile`)
* Add a New C# Interface File (`vsSharper.addCsharpClassFile`)
* Embed Current Line or Selection (`vsSharper.embedSelection`)
* Embed Current Line or Selection into Code Block (`vsSharper.embedSelection.block`)

## Known Issues

No known isssues.

## Release Notes

### Version 0.0.n

First preview release. More features and productivity tools will be added in the coming weeks and months.

Please use Github to report issues or send any feature requests.

## License

This Github repo is for issues and feature requests.

The project is a private endeavour and the source code is not publicly available.

See: LICENSE.md
