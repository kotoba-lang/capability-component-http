# capability-component-http

Atomic authority package for `component/http`.

- imports: `#{:http-open :http-close :http-write :http-read :http-get}`
- effects: `#{:data-egress :network-read :network-write}`
- default policy: `:approval-required`
- provider status: `contract-only`

Importing this package does not grant runtime authority. Tamaki must
request it explicitly and Kototama must admit the sealed envelope.

```sh
clojure -M:test
```
