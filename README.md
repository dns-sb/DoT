## DNS Over TLS

DNS over TLS (DoT) is a security protocol for encrypting and wrapping Domain Name System (DNS) queries and answers via the Transport Layer Security (TLS) protocol. ([Wikipedia](https://en.wikipedia.org/wiki/DNS_over_TLS))

## Our DoT Servers

### Hostname for TLS Authentication

`dot.sb` or `dns.sb`

### TLS Port

`853`

### IPv4

```
185.222.222.222
185.184.222.222
```

### IPv6

```
Not supported now because Comodo does not support IPv6 on SSL certificates.
```

Expiry Date: Tue, 15 Mar 2022 23:59:59 GMT

### PEM / CRT File

[dns.sb.crt](cert/dns.sb.crt)

## Example Configurations

### Stubby

[stubby.yml](example/stubby.yml)

### Unbound

[unbound.conf](example/unbound.conf)

### Nebulo (Android App)

The server is included in this app. [Download it](https://git.frostnerd.com/PublicAndroidApps/smokescreen), open the server list at the bottom right and select DNS.SB
