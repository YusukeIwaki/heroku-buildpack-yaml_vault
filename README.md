# heroku-buildpack-yaml_vault

This buildpack just decrypt config/secrets.yml.enc into config/secrets.yml with [@joker1007/yaml_vault](https://github.com/joker1007/yaml_vault)


## Setup

This buildpack assumes `heroku-buildpack-ruby` is already set.

Just execute:

```
heroku buildpacks:add https://github.com/YusukeIwaki/heroku-buildpack-yaml_vault --index 1 -a <your app>
```

(Don't forget to add `--index 1` option :beer: )

## Configure

Put your `config/secrets.yml.enc`,
and set the passphrase to the `YAML_VAULT_PASSPHRASE` environment variable.
