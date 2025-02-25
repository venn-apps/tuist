---
slug: '/commands/plugin'
title: Sharing via plugins
description: 'Learn how to use plugin commands for developing and publishing Tuist plugins.'
---

To help developers with the process of [creating plugins](plugins/creating-plugins.md),
we provide a set of commands under `tuist plugin`. These plugin commands are aimed at parts of the plugin defined in `Package.swift`.

### Build

`tuist plugin build` will build the plugin.

#### Arguments

| Argument | Short | Description | Default | Required |
| ------------------ | ----- | ------------------------- | ------- | -------- |
| `--configuration` | `-c`  | Choose configuration | `debug` | No |
| `--path`  | `-p`  | Path to the directory that contains the definition of the plugin | Current directory | No |
| `--build-tests` | n/a | Build both source and test targets | No | No |
| `--show-bin-path` | n/a | Print the binary output path | No | No |
| `--targets` | n/a | Build the specificed targets |  | No |
| `--products` | n/a | Build the specified products | | No |

### Test

`test` subcommand is used for testing the plugin.

#### Arguments

| Argument | Short | Description | Default | Required |
| ------------------ | ----- | ------------------------- | ------- | -------- |
| `--configuration` | `-c`  | Choose configuration | `debug` | No |
| `--path`  | `-p`  | Path to the directory that contains the definition of the plugin | Current directory | No |
| `--build-tests` | n/a | Build both source and test targets | No | No |
| `--test-products` | n/a | Test the specified products | No | No |

### Archive

Archives a plugin into a `NameOfPlugin.tuist-plugin.zip`. This file is then used for publishing the plugin as described [here](plugins/creating-plugins.md).

#### Arguments

| Argument | Short | Description | Default | Required |
| ------------------ | ----- | ------------------------- | ------- | -------- |
| `--path`  | `-p`  | Path to the directory that contains the definition of the plugin | Current directory | No |