# Release publishing guide

This file is a maintainer checklist and reusable release-note template. GitHub does not apply it automatically.

## Before publishing

- Use a product-specific tag, such as `product-name/v1.0.0`, and title the release `Product Name 1.0.0`.
- Attach only intended public deliverables: installers, portable archives, plugin packages, and relevant documentation. Keep product source code, credentials, private configuration, signing keys, and internal files out of this repository and its release assets.
- Include the applicable LICENSE and copyright notice in each distribution package. Include third-party notices and comply with each bundled dependency's license.
- If different product-specific terms apply, identify them explicitly in the release notes and include them with the package.
- Check installation, supported platforms, version numbers, and package contents. Generate SHA-256 checksums after the files are final; attach `SHA256SUMS.txt` where practical.
- Mark preview builds as **Pre-release**. Only mark a release as the repository-wide latest when that designation is useful across this multi-product hub.
- Update the README's available-products section when publishing a product's first release, and remove its empty-state notice.

## Release-note template

```markdown
# Product Name 1.0.0

One sentence explaining what this tool does.

## Downloads

| Asset | Platform | Package |
| --- | --- | --- |
| Exact filename | OS and architecture | Installer / portable / plugin |

Download files from Assets below. The automatic Source code archives contain hub documentation only.

## Requirements

Supported operating systems, required host application versions, dependencies, and permissions.

## Installation and removal

Steps to install or load the tool, upgrade from an older version, and uninstall it.

## Changes

- Describe user-visible changes.

## Known limitations

List relevant limitations, or state that no known limitations are documented for this release.

## Integrity

When provided, compare the download's SHA-256 hash with SHA256SUMS.txt.

## License and credits

Copyright (c) 2026 Pedro "Frost" Lagoa (FrostLagoa).

Licensed under the FrostLagoa Public Release License 1.0 included with this download, unless different product-specific terms are explicitly stated here and included with the package. Non-commercial redistribution requires unchanged packages, preserved notices, and attribution linking to the hub and this release. Third-party components retain their own licenses.

## Support

Specify the product's support channel, or state that no support channel is offered for this release.
```
