# Memòria breu

## Problemes i solucions
* **Ruta massa llarga** en clonar el repositori (error *Filename too long*): vaig clonar-lo en una carpeta curta de l'escriptori.
* **Menú sense Linux**: una modificació del `mkdocs.yml` va fallar; ho vaig corregir en un commit (`Fix navigation menu`).

## Decisions de configuració
Tema `readthedocs` (inclòs a MkDocs), CSS propi (`extra.css`) amb color verd, menú definit a `nav` i `site_url` per a GitHub Pages. Els fitxers del projecte (`mkdocs.yml` i `docs/`) són a l'arrel del repositori.

## SSG utilitzat i comparació
MkDocs: simple i orientat a documentació. Hugo és el més ràpid i flexible però més complex; Jekyll és el que integra GitHub Pages de manera nativa, però depèn de Ruby.

## GitHub Pages i Actions
GitHub Pages serveix fitxers estàtics des del repositori. El workflow de GitHub Actions (s'activa a cada `push`) construeix la web amb MkDocs i la desplega sense passos manuals.

## Qüestionari final
1. **SSG:** programa que genera una web HTML a partir de Markdown, plantilles i configuració.
2. **Markdown vs HTML:** el Markdown és el text font fàcil d'escriure; l'HTML és el resultat final que llegeix el navegador.
3. **Git:** sistema de control de versions.
4. **Git vs GitHub:** Git és l'eina local; GitHub és el servei web que allotja repositoris Git.
5. **GitHub Pages:** servei per publicar webs estàtiques des d'un repositori.
6. **git push:** envia els commits locals al repositori remot de GitHub.
7. **Modificar Markdown i regenerar:** l'SSG torna a crear l'HTML amb el canvi.
8. **Diferències:** MkDocs és el més senzill per a documentació; Hugo és més ràpid; Jekyll necessita Ruby.
9. **Avantatges web estàtica:** ràpida, segura, barata i fàcil d'allotjar.
10. **Ús empresarial:** documentació interna, webs corporatives i blogs.
11. **SSG per a documentació tècnica:** MkDocs, per la seva senzillesa i cerca integrada.
12. **SSG per a web corporativa:** Hugo, per la velocitat i flexibilitat de plantilles.
13. **GitHub Actions:** automatitza tasques (compilar, provar, desplegar) a partir d'esdeveniments.
14. **Avantatges d'automatitzar:** menys errors, estalvi de temps i publicacions consistents.

## Repte final
Sí, recomanaria un SSG per a documentació interna amb centenars de pàgines: és segur (no hi ha base de dades ni codi al servidor), ràpid, de cost mínim, fàcil d'editar en Markdown, versionat amb Git i es desplega automàticament. Triaria **MkDocs** per la facilitat d'edició i la cerca; Hugo seria millor si les pàgines fossin milers.
