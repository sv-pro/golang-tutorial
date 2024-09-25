## Make a Golang module
```bash
go mod init github.com/username/repo
```

## Install a package
```bash
go get github.com/username/repo
```

## Run a file
```bash
go run main.go
```
## Use an existing library package inside a main package

### Import a package in a file
```go
package main

import "github.com/username/repo"
```
### make a local package available
```bash
go mod edit -replace=github.com/username/repo=../repo
```
### sync after editing go.mod
```bash
go mod tidy
```

