# Release v38
*Déploiement effectué le : 16/07/2026 à 16:38*

## Nouveautés :
- Optimisation du script Batch de build avec détection automatique de l'âge du dernier firmware binaire via chemins absolus et PowerShell 
- Intégration de l'option de contournement 'Fast-Track' permettant un commit et push directs si le binaire a moins de 2 minutes 
- Remplacement du verrou temporel millis() par une vérification stricte basée sur l'Epoch Unix NTP dans handlePassiveOTACheck() 
- Ajout d'un Getter public isTimeSynchronized() dans la classe TimeManager pour valider l'accès Internet avant requêtage GitHub 
- Intégration d'un affichage dynamique du compte à rebours et de l'âge du binaire dans les logs de la console
---
# Release v37
*DÃ©ploiement effectuÃ© le : 16/07/2026 Ã  15:55*

## NouveautÃ©s :
- ImplÃ©mentation du laboratoire LED et du mode de dÃ©ploiement Express (Fast-Track) 
 - CrÃ©ation d'une page IHM dÃ©diÃ©e '/led_page' et d'une API '/set_led' pour piloter la LED RVB en direct 
 - Ajout de commandes interactives Ã©quivalentes dans l'onglet CRUD de l'application Python W8.py 
 - Optimisation du script Batch de build avec dÃ©tection automatique de l'Ã¢ge du dernier firmware binaire 
 - IntÃ©gration de l'option de contournement 'Fast-Track' permettant un commit et push directs si le binaire a moins de 2 minutes
---
# Release v36
*DÃƒÂ©ploiement effectuÃƒÂ© le : 16/07/2026 ÃƒÂ  15:13*

## NouveautÃƒÂ©s :
- AmÃƒÂ©lioration du script JavaScript checkReconnect() avec un compteur de tentatives pour avertir l'utilisateur sur l'IHM Web en cas de timeout local avec la box.
---
# Release v35
*DÃƒÆ’Ã‚Â©ploiement effectuÃƒÆ’Ã‚Â© le : 16/07/2026 ÃƒÆ’Ã‚Â  15:07*

## NouveautÃƒÆ’Ã‚Â©s :
Release OTA v28 - Centralisation du reboot et optimisation du buffer TLS 
  
 - Extraction et crÃƒÆ’Ã‚Â©ation de la mÃƒÆ’Ã‚Â©thode statique publique WifiConfigPortal::resetNextWakeup() pour ÃƒÆ’Ã‚Â©viter la duplication de code NVS. 
 - Mise ÃƒÆ’Ã‚Â  jour de performOTA() pour utiliser cette mÃƒÆ’Ã‚Â©thode centralisÃƒÆ’Ã‚Â©e de purge avant chaque redÃƒÆ’Ã‚Â©marrage (succÃƒÆ’Ã‚Â¨s ou ÃƒÆ’Ã‚Â©chec). 
 - Augmentation du buffer TLS ÃƒÆ’Ã‚Â  2048 octets dans la boucle de tÃƒÆ’Ã‚Â©lÃƒÆ’Ã‚Â©chargement pour accÃƒÆ’Ã‚Â©lÃƒÆ’Ã‚Â©rer le flashage via GitHub. 
 - IntÃƒÆ’Ã‚Â©gration de la sÃƒÆ’Ã‚Â©curitÃƒÆ’Ã‚Â© anti-triche basÃƒÆ’Ã‚Â©e sur la progression rÃƒÆ’Ã‚Â©elle de l'ÃƒÆ’Ã‚Â©criture en mÃƒÆ’Ã‚Â©moire Flash.
---
# Release v34
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  15:06*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
Release OTA v28 - Centralisation du reboot et optimisation du buffer TLS 
  
 - Extraction et crÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ation de la mÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©thode statique publique WifiConfigPortal::resetNextWakeup() pour ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©viter la duplication de code NVS. 
 - Mise ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  jour de performOTA() pour utiliser cette mÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©thode centralisÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©e de purge avant chaque redÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©marrage (succÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â¨s ou ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©chec). 
 - Augmentation du buffer TLS ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  2048 octets dans la boucle de tÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©lÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©chargement pour accÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©lÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©rer le flashage via GitHub. 
 - IntÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©gration de la sÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©curitÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© anti-triche basÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©e sur la progression rÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©elle de l'ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©criture en mÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©moire Flash.
---
# Release v29
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:56:50,43*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :

---

# Release v28
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:42:29,70*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- performOTA() entiÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â¨rement nettoyÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©e, optimisÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©e et fusionnÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©e avec toutes nos derniÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â¨res dÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©couvertes (gros buffer TLS de 2048 octets pour la vitesse, sÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©curitÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© anti-triche basÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©e sur la progression rÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©elle de l'ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©criture, et bascule automatique en arriÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â¨re-plan).

---

# Release v27
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:31:39,43*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- rien c pour les tests .. fix du .bat 

---

# Release v26
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:26:44,79*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- test v27

---

# Release v25
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:19:16,19*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- ajout minuteur et test v25

---

# Release v24
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:17:20,68*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- test OTA v24 

---

# Release v23
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  14:04:19,52*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- test OTA 

---

# Release v22
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  13:55:36,51*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- aiguillage entre les partitions et fix boucle infinie sur la mauvaise

---

# Release v21
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  13:46:13,04*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- test OTA

---

# Release v20
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  13:28:12,74*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- v20 ?

---

# Release v19
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  13:15:13,73*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- fix .bat O -> y 

---

# Release v18
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  12:57:37,57*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- fix .zip rapide

---

# Release v17
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  12:55:44,53*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- animation er reboot auto aprÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â¨s la mise ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  jour

---

# Release v16
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  12:25:39,75*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- le .zip fix pour test local et l'affichage pour la V16, donc test de l'OTA de v15 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  V16. let's go avec le test pour vois avec l'affichage des log sur le SAW

---

# Release v15
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  12:13:18,01*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- le.txt en .md

---

# Release v14
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  12:07:54,81*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- on a oubliÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le _internal pour la compil avec le .exe, donc on fait un zip pour le github et modif du readme aussi

---

# Release v13
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:59:46,36*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- le C par S dans LICENSE en version EN

---

# Release v12
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:57:50,17*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- fix github, licence et readme et le .bat

---

# Release v13
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:48:00,25*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- Synchro totale v13

---

# Release v12
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:44:03,88*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- oups j'ai delete le version.txt

---

# Release v11
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:38:00,30*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- fix du .bat variables d'environnement

---

# Release v10
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:34:38,49*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- test commit

---

# Release v9
*DÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©ploiement effectuÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â© le : 16/07/2026 ÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â  11:30:54,56*

## NouveautÃƒÆ’Ã†â€™Ãƒâ€šÃ‚Â©s :
- le.bat et le .md et tout le code ... 

---

# Release v8
*Deploiement : 16/07/2026 a 11:26:52,05*

## Nouveautes :
- realsenote 

---

# Release v7
*Deploiement : 16/07/2026 a 11:24:02,05*

## Nouveautes :
- changelog qui reste ? 

---

# Release v6

## Nouveautes :
- version markdown et fix de qq bouton

*Date de deploiement : 16/07/2026 a 11:20:28,18*