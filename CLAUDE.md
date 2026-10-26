@.claude/CLAUDE-commun.md

# CLAUDE.md — SmartAquaWiz-AMK4

Dépôt de livraison OTA du capteur AquaCheck (AMK4) : la flotte ESP32 et l'appli Windows AquaWiz y récupèrent les releases.
Dépôt partagé avec : Damien (et le compte JazzNeusta).
Config du socle : `_dev/projet.json`. Règles communes : `.claude/CLAUDE-commun.md` (ne pas dupliquer ici).

## Stack

- Aucun code source : `firmware.bin` (ESP32), `version.txt` (numéro de release entier, ex. `74`), `changelog.md`,
  `AquaWiz.zip` (appli Windows). Le code vit dans `../AquaCheck`.
- Tous ces fichiers sont générés par `AquaCheck/LANCER_WINDOWS.bat` → `MIP-BIN` (un commit « Release OTA vN ») : ne pas les éditer.
- Rien à installer, tester, construire ni lancer (toutes les `commandes` sont absentes de `projet.json`).

## Gros risques du projet

En plus de `CLAUDE-commun.md` § 3 :
- ⛔ Pousser sur `main` : la flotte lit `main` en OTA (`version.txt` + `firmware.bin`) et se reflashe sans intervention.
- ⛔ Publier ou remplacer `firmware.bin` à la main, hors de `LANCER_WINDOWS.bat` (qui exige une branche `PROD` propre d'AquaCheck).
- ⛔ Modifier `version.txt` : un numéro plus haut que celui des appareils déclenche l'OTA de toute la flotte.

## Pièges

- `version.txt` est un entier (`74`), pas un `x.y.z` : le socle ne sait pas le lire, `version` reste donc `null`.
- Le `README.md` et la `LICENSE` sont publics (dépôt de distribution) : n'y mets rien d'interne.
- Ce dépôt n'a pas de `.github/workflows/socle.yml` : la CI du socle n'y tourne pas.
- Ne travaille que sur `dev/socle-claude` : `main` est la branche lue par les appareils.
