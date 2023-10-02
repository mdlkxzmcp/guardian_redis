# Changelog

## Unreleased
GuardianDB 3.0 changes the way the it's configuration is done.
Change
```elixir
config :guardian, Guardian.DB, repo: GuardianRedis.Repo
```
in your config to:
```elixir
config :guardian, Guardian.DB, adapter: GuardianRedis.Adapter
```

### Added
- support for all configuration options of Redix (except for name)
- support for `name_prefix` config

### Breaking
- `port` and `pool_size` config options have to be integers now

### Breaking
- bump `GuardianDB` from 2.1.1 to 3.0.0

## V0.1.0

Initial release
