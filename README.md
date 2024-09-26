## package-crawler

A crawler for packages distributed by Linux distros. This is a proof of concept for a multi-stage data processing pipeline in Go.

> **Disclaimer**: this project is in experimental stage.

## Quickstart

```shell
package-crawler --all PACKAGE_NAME 2>debug.log 1>result.json
```

## Development

### Testing

All tests:

```
go test -tags all_tests ./...
```

#### Unit tests

All unit tests:

```
go test -tags all_unit_tests ./...
```

Unit tests per feature:

```
go test -tags unit_tests,packages ./...
go test -tags unit_tests,database ./...
go test -tags unit_tests,repository ./...
```

#### Integration tests

All integration tests:

```
go test -tags all_integration_tests ./...
```

Integration tests per feature:

```
go test -tags integration_tests,packages ./...
go test -tags integration_tests,database ./...
go test -tags integration_tests,repository ./...
```

