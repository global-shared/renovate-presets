# renovate-presets
Renovate bot presets for specific language configurations

Renovate's "config presets" are a convenient way to distribute config for reuse across multiple repositories. It is similar in design to ESLint's shareable configs, and can be used for whole repository configs and for individual rules. They are defined using the extends array within config and may also be nested.

Documentation for this configuration can be found [here](https://docs.renovatebot.com/config-presets/)

These presets can be used in each github repo in the .github/renovate.json file

An example of the file used for terraform code:

```
{
  "extends":[
     "github>global-shared/renovate-presets:terraform"
  ]
}
```

Making changes to these files will affect all repositories using them