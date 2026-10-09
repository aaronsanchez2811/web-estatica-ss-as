# SSH

**SSH** permet accedir de manera segura i xifrada a un servidor remot (port **22**).

## Ús bàsic

```bash
ssh usuari@192.168.1.20
ssh-keygen -t ed25519          # generar parell de claus
ssh-copy-id usuari@192.168.1.20
scp fitxer.txt usuari@192.168.1.20:/tmp/
```

## Configuració del servidor

Fitxer `/etc/ssh/sshd_config`:

```text
PermitRootLogin no
PasswordAuthentication no
Port 22
```

Després de canviar-lo: `sudo systemctl restart ssh`.
