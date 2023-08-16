oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![GitHub license](https://img.shields.io/github/license/oclif/hello-world)](https://github.com/oclif/hello-world/blob/main/LICENSE)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g ombayus-cli
$ ombayus-cli COMMAND
running command...
$ ombayus-cli (--version)
ombayus-cli/0.0.0 darwin-arm64 node-v16.15.1
$ ombayus-cli --help [COMMAND]
USAGE
  $ ombayus-cli COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`ombayus-cli hello PERSON`](#ombayus-cli-hello-person)
* [`ombayus-cli hello world`](#ombayus-cli-hello-world)
* [`ombayus-cli help [COMMANDS]`](#ombayus-cli-help-commands)
* [`ombayus-cli plugins`](#ombayus-cli-plugins)
* [`ombayus-cli plugins:install PLUGIN...`](#ombayus-cli-pluginsinstall-plugin)
* [`ombayus-cli plugins:inspect PLUGIN...`](#ombayus-cli-pluginsinspect-plugin)
* [`ombayus-cli plugins:install PLUGIN...`](#ombayus-cli-pluginsinstall-plugin-1)
* [`ombayus-cli plugins:link PLUGIN`](#ombayus-cli-pluginslink-plugin)
* [`ombayus-cli plugins:uninstall PLUGIN...`](#ombayus-cli-pluginsuninstall-plugin)
* [`ombayus-cli plugins:uninstall PLUGIN...`](#ombayus-cli-pluginsuninstall-plugin-1)
* [`ombayus-cli plugins:uninstall PLUGIN...`](#ombayus-cli-pluginsuninstall-plugin-2)
* [`ombayus-cli plugins update`](#ombayus-cli-plugins-update)

## `ombayus-cli hello PERSON`

Say hello

```
USAGE
  $ ombayus-cli hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/OmBayus/ombayus-cli/blob/v0.0.0/dist/commands/hello/index.ts)_

## `ombayus-cli hello world`

Say hello world

```
USAGE
  $ ombayus-cli hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ ombayus-cli hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [dist/commands/hello/world.ts](https://github.com/OmBayus/ombayus-cli/blob/v0.0.0/dist/commands/hello/world.ts)_

## `ombayus-cli help [COMMANDS]`

Display help for ombayus-cli.

```
USAGE
  $ ombayus-cli help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for ombayus-cli.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.16/src/commands/help.ts)_

## `ombayus-cli plugins`

List installed plugins.

```
USAGE
  $ ombayus-cli plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ ombayus-cli plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.2.5/src/commands/plugins/index.ts)_

## `ombayus-cli plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ ombayus-cli plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ ombayus-cli plugins add

EXAMPLES
  $ ombayus-cli plugins:install myplugin 

  $ ombayus-cli plugins:install https://github.com/someuser/someplugin

  $ ombayus-cli plugins:install someuser/someplugin
```

## `ombayus-cli plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ ombayus-cli plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ ombayus-cli plugins:inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.2.5/src/commands/plugins/inspect.ts)_

## `ombayus-cli plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ ombayus-cli plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ ombayus-cli plugins add

EXAMPLES
  $ ombayus-cli plugins:install myplugin 

  $ ombayus-cli plugins:install https://github.com/someuser/someplugin

  $ ombayus-cli plugins:install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.2.5/src/commands/plugins/install.ts)_

## `ombayus-cli plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ ombayus-cli plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ ombayus-cli plugins:link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.2.5/src/commands/plugins/link.ts)_

## `ombayus-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ ombayus-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ ombayus-cli plugins unlink
  $ ombayus-cli plugins remove
```

## `ombayus-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ ombayus-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ ombayus-cli plugins unlink
  $ ombayus-cli plugins remove
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.2.5/src/commands/plugins/uninstall.ts)_

## `ombayus-cli plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ ombayus-cli plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ ombayus-cli plugins unlink
  $ ombayus-cli plugins remove
```

## `ombayus-cli plugins update`

Update installed plugins.

```
USAGE
  $ ombayus-cli plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v3.2.5/src/commands/plugins/update.ts)_
<!-- commandsstop -->
