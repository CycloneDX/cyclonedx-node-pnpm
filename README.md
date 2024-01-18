[![shield_license]][license_file]  
[![shield_website]][link_website]
[![shield_slack]][link_slack]
[![shield_groups]][link_discussion]
[![shield_twitter-follow]][link_twitter]

----

# cyclonedx-pnpm

Create [CycloneDX] Software Bill of Materials (SBOM) from  _[pnpm]_ projects.

## 🚧 🏗️ this project is in early development stage

See the projects [issues](https://github.com/CycloneDX/cyclonedx-node-pnpm/issues),
[pull requests](https://github.com/CycloneDX/cyclonedx-node-pnpm/pulls) and
[milestones](https://github.com/CycloneDX/cyclonedx-node-pnpm/milestones) for the progress.

Development will happen in branch [`1.0-dev`](https://github.com/CycloneDX/cyclonedx-node-pnpm/tree/1.0-dev).

## Requirements

* `node` >= `16`
* `pnpm` in range `7 - 8`

## Internals

This tool utilizes the [CycloneDX library][cyclonedx-library] to generate the actual data structures.

This tool does **not** expose any additional _public_ API or classes - all code is intended to be internal and might change without any notice during version upgrades.

## License

Permission to modify and redistribute is granted under the terms of the Apache 2.0 license.  
See the [LICENSE][license_file] file for the full license.

[CycloneDX]: https://cyclonedx.org/
[cyclonedx-library]: https://www.npmjs.com/package/%40cyclonedx/cyclonedx-library
[pnpm]: https://pnpm.io/

[license_file]: https://github.com/CycloneDX/cyclonedx-node-pnpm/blob/1.0-dev/LICENSE

[shield_license]: https://img.shields.io/github/license/CycloneDX/cyclonedx-node-pnpm?logo=open%20source%20initiative&logoColor=white "license"
[shield_website]: https://img.shields.io/badge/https://-cyclonedx.org-blue.svg "homepage"
[shield_slack]: https://img.shields.io/badge/slack-join-blue?logo=Slack&logoColor=white "slack join"
[shield_groups]: https://img.shields.io/badge/discussion-groups.io-blue.svg "groups discussion"
[shield_twitter-follow]: https://img.shields.io/badge/Twitter-follow-blue?logo=Twitter&logoColor=white "twitter follow"

[link_website]: https://cyclonedx.org/
[link_slack]: https://cyclonedx.org/slack/invite
[link_discussion]: https://groups.io/g/CycloneDX
[link_twitter]: https://twitter.com/CycloneDX_Spec
