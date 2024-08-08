# lune-generate-cdp

Generates Luau definition files from Chrome Devtools Protocol [JSON definitions](https://github.com/ChromeDevTools/devtools-protocol/tree/master/json).

## Installation

You can install `lune-generate-cdp` simply by dragging [build-definitions.luau](/.lune/build-definitions.luau) into your project. From there, you can tweak constants to your liking.

## Usage

`lune-generate-cdp` is a Lune script which means you'll need the [Lune](https://github.com/lune-org/lune) runtime to execute it.

```bash
> lune run build-definitions
```

**Warning:** The formatting of Luau files relies on [stylua](https://github.com/JohnnyMorganz/StyLua) being on the system PATH. You can toggle formatting by tweaking the `SHOULD_FORMAT` constant.

## Support

`lune-generate-cdp` can/cannot:

- ✅ generate definitions for commands
- ✅ generate definitions for events
- ✅ generate general type definitions
- ❌ generate **type** definitions for commands
- ❌ generate **type** definitions for events
