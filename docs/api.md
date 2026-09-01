# API Reference

[简体中文](api.zh-CN.md) | [Docs Index](README.md)

This inventory is generated from `go doc -short` for the packages in this repository. It is a quick public-surface map; source files and tests remain the authority for exact semantics.

## Packages

### `gnalloy.org/handler-timeout`

Package name: `timeout`

```text
var ErrReadTimeout = errors.New("gnalloy/handler/timeout: read timeout") ...
type IdleState uint8
    const ReaderIdle IdleState = iota ...
type IdleStateEvent struct{ ... }
type IdleStateHandler struct{ ... }
    func NewIdleStateHandler(readerIdleMillis int64, writerIdleMillis int64, allIdleMillis int64) *IdleStateHandler
type ReadTimeoutHandler struct{ ... }
    func NewReadTimeoutHandler(timeoutMillis int64) *ReadTimeoutHandler
type WriteTimeoutHandler struct{ ... }
    func NewWriteTimeoutHandler(timeoutMillis int64) *WriteTimeoutHandler
```
