# SimpleInspector Group

## Overview

`Group` is the module for grouping inspector fields under shared headers and foldouts.
It extends the SimpleInspector rendering pipeline with grouped field layout.

## Contents

- `Runtime`
  `GroupAttribute`
- `Editor`
  group processor, bootstrap registration, and group GUI rendering
- `Examples`
  sample grouped `MonoBehaviour` and `ScriptableObject` types

## Usage

Annotate consecutive fields with the same group header:

```csharp
[Group("Gameplay")]
public int ScoreLimit;

[Group("Gameplay", foldout: true, defaultExpanded: false)]
public float RespawnDelay;
```

Fields with the same group header are rendered inside one visual block.

## Packaging

Dependencies:

- `SimpleInspector.Core`

## Version

See `Version.txt`.
