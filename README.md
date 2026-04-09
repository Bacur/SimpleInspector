# SimpleInspector

## Overview

`SimpleInspector` is a modular Unity editor toolkit for inspector workflows, project documentation, markdown browsing, feature discovery, and config management.

It is organized as separate modules that can be used together or packaged independently with `Core` as the base dependency.

## Modules

- `Core`
  Shared runtime and editor infrastructure for the whole plugin.
- `Documentation`
  Browsing and indexing documented project types through `DocumentationAttribute`.
- `FeatureCenter`
  Feature discovery, grouping, and validation tools.
- `Group`
  Grouped inspector layout and foldout rendering through `GroupAttribute`.
- `MarkdownViewer`
  Markdown indexing and viewing inside Unity.
- `ConfigsBrowser`
  Tree-based browser for `ScriptableObject` configs marked with `ProjectConfigAttribute`.

## Main Menu

- `SimpleInspector/Documentation`
- `SimpleInspector/Markdown Viewer`
- `SimpleInspector/Configs Browser`
- `SimpleInspector/Feature Center`
- `SimpleInspector/Refresh All`
- `SimpleInspector/Feature Center Validate All`
- `SimpleInspector/About Simple Inspector`

## Packaging

The plugin supports separate `unitypackage` export per module.

Base dependency:

- `SimpleInspector.Core`

Optional modules:

- `SimpleInspector.Documentation`
- `SimpleInspector.FeatureCenter`
- `SimpleInspector.Group`
- `SimpleInspector.MarkdownViewer`
- `SimpleInspector.ConfigsBrowser`

## Author

Stepan Selyuchenko

## GitHub

https://github.com/Bacur/SimpleInspector
