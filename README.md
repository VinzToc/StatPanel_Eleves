# StatPanel (Applis EPS Élèves)
Version élèves de StatPanel : l'élève observe un camarade (ou une équipe, ou un match A contre B) et compte ses actions sur un panneau de boutons.

Dépôt conseillé : `StatPanel_Eleves` → https://vinztoc.github.io/StatPanel_Eleves/

- Identification de l'observateur par `eleve-core.js` (base locale « EPSEleves », jamais la liste du professeur).
- Le camarade observé est saisi à la main (nom, prénom, classe) ; une équipe = un élève par ligne « NOM Prénom ».
- Panneaux : création libre ou import du fichier `.xlsx` fourni par le professeur (feuille `StatPanel_Config`).
- « Fichier à remettre au prof » : `.xlsx` avec la feuille **statpanel** (+ `_meta`), rattachée à l'élève observé et portant la colonne **Observateur**. Le professeur l'importe dans Mes Apps EPS (onglet Import), qui met à jour la fiche de l'élève.
- Fonctionne hors ligne (PWA). Mise à jour : `APP_VERSION` dans `version.js` et `VERSION` dans `sw.js`.
