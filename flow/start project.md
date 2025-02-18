```sh
go mod init example/user/hello
```

```sh
module example/user/hello
```

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, world.")
}
```

モジュールをインストールする。

```sh
go install example/user/hello
```
1. builds the hello command
2. produces an executable binary
3. installs that binary as $HOME/go/bin/hello (or, under Windows, %USERPROFILE%\go\bin\hello.exe).

### 環境変数

```shell
go env -w GOBIN=/somewhere/else/bin
```

```shell
go env -u GOBIN
```