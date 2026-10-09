# Permisos

Cada fitxer té permisos per a tres tipus d'usuari: **propietari**, **grup** i **altres**.

| Permís | Lletra | Valor numèric |
|--------|--------|---------------|
| Lectura | `r` | 4 |
| Escriptura | `w` | 2 |
| Execució | `x` | 1 |

## Exemples

```bash
ls -l fitxer.txt             # -rw-r--r-- 1 anna informatica ...
chmod 755 script.sh          # rwx per al propietari, r-x per a la resta
chmod u+x script.sh          # afegir execució al propietari
chown anna:informatica fitxer.txt
```

*Consell:* evita fer servir `chmod 777`, és una mala pràctica de seguretat.
