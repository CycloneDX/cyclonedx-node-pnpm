# Integration test: local workspaces

*ATTENTION*: this demo might use known vulnerable dependencies for showcasing purposes.

Install local workspaces and see how they behave.

## remarks

* the dependencies are listed under `devDependencies`.

## output

(i) see [demo snapshots](../../tests/_data/pnpm-ls_demo-results/dev-dependencies).

Output of `pnpm ls --json ...` look like this:

```json5
[
  {
    "name": "demo-dev-dependencies",
    "version": "0.0.0",
    "path": ".../demo/dev-dependencies/project",
    "private": true,
    "devDependencies": {
      "@types/node": {
        "from": "@types/node",
        "version": "18.7.23",
        "resolved": "https://registry.npmjs.org/@types/node/-/node-18.7.23.tgz",
        "description": "TypeScript definitions for Node.js",
        "homepage": "https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/node",
        "repository": "git+https://github.com/DefinitelyTyped/DefinitelyTyped.git"
      }
    }
  }
]
```
