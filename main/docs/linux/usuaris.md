# Usuaris i grups

Linux és un sistema **multiusuari**. Cada usuari té un identificador (*UID*) i pertany a un o més grups (*GID*).

## Fitxers importants

| Fitxer | Contingut |
|--------|-----------|
| `/etc/passwd` | Llista d'usuaris |
| `/etc/shadow` | Contrasenyes xifrades |
| `/etc/group` | Llista de grups |

## Comandes habituals

```bash
sudo useradd -m -s /bin/bash anna     # crear usuari
sudo passwd anna                      # assignar contrasenya
sudo groupadd informatica             # crear grup
sudo usermod -aG informatica anna     # afegir l'usuari al grup
id anna                               # veure UID i grups
```

Més informació: [man useradd](https://man7.org/linux/man-pages/man8/useradd.8.html).
