# ChatWork API Client for Golang

[ChatWork](http://www.chatwork.com/) client for Golang.

## Install

```
$ go get github.com/rskull/go-chatwork
```

## Usage

```go
package main

import (
  chatwork "github.com/rskull/go-chatwork"
)

func main() {
  chatwork := chatwork.NewClient(`api-key`)

  chatwork.Me()

  chatwork.MyStatus()

  chatwork.MyTasks(map[string]string {
    "assigned_by_account_id": "123",
    "status": "open"
  })

  ...
}
```

See more examples in `examples` directory.
