# Renovate Presets

This repository contains common presets for [Mend Renovate](https://www.mend.io/renovate/) that I use in my repositories.

## Usage

Just add the preset that you want to add to your `extends` field in the `renovate.json` file:
```json
{
  "extends": [ "github>jonasgeiler/renovate-presets:<name of the preset>" ]
}
````

### Example

```json
{
  "extends": [ "github>jonasgeiler/renovate-presets:base" ]
}
````
