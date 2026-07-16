# Release v43
*Déploiement effectué le : 16/07/2026 à 17:06*

## Nouveautés :
Intégration du laboratoire de création led_studio et de l'API de contrôle interactive 
- Création d'une interface web dédiée '/led_page' dans le WifiConfigPortal avec le diagramme interactif de la machine à états native 
- Ajout d'un espace de création 'led_studio' équipé d'un sélecteur de couleurs (cercle colorimétrique) et de 5 slots mémoires configurables (durée d'affichage Xms et boucle Loop) 
- Implémentation de la route API REST '/api/play_custom_led' (requêtes HTTP POST) pour analyser les structures JSON d'ArduinoJson et piloter en direct les GPIO matériels (14, 27, 26) de l'AMK4 
- Mise à jour de l'onglet CRUD de l'application Python Windows W8.py avec alignement strict des contrôles de la machine à états et gestion asynchrone des threads d'envoi pour éviter le gel de l'IHM 
- Correction de la syntaxe Tkinter et des callbacks d'événements (lambda event) sur le clic des slots de couleurs
---
# Release v42
*Déploiement effectué le : 16/07/2026 à 16:53*

## Nouveautés :
by pass 5min -> 30s
---
# Release v41
*Déploiement effectué le : 16/07/2026 à 16:47*

## Nouveautés :
- Optimisation du script Batch de build avec détection automatique de l'âge du dernier firmware binaire via chemins absolus et PowerShell
- Intégration de l'option de contournement 'Fast-Track' permettant un commit et push directs si le binaire a moins de 2 minutes
- Remplacement du verrou temporel millis() par une vérification stricte basée sur l'Epoch Unix NTP dans handlePassiveOTACheck()
- Ajout d'un Getter public isTimeSynchronized() dans la classe TimeManager pour valider l'accès Internet avant requêtage GitHub
- Intégration d'un affichage dynamique du compte à rebours et de l'âge du binaire dans les logs de la console

---

# Release v40
*Déploiement effectué le : 16/07/2026 à 16:45*

## Nouveautés :
- Optimisation du script Batch de build avec détection automatique de l'âge du dernier firmware binaire via chemins absolus et PowerShell
- Intégration de l'option de contournement 'Fast-Track' permettant un commit et push directs si le binaire a moins de 2 minutes
- Remplacement du verrou temporel millis() par une vérification stricte basée sur l'Epoch Unix NTP dans handlePassiveOTACheck()
- Ajout d'un Getter public isTimeSynchronized() dans la classe TimeManager pour valider l'accès Internet avant requêtage GitHub
- Intégration d'un affichage dynamique du compte à rebours et de l'âge du binaire dans les logs de la console

---

# Release v39
*Déploiement effectué le : 16/07/2026 à 16:44*

## Nouveautés :
- Optimisation du script Batch de build avec détection automatique de l'âge du dernier firmware binaire via chemins absolus et PowerShell
- Intégration de l'option de contournement 'Fast-Track' permettant un commit et push directs si le binaire a moins de 2 minutes
- Remplacement du verrou temporel millis() par une vérification stricte basée sur l'Epoch Unix NTP dans handlePassiveOTACheck()
- Ajout d'un Getter public isTimeSynchronized() dans la classe TimeManager pour valider l'accès Internet avant requêtage GitHub
- Intégration d'un affichage dynamique du compte à rebours et de l'âge du binaire dans les logs de la console

---

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
*Déploiement effectué le : 16/07/2026 à 15:55*

## Nouveautés :
- Implémentation du laboratoire LED et du mode de déploiement Express (Fast-Track) 
- Création d'une page IHM dédiée '/led_page' et d'une API '/set_led' pour piloter la LED RVB en direct 
- Ajout de commandes interactives équivalentes dans l'onglet CRUD de l'application Python W8.py 
- Optimisation du script Batch de build avec détection automatique de l'âge du dernier firmware binaire 
- Intégration de l'option de contournement 'Fast-Track' permettant un commit et push directs si le binaire a moins de 2 minutes

---

# Release v36
*Déploiement effectué le : 16/07/2026 à 15:13*

## Nouveautés :
- Amélioration du script JavaScript checkReconnect() avec un compteur de tentatives pour avertir l'utilisateur sur l'IHM Web en cas de timeout local avec la box.

---

# Release v35
*Déploiement effectué le : 16/07/2026 à 15:07*

## Nouveautés :
- Extraction et création de la méthode statique publique WifiConfigPortal::resetNextWakeup() pour éviter la duplication de code NVS. 
- Mise à jour de performOTA() pour utiliser cette méthode centralisée de purge avant chaque redémarrage (succès ou échec). 
- Augmentation du buffer TLS à 2048 octets dans la boucle de téléchargement pour accélérer le flashage via GitHub. 
- Intégration de la sécurité anti-triche basée sur la progression réelle de l'écriture en mémoire Flash.

---

# Release v34
*Déploiement effectué le : 16/07/2026 à 15:06*

## Nouveautés :
- Extraction et création de la méthode statique publique WifiConfigPortal::resetNextWakeup() pour éviter la duplication de code NVS. 
- Mise à jour de performOTA() pour utiliser cette méthode centralisée de purge avant chaque redémarrage (succès ou échec). 
- Augmentation du buffer TLS à 2048 octets dans la boucle de téléchargement pour accélérer le flashage via GitHub. 
- Intégration de la sécurité anti-triche basée sur la progression réelle de l'écriture en mémoire Flash.

---

# Release v29
*Déploiement effectué le : 16/07/2026 à 14:56:50*

## Nouveautés :
- Nettoyage du fichier d'historique.

---

# Release v28
*Déploiement effectué le : 16/07/2026 à 14:42:29*

## Nouveautés :
- performOTA() entièrement nettoyée, optimisée et fusionnée avec toutes nos dernières découvertes (gros buffer TLS de 2048 octets pour la vitesse, sécurité anti-triche basée sur la progression réelle de l'écriture, et bascule automatique en arrière-plan).

---

# Release v27
*Déploiement effectué le : 16/07/2026 à 14:31:39*

## Nouveautés :
- Ajustements et correctifs sur le script d'automatisation .bat pour les validations de tests.

---

# Release v26
*Déploiement effectué le : 16/07/2026 à 14:26:44*

## Nouveautés :
- Phase de test intermédiaire pour validation de la v27.

---

# Release v25
*Déploiement effectué le : 16/07/2026 à 14:19:16*

## Nouveautés :
- Ajout d'un minuteur de sécurité sur le portail captif et tests de montée de version v25.

---

# Release v24
*Déploiement effectué le : 16/07/2026 à 14:17:20*

## Nouveautés :
- Banc d'essai fonctionnel pour la validation de la routine OTA v24.

---

# Release v23
*Déploiement effectué le : 16/07/2026 à 14:04:19*

## Nouveautés :
- Série de tests à blanc sur l'infrastructure de téléchargement OTA GitHub.

---

# Release v22
*Déploiement effectué le : 16/07/2026 à 13:55:36*

## Nouveautés :
- Correction de l'aiguillage entre les partitions applicatives OTA et résolution du bug de boucle infinie sur la mauvaise partition au boot.

---

# Release v21
*Déploiement effectué le : 16/07/2026 à 13:46:13*

## Nouveautés :
- Déploiement d'une version de test pour la validation du comportement de la table des partitions.

---

# Release v20
*Déploiement effectué le : 16/07/2026 à 13:28:12*

## Nouveautés :
- Incrémentation technique de sécurité v20.

---

# Release v19
*Déploiement effectué le : 16/07/2026 à 13:15:13*

## Nouveautés :
- Correction du script Batch : remplacement du commutateur de validation global O par y.

---

# Release v18
*Déploiement effectué le : 16/07/2026 à 12:57:37*

## Nouveautés :
- Correctif rapide sur la routine d'archivage et de génération de l'archive zip de distribution.

---

# Release v17
*Déploiement effectué le : 16/07/2026 à 12:55:44*

## Nouveautés :
- Ajout de l'animation de chargement sur l'IHM web et forçage du redémarrage automatique après application réussie de la mise à jour.

---

# Release v16
*Déploiement effectué le : 16/07/2026 à 12:25:39*

## Nouveautés :
- Intégration du dossier _internal dans le package zip final pour le fonctionnement du test local. Validation du cycle de mise à jour complet de la v15 vers la v16 avec affichage structuré des logs sur la console du SAW.

---

# Release v15
*Déploiement effectué le : 16/07/2026 à 12:13:18*

## Nouveautés :
- Migration et conversion du journal de modifications brut au format Markdown standard (.md).

---

# Release v14
*Déploiement effectué le : 16/07/2026 à 12:07:54*

## Nouveautés :
- Inclusion des dépendances Python de PyInstaller dans le pack de livraison, automatisation de la compression zip sur GitHub et mise à jour de la documentation d'accueil.

---

# Release v13
*Déploiement effectué le : 16/07/2026 à 11:59:46*

## Nouveautés :
- Correction typographique mineure dans le fichier LICENSE pour la version anglophone.

---

# Release v12
*Déploiement effectué le : 16/07/2026 à 11:57:50*

## Nouveautés :
- Alignement du dépôt distant, mise à jour des mentions légales, du guide de démarrage et du script d'automatisation.

---

# Release v13
*Déploiement effectué le : 16/07/2026 à 11:48:00*

## Nouveautés :
- Synchronisation complète de l'arborescence v13.

---

# Release v12
*Déploiement effectué le : 16/07/2026 à 11:44:03*

## Nouveautés :
- Restauration de sécurité suite à la suppression involontaire du marqueur version.txt.

---

# Release v11
*Déploiement effectué le : 16/07/2026 à 11:38:00*

## Nouveautés :
- Résolution des conflits d'affectation sur les variables d'environnement locales du script d'initialisation.

---

# Release v10
*Déploiement effectué le : 16/07/2026 à 11:34:38*

## Nouveautés :
- Validation initiale de la structure d'envoi automatique des commits.

---

# Release v9
*Déploiement effectué le : 16/07/2026 à 11:30:54*

## Nouveautés :
- Déploiement initial de l'architecture d'orchestration, du journal de bord, du microcode embarqué et de l'outil d'IHM.

---

# Release v8
*Déploiement effectué le : 16/07/2026 à 11:26:52*

## Nouveautés :
- Écriture de la note de mise à jour de référence.

---

# Release v7
*Déploiement effectué le : 16/07/2026 à 11:24:02*

## Nouveautés :
- Test de persistance des variables d'état de l'historique local.

---

# Release v6
*Déploiement effectué le : 16/07/2026 à 11:20:28*

## Nouveautés :
- Initialisation de la mise en page sous format Markdown et résolution de dysfonctionnements sur les boutons de commande de l'interface.