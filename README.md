<!--
SPDX-FileCopyrightText: NOI Techpark <digital@noi.bz.it>

SPDX-License-Identifier: CC0-1.0
-->

# project-landingpage

Static web pages of NOI Techpark projects. Each project lives in its own folder and is deployed to its own S3 bucket by the GitHub Actions workflow on every push to `main`.

| Folder | Bucket | URL |
| --- | --- | --- |
| `src/impact/` | `prod-impact-landingpage` | https://impact.digital.noi.bz.it |
| `src/mentor/` | `prod-mentor-landingpage` | https://journey.mentor.digital.noi.bz.it |

## Adding a project

1. Add a folder under `src/` with the static site.
2. Add an entry to the `deploy` matrix in `.github/workflows/main.yaml`.
3. Create the bucket and the proxy rule in the infrastructure repository.

## License

AGPL-3.0-or-later, see [LICENSE](LICENSE). The project is [REUSE](https://reuse.software) compliant.
