# NEXUS PRO — Releases

Ce dépôt public ne contient **aucun code source** : uniquement les
installateurs officiels de **NEXUS PRO — Édition Atelier & Caisse**.

## Mises à jour automatiques

L'application installée vérifie la dernière release de ce dépôt
(`/releases/latest`), télécharge l'installateur `*Setup*.exe`, contrôle son
empreinte **SHA-256** quand GitHub fournit le digest, puis l'installe après
redémarrage — toujours avec confirmation de l'utilisateur.

- Paramètres › Données › Mise à jour : vérification manuelle et réglages.
- Un bandeau signale les nouvelles versions disponibles.
- Aucune installation silencieuse pendant le service.
- Les données locales (base, sauvegardes) sont conservées.

## Installation manuelle

1. Ouvrez la section **Releases**.
2. Téléchargez le dernier `NEXUS PRO Setup x.y.z.exe`.
3. Lancez-le : l'installation se fait par-dessus l'existante, sans supprimer
   la base locale.

## Sécurité

- Installateurs produits par `electron-builder` (NSIS, Windows x64).
- Vérification SHA-256 de l'asset avant installation.
- Source de confiance unique : ce dépôt. Ne modifiez pas le dépôt configuré
  dans l'application.

## Support

En cas de problème de mise à jour : créez une sauvegarde (Paramètres ›
Données), puis réinstallez manuellement l'installateur de la release
précédente. Les anciennes releases restent disponibles.
