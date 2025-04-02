# Renovate Config

> My personal configuration preset for Mend Renovate.

This repository contains my configuration preset for [Mend Renovate][renovate]
(aka. "Renovate Bot" or "Renovate") which is used in many of my repositories to
automatically manage dependencies and security updates.
Renovate is very similar to Dependabot, but due to many additional features and
easier config sharing I have decided to use it in favor of Dependabot.

[renovate]: https://www.mend.io/renovate/

## Usage

When you give the Renovate GitHub App access to a new repository,
the onboarding PR created by Renovate should already suggest a config file
similar to the following:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jonasgeiler/renovate-config"
  ]
}
```

If not, create it manually and store it under `renovate.json` or
`.github/renovate.json` or [one of the other supported locations][options].

[options]: https://docs.renovatebot.com/configuration-options/
