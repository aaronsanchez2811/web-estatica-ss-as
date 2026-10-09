# Còpies de seguretat amb rsync

**Data:** 2026-10-08 · **Autor:** Aaron Sanchez

![Imatge Backup](../img/backup.png)

Una còpia de seguretat que no es prova **no és una còpia de seguretat**. `rsync` copia només els canvis.

```bash
rsync -av --delete /dades/ /backup/dades/
rsync -av /dades/ usuari@servidor:/backup/
```

Es pot automatitzar amb `cron`:

```text
0 2 * * * rsync -av /dades/ /backup/dades/
```

Més informació a la [pàgina oficial de rsync](https://rsync.samba.org/).
