# Firewall senzill amb UFW

**Data:** 2026-10-05 · **Autor:** Aaron Sanchez

![Imatge Firewall](../img/firewall.png)

**UFW** (*Uncomplicated Firewall*) és una manera fàcil de gestionar `iptables` a Ubuntu.

| Comanda | Efecte |
|---------|--------|
| `ufw allow 22/tcp` | Permet SSH |
| `ufw allow 80/tcp` | Permet HTTP |
| `ufw status` | Mostra les regles |

```bash
sudo ufw default deny incoming
sudo ufw allow 22/tcp
sudo ufw enable
```
