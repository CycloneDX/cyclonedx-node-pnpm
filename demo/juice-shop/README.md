# Integration test: OWASP Juice Shop

*ATTENTION*: this demo might use known vulnerable dependencies for showcasing purposes.

The package manifest is based on
<https://github.com/juice-shop/juice-shop/tree/v14.1.1>

## remarks

* dependencies that are transitive might not have all its dependencies,
  because a complete version was printed in a layer above.

## output

(i) see [demo snapshots](../../tests/_data/pnpm-ls_demo-results/juice-shop).

Output of `pnpm ls --json ...` look like this:

```json5
[
  {
    "name": "juice-shop",
    "version": "14.1.1",
    "path": ".../demo/juice-shop/project",
    "private": true,
    "dependencies": {
      // list of more dependencies
      "body-parser": {
        "from": "body-parser",
        "version": "1.20.0",
        "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.20.0.tgz",
        "description": "Node.js body parsing middleware",
        "homepage": "https://github.com/expressjs/body-parser#readme",
        "repository": "git+https://github.com/expressjs/body-parser.git",
        "dependencies": {
          "js-yaml": {
            "from": "js-yaml",
            "version": "3.14.1",
            "resolved": "https://registry.npmjs.org/js-yaml/-/js-yaml-3.14.1.tgz",
            "description": "YAML 1.2 parser and serializer",
            "homepage": "https://github.com/nodeca/js-yaml",
            "repository": "git+https://github.com/nodeca/js-yaml.git"
          },
          // list of more dependencies
        }
      },
      "js-yaml": {
        "from": "js-yaml",
        "version": "3.14.1",
        "resolved": "https://registry.npmjs.org/js-yaml/-/js-yaml-3.14.1.tgz",
        "description": "YAML 1.2 parser and serializer",
        "homepage": "https://github.com/nodeca/js-yaml",
        "repository": "git+https://github.com/nodeca/js-yaml.git",
        "dependencies": {
          "argparse": {
            "from": "argparse",
            "version": "1.0.10",
            "resolved": "https://registry.npmjs.org/argparse/-/argparse-1.0.10.tgz",
            "description": "Very powerful CLI arguments parser. Native port of argparse - python's options parsing library",
            "homepage": "https://github.com/nodeca/argparse#readme",
            "repository": "git+https://github.com/nodeca/argparse.git"
          },
          "esprima": {
            "from": "esprima",
            "version": "4.0.1",
            "resolved": "https://registry.npmjs.org/esprima/-/esprima-4.0.1.tgz",
            "description": "ECMAScript parsing infrastructure for multipurpose analysis",
            "homepage": "http://esprima.org",
            "repository": "git+https://github.com/jquery/esprima.git"
          }
        }
      }
      // list of more dependencies
    }
  }
]
```
