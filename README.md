# Renovate Config

This repository contains my configuration and common presets for [Mend Renovate](https://www.mend.io/renovate/) (aka. "Renovate Bot" or "Renovate") which is used in many of my repositories to manage dependencies and security updates.
Renovate is very similar to Dependabot, but due to many additional features and easier config sharing I have decided to use it in favor of Dependabot.

## Usage

The onboarding PR created by Renovate should already suggest a config file similar to the following:
```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jonasgeiler/renovate-config"
  ]
}
```
If not, create it manually and store it under `renovate.json` or `.github/renovate.json` or [one of the other supported locations](https://docs.renovatebot.com/configuration-options/).

### Using the common presets

To use the presets included in this repository you will have to extend them like so:
```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jonasgeiler/renovate-config",
    "github>jonasgeiler/renovate-config:<preset>"
  ]
}
```
For example:
```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jonasgeiler/renovate-config",
    "github>jonasgeiler/renovate-config:yaml-version-comments"
  ]
}
````
