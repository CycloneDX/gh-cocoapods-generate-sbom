# gh-cocoapods-generate-sbom
GitHub action to generate a CycloneDX SBOM for Swift and Objective-C projects that use CocoaPods.

> This action uses [*cyclonedx-cocoapods*](https://github.com/CycloneDX/cyclonedx-cocoapods) to generate SBOMs.

## Inputs

### `version`

The version of *cyclonedx-cocoapods* to use.
Minimum allowed version is v1.0.0. Must be an [existing semantic version](https://github.com/CycloneDX/cyclonedx-cocoapods/releases).

### `some other input`

etc, etc...

## Example usage

```yaml
- name: Generate SBOMs
  uses: CycloneDX/gh-cocoapods-generate-sbom@v1

...to be filled in
```
