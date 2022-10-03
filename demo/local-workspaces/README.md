# Integration test: local workspaces

*ATTENTION*: this demo might use known vulnerable dependencies for showcasing purposes.

Install local workspaces and see how they behave.
## remarks

* direct dependencies in workspaces are not listed at all
* neither are transitive workspace dependencies

## output

Output of `pnpm ls --json ...` look like this:

```json5
[
  {
    "name": "demo-workspaces",
    "version": "0.0.0",
    "path": ".../demo/local-workspaces/project",
    "private": true
  }
]
```
