# Com assegurar SSH en un servidor

**Data:** 2026-10-02 · **Autor:** Aaron Sanchez

![Imatge SSH](../img/ssh.png)

SSH és la porta d'entrada principal a un servidor Linux, per això cal protegir-lo.

## Mesures bàsiques

* Desactivar l'accés de **root**.
* Fer servir *claus* en lloc de contrasenyes.
* Canviar el port per defecte (opcional).

```bash
sudo nano /etc/ssh/sshd_config
sudo systemctl restart ssh
```
