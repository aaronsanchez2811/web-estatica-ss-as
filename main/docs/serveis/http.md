# HTTP

**HTTP** és el protocol de la web (port **80**; **443** amb HTTPS).

## Instal·lació d'Apache

```bash
sudo apt update
sudo apt install apache2
sudo systemctl enable --now apache2
curl -I http://localhost
```

## Codis de resposta

| Codi | Significat |
|------|------------|
| 200 | OK |
| 301 | Redirecció permanent |
| 404 | No trobat |
| 500 | Error del servidor |

Els fitxers web es troben a `/var/www/html/`.
