Looking to upgrade from `http-proxy@1.x.x` to `http-proxy@2.0`? You've come to the right place!
`http-proxy@2.0` is a forked version of `http-proxy@1.18.1` and
brings some breaking changes to APIs.

## Proxy Request/Response Events

As the event-based approach does not support waiting for completion of asynchronous functions the events `proxyReq`, `proxyReqWs`, `proxyRes`, `start`, `end`, `open` and `close` got removed. 
Use there option counterparts `onProxyReq`, `onProxyReqWs`, `onProxyRes`, `onStart`, `onEnd`, `onOpen` and `onClose` instead.


The deprecated event `proxySocket` was removed. Use the now added option `onOpen` instead.