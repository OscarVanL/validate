# Local checks

## Test

`go test ./...`

## Lint

Note: Ensure you are using the same linter version as in CI (.github/workflows/go.yml. Eg: `version: v1.49.0`)

Via docker:
`docker run --rm -v $(git rev-parse --show-toplevel):/app -w /app golangci/golangci-lint:v1.49.0 golangci-lint run --fix`

Or natively:
`golangci-lint --version`
`golangci-lint run --fix`
