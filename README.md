## Bloem community build

This is Bloem's community build of [brettpetch/silo-plugin-sportarr](https://github.com/brettpetch/silo-plugin-sportarr) by **brettpetch**
(contributors: brettpetch). It is ported to the Bloem plugin SDK and listed in the
Bloem community plugin catalog. All credit for the plugin goes to its author; please
report plugin behavior issues upstream. See [NOTICE](NOTICE) for provenance.

---

# Silo Sportarr Plugin

First-party Silo metadata plugin backed by [Sportarr](https://sportarr.net). Provides sports league metadata as TV shows, with series, seasons, and episodes mapped from leagues, seasons, and events.

## Dependency Model

This repository consumes `github.com/Silo-Server/silo-plugin-sdk` as a normal Go module dependency. CI and release builds run with `GOWORK=off` and expect the SDK version in `go.mod` to resolve from a published semver tag.

For local multi-repo development, use a temporary `replace` or a local `go.work` that points at `dev/github/silo-plugin-sdk`. Do not commit machine-local filesystem replaces as the supported release path.

## Development

```sh
go test ./...
go build .
```

## Attribution

Metadata provided by [Sportarr](https://sportarr.net).

## License

`silo-plugin-sportarr` is licensed under `AGPL-3.0-or-later`. See [LICENSE](LICENSE).
