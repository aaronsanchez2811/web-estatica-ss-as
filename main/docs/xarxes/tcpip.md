# TCP/IP

TCP/IP és el conjunt de protocols que fa funcionar Internet i les xarxes locals.

## Capes

1. **Aplicació**: HTTP, SSH, DNS...
2. **Transport**: TCP i UDP.
3. **Internet**: IP.
4. **Accés a la xarxa**: Ethernet, Wi-Fi.

## Exemple d'adreçament

| Camp | Valor |
|------|-------|
| Adreça IP | 192.168.1.10 |
| Màscara | 255.255.255.0 (/24) |
| Porta d'enllaç | 192.168.1.1 |

## Comandes útils

```bash
ip a                  # veure adreces IP
ip route              # veure la taula de rutes
ping -c 4 8.8.8.8     # comprovar connectivitat
```
