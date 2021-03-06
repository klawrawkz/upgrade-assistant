# Upgrade Assistant samples

This directory contains sample projects demonstrating how to create Upgrade Assistant add-ons using its [extensibility model](../docs/extensibility.md).

## Using the samples

To test out a sample, build the samples solution and then start Upgrade Assistant with the sample extension registered. This can be done in two ways:

1. Use the -e command line parameter when launching Upgrade Assistant and give it the path to either the extension's manifest file (ExtensionManifest.json) or the path where that file is located.
1. Set the environment variable `UpgradeAssistantExtensionPathsSettingName` to the extension manifest's path or directory. This environment variable can reference multiple extensions delimited by semicolons.

## Samples

| Sample | Features demonstrated |
| ------ | --------------------- |
| [UpgradeStepSample](./UpgradeStepSample) | Demonstrates how to create custom upgrade steps by making a sample upgrade step that ensures upgrade project files include a NuGet `<Authors>` property. |