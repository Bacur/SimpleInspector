# SimpleInspector Core

## Overview

`Core` is the base module for the SimpleInspector ecosystem.
It contains the shared runtime and editor infrastructure used by the other modules.

## Contents

- `Runtime`
  Base runtime types used by SimpleInspector modules.
- `Editor`
  Shared editor infrastructure:
  custom inspectors, rendering pipeline, reflection helpers, cache IO, state storage, indexing helpers, diagnostics, and UI utilities.
- `Examples`
  Small smoke examples for validating the base inspector pipeline.

## Menu

- `SimpleInspector/About Simple Inspector`

## What It Provides

- fallback custom inspectors for `MonoBehaviour` and `ScriptableObject`
- processor-based inspector rendering pipeline
- reflection helpers for attributes and field paths
- cache and state storage utilities for editor tools
- shared editor utilities used by `Documentation`, `MarkdownViewer`, `ConfigsBrowser`, `FeatureCenter`, and `Group`

## Packaging

Use `Core` as the base package.
Other SimpleInspector modules depend on it.

## Version

See `Version.txt`.
