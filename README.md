# 37124

Reproduction for [Renovate Discussion 37124](https://github.com/renovatebot/renovate/discussions/37124).

## Current behavior

Renovate Dependency Dashboard reports the following warning as seen in the [dashboard](https://github.com/jujaga/renovate-37124/issues/1):

```md
## Repository problems

These problems occurred while renovating this repository. [View logs](https://developer.mend.io//github/jujaga/renovate-37124).

 - WARN: Invalid hashicorp constraint
```

The warning log on Renovate repeats the following message multiple times:

```txt
WARN: Invalid hashicorp constraint
{
  "constraint": ".*-(alpha|beta|rc|next|preview|dev|experimental).*"
  "element": ".*-(alpha|beta|rc|next|preview|dev|experimental).*"
}
```

## Expected behavior

These warnings should not be present, as the HashiCorp constraint syntax is valid and sound.

## Link to the Renovate issue or Discussion

Reproduction for [Renovate Discussion 37124](https://github.com/renovatebot/renovate/discussions/37124).
