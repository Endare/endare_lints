# The `endare_lints` package

This repository defines the lint rules for Dart and Flutter projects
tailored to the Endare BVBA [Code Style Guide](https://endare.atlassian.net/wiki/spaces/MISC/pages/2878177281/Code+Style+Guidelines).

These lint rules extend the [flutter_lints](https://pub.dev/packages/flutter_lints) lint set, which defines lint rules for Flutter projects. `flutter_lints` itself is an extension of the recommended lint set for Dart projects.

## Release process

Whenever the language deprecates old rules or adds new rules that are relevant to the style guide,
a new version of this package will be published that incorporates those changes.

Whenever fixes to existing lint rules (i.e. fixing false positives) are published,
a new version of this package will be published that incorporates those changes.

## Getting started

Add this package to your dependencies:

```shell
flutter pub add endare_lints --dev
```

This will add `endare_lints` as a dev dependency to your project:

```yaml
dev_dependencies:
  endare_lints: ^1.0.0
```

Add a reference to the lint rules in your `analysis_options.yaml`:

```yaml
include: package:endare_lints/endare_lints.yaml
```