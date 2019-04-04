# Helios

Helios is an Identity & Access Proxy (IAP) that authorizes HTTP requests based on sets of rules. 
The [BeyondCorp](https://beyondcorp.com) Model is designed by Google and secures applications in Zero-Trust networks. 
An Identity & Access Proxy is typically deployed in front of (think API Gateway) web-facing applications
and is capable of authenticating and optionally authorizing access requests.

## Development

### Prerequisites

 - Go 1.12
 - [mkcert](https://github.com/FiloSottile/mkcert)

### Environment Setup

Deploy local CA

```shell
mkcert -install
```

Create a certificate for local development

```shell
mkcert localhost 127.0.0.1
```

### Developing

Install dependencies

```shell
go mod download
```

Run the program

```shell
go run main.go
```