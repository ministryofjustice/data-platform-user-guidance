# Data Platform User Guidance

The Data Platform User Guidance is a portal intended to provide supplementary information about the [Data Platform](https://github.com/ministryofjustice/data-platform), such as how to guides, as well as comms and blogs for prospective users and anyone else interested in learning about the platform.

Implemented using the [GOV.UK Eleventy Plugin](https://github.com/x-govuk/govuk-eleventy-plugin), it is a node.js-based static site generator with content written in Markdown. 

## Technical documentation

See the [GOV.UK Eleventy Plugin documentation](https://x-govuk.github.io/govuk-eleventy-plugin/get-started/) for instructions on how to use this site's tooling.

For more advanced configurations, see the [Eleventy documentation](https://www.11ty.dev/). 

Note that not all configurations in the Eleventy documentation are compatible with the GOV.UK Eleventy Plugin.

### Before running the app (if applicable)

To preview documentation locally, you require a Docker installation. Otherwise, ensure you meet the requirements stated in the [Plugin's Get Started guide](https://x-govuk.github.io/govuk-eleventy-plugin/get-started/).

### Previewing the documentation

The `--npx eleventy serve` command does not work with this repository as we use Docker instead for previewing documentation.

Instead, once you have installed Docker, navigate to the root directory and run `bash scripts/serve.sh`.

## Licence

[MIT License](https://github.com/ministryofjustice/data-platform-user-guidance/blob/main/LICENSE)