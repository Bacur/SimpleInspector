# SimpleInspector Documentation

## Overview

`Documentation` is the module for browsing documented project types inside Unity.
It builds an indexed list of classes marked with `DocumentationAttribute` and shows them in a dedicated editor window.

## Contents

- `Runtime`
  `DocumentationAttribute` and related runtime metadata.
- `Editor`
  documentation cache builder, editor window, menu entry, and rendering logic.
- `Examples`
  sample documented assets and types.

## Menu

- `SimpleInspector/Documentation`

## Usage

Annotate a type with `DocumentationAttribute`, for example:

```csharp
[Documentation("My Title", Category.Config, "Short description")]
public class ExampleDocumentedConfig : ScriptableObject
{
}
```

Then open the Documentation window to browse indexed entries.

## Packaging

Dependencies:

- `SimpleInspector.Core`

## Version

See `Version.txt`.
