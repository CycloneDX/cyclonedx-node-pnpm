# Integration test: bundled dependencies

*ATTENTION*: this demo might use known vulnerable dependencies for showcasing purposes.

Install [bundled packages](https://docs.npmjs.com/cli/v6/configuring-npm/package-json#bundleddependencies)
and see how they behave.  
They can be caused via deprivation `bundleDependencies` or new `bundledDependencies`.
Values can be `true` to mark all dependencies as bundled,
or a list of `string` that identifies the keys in dependencies-lists.

The package [`bundle-dependencies`](https://www.npmjs.com/package/bundle-dependencies)
ships with bundled version of `yargs`.

## remarks

* shipped/bundled dependencies are not listed at all

## output

(i) see [demo snapshots](../../tests/_data/pnpm-ls_demo-results/bundled-dependencies).

Output of `pnpm ls --json ...` look like this:

```json5
[
  {
    "name": "demo-bundled-deps",
    "version": "0.0.0",
    "path": ".../demo/bundled-dependencies/project",
    "private": true,
    "dependencies": {
      "bundle-dependencies": {
        "from": "bundle-dependencies",
        "version": "1.0.2",
        "resolved": "https://registry.npmjs.org/bundle-dependencies/-/bundle-dependencies-1.0.2.tgz",
        "description": "Generates bundledDependencies package.json value using values of the dependencies property.",
        "homepage": "https://github.com/gajus/bundle-dependencies#readme",
        "repository": "git+https://github.com/gajus/bundle-dependencies.git"
      }
    }
  }
]
```
