## DNS Over TLS

DNS over TLS (DoT) is a security protocol for encrypting and wrapping Domain Name System (DNS) queries and answers via the Transport Layer Security (TLS) protocol. ([Wikipedia](https://en.wikipedia.org/wiki/DNS_over_TLS))

## Our DoT Servers

### Hostname for TLS Authentication

`dns.sb`

### TLS Port

`853`

### IPv4

```
185.222.222.222
185.184.222.222
```

### IPv6

```
2a09::
2a09::1
```

### IPv6 with Full Address

```
2a09:0000:0000:0000:0000:0000:0000:0000
2a09:0000:0000:0000:0000:0000:0000:0001
```

### Base 64 encoded form of SPKI pin(s) for TLS Authentication (RFC7858)

```
/qCm+kZoAyouNBtgd1MPMS/cwpN4KLr60bAtajPLt0k=
```

Expiry Date: Thursday, March 18, 2021

## Example Configurations

### Stubby

[stubby.yml](example/stubby.yml)