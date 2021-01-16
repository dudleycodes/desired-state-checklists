# Desired State Checklist: Go

## HTTP

* default `http.Client` is not used.
  * a timeout should *always* be set.
* `DefaultTransport` is not used.
  * `MaxConnsPerHost` and `MaxIdleConnsPerHost` should be set to a reasonable number.
  * `MaxIdleConns` should be set for reasonable connection pooling.

```go
  t := http.DefaultTransport.(*http.Transport).Clone()
  t.MaxIdleConns = 100
  t.MaxConnsPerHost = 100
  t.MaxIdleConnsPerHost = 100

  httpClient = &http.Client{
    Timeout:   10 * time.Second,
    Transport: t,
  }
```
