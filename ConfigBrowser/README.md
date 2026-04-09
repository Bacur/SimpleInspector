# SimpleInspector Configs Browser

## Overview

`ConfigsBrowser` is the module for browsing `ScriptableObject` configs marked with `ProjectConfigAttribute`.
It shows configs in a tree view, supports inline operations, and renders the selected asset in the right inspector panel.

## Contents

- `Runtime`
  `ProjectConfigAttribute` and example config types
- `Editor`
  config index builder, browser window, menu entry, cache models, and editor actions
- `Examples`
  example config assets and sample usage

## Menu

- `SimpleInspector/Configs Browser`

## Usage

Mark a `ScriptableObject` type with `ProjectConfigAttribute`:

```csharp
[ProjectConfig(Category.Core, featureName: "Levels/Premium")]
public class ExampleProjectConfig : ScriptableObject
{
}
```

### Supported `featureName` patterns

- plain text
- nested paths through `/` or `\`
- template values such as `{FieldName}`, `{PropertyName}`, `{Nested.Value}`
- asset-folder token such as `{#ParentFolderName_2}`

## Built-In Actions

- selection inside the browser
- inline rename
- duplicate
- delete
- select asset
- select script
- copy link
- drag and drop of config assets from the tree

## Packaging

Dependencies:

- `SimpleInspector.Core`

## Version

See `Version.txt`.
