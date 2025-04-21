# MTLS-Go
A simple MTLS(Mututal Transport Layer Security) implemented in Go.

## Certificate Create Command
```shell
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
  -keyout key.pem -out cert.pem \
  -config cert.conf
```

## Start Server (Terminal 1)
```shell
go run server.go
```

## Start Client (Terminal 2)
```shell
go run clien.go 

```
Got `Hello World` as response from the server


## Reference Blog
1. [A step by step guide to mTLS in Go](https://venilnoronha.io/a-step-by-step-guide-to-mtls-in-go)
