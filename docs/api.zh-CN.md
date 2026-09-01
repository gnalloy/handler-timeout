# API 参考

[English](api.md) | [文档索引](README.zh-CN.md)

本清单由本仓库 package 的 `go doc -short` 生成，用于快速查看公共面。精确语义以源码和测试为准。

## 包

### `gnalloy.org/handler-timeout`

包名：`timeout`

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
