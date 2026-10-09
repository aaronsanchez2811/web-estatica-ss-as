# DNS

El **DNS** (*Domain Name System*) tradueix noms de domini a adreces IP.

## Tipus de registres

| Registre | Funció |
|----------|--------|
| A | Nom → IPv4 |
| AAAA | Nom → IPv6 |
| MX | Servidor de correu |
| CNAME | Àlies d'un altre nom |

## Consultes

```bash
dig github.com            # consulta completa
dig +short github.com A   # només l'adreça
nslookup github.com
cat /etc/resolv.conf      # servidors DNS configurats
```
