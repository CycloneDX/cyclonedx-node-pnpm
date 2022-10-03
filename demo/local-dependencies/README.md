# Integration test: local dependencies

*ATTENTION*: this demo might use known vulnerable dependencies for showcasing purposes.

Install local packages/dependencies and see how they behave.

## remarks

* `pnpm6` does not list relative dependencies, but `pnpm7` does

## output

Output of `pnpm ls --json ...` look like this:

```json5
[
  {
    "name": "demo-local-deps",
    "version": "0.0.0",
    "path": ".../demo/local-dependencies/project",
    "private": true,
    "dependencies": {
      "my-local-a": {
        "from": "my-local-a",
        "version": "0.0.0",
        "description": "demo: my-local-a",
        "homepage": "https://github.com/CycloneDX/cyclonedx-node-npm#readme",
        "repository": "git+https://github.com/CycloneDX/cyclonedx-node-npm.git",
        "dependencies": {
          "my-local-b-off": {
            "from": "my-local-b-off",
            "version": "0.0.0",
            "description": "demo: my-local-b-off - a package with a different name than its dir"
          }
        }
      }
    }
  }
]
```
