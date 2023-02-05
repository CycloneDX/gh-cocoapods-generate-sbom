# gh-cocoapods-generate-sbom
GitHub action to generate a CycloneDX SBOM for Swift and Objective-C projects that use CocoaPods.

> This action uses [*cyclonedx-cocoapods*](https://github.com/CycloneDX/cyclonedx-cocoapods) to generate SBOMs.

## Inputs

### `version`

The version of *cyclonedx-cocoapods* to use.
Minimum allowed version is v1.0.0. Must be an [existing semantic version](https://github.com/CycloneDX/cyclonedx-cocoapods/releases).

## Example usage

Add the following entry to your Github workflow YAML file:

```
uses: CycloneDX/cyclonedx-cocoapods
with:
  path: '.'
```

### Example using all optional inputs:

```
uses: CycloneDX/cyclonedx-cocoapods
with:
  path: "."
  version: 1.1.1 # optional
  bom_version: 1 # optional
  component_type: application # optional
  component_group: com.example # optional
  component_name: App # optional
  component_version: 0.0.1 # optional
  exclude_test: true # optional
  output: bom.xml # optional
```