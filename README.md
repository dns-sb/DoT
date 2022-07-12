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
45.11.45.11
```

### IPv6

```
2a09::
2a11::
```

### IPv6 with Full Address

```
2a09:0000:0000:0000:0000:0000:0000:0000
2a11:0000:0000:0000:0000:0000:0000:0000
```

### PEM / CRT File

[dns.sb.crt](cert/dns.sb.crt)

### SPKI Pin

```
0Ot+uUBCfWZkE2GFQQcIpR9GmuhWioGEl+K11FhNmHk=
```
You can generate and verify SPKI PIN with the following command:

```bash
echo | openssl s_client -connect 185.222.222.222:853 2>/dev/null | openssl x509 -pubkey -noout | openssl pkey -pubin -outform der | openssl dgst -sha256 -binary | openssl enc -base64
```

## Example Configurations

### Unbound

[unbound.conf](example/unbound.conf)

### Nebulo (Android App)

The server is included in this app. [Download it](https://git.frostnerd.com/PublicAndroidApps/smokescreen), open the server list at the bottom right and select DNS.SB
