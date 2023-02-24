# How it works

This tool utilizes `pnpm-ls` on the target project and parses its output.

This way the tool does not depend on libraries that are already part of `pnpm`.
All logic and analysis is done by `pnpm` itself, the output is just interpreted and used.
To get all dependencies, the depth is set to `Infinity`.

Sometimes `pnpm-ls` got hiccups - caused by individual broken project installation or bugs with `pnpm`.
Then, this tool may also read `package.json` files inside the `node_module` directory as an additional information source.
