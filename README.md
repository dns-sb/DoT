## DNS Over TLS

DNS over TLS (DoT) is a security protocol for encrypting and wrapping Domain Name System (DNS) queries and answers via the Transport Layer Security (TLS) protocol. ([Wikipedia](https://en.wikipedia.org/wiki/DNS_over_TLS))

## Our DoT Servers

### IPv4

```
185.222.222.222@853
185.184.222.222@853
```

### IPv6

```
2a09::@853
2a09::1@853
```

### IPv6 with Full Address

```
2a09:0000:0000:0000:0000:0000:0000:0000@853
2a09:0000:0000:0000:0000:0000:0000:0001@853
```

## Example Configurations

### Stubby

[stubby.yml](example/stubby.yml)