# Yam’s — Feuille de score & Classement

**Version actuelle : v7.4.6**

Une petite application PWA (Progressive Web App) simple et élégante pour suivre les scores du jeu de Yam’s (Yahtzee). Conçue pour être utilisée sur tous types d’appareils (mobile, tablette, desktop), avec un mode clair/sombre, en-têtes figées, stats, PDF export, et plus encore.

---

##  Fonctionnalités clés

- Saisie intuitive des scores par catégorie (1×, 2×, ..., Chance, etc.), avec limite maximale par catégorie pour éviter les erreurs.
- Colonne **Catégorie** bien alignée (sticky) pour une lecture claire pendant le scroll horizontal.
- **Classement unifié** : option de vue  
  - Manche actuelle  
  - Moyenne de toutes les manches  
  - Nombre de victoires
- Un seul bouton intuitif, qui change de fonction selon le contexte : **“Clôturer la manche”** / **“Nouvelle manche”**.
- **Stockage local** des scores et de l'historique des manches, avec une **sauvegarde détaillée (par catégorie)** pour chaque partie.
- **Statistiques joueurs** : moyenne, victoires, podiums, tendance, série de victoires, etc., avec un graphique clair et légendé.
- **Export/Import JSON** des données, **export PDF** bien structuré (scores, classements, fiches joueurs) et impression-friendly.
- **Safe Mode + Service Worker v12.6** avec bouton intégré pour vider le cache et forcer la mise à jour.

---

##  Technologie & Déploiement

- 100% HTML, CSS et JavaScript **sans dépendances externes**.
- PWA compatible, donc **installable et utilisable hors ligne**.
- **Service Worker (sw-v12.6.js)** pour la gestion du cache et des mises à jour.
- Utilise **localStorage** pour les données persistantes (état, historique, préférences UI).

---

## 🚀 Accès direct

Pas besoin d’installer quoi que ce soit, l’application est disponible en ligne :  
👉 [Accéder à l’application Yam’s](https://baptjeannerod.github.io/yams-app_v1/)

---

## 📲 Utilisation hors-ligne (optionnel)

L’app est une **Progressive Web App (PWA)** :  
- Sur **mobile ou tablette**, tu peux l’ajouter à ton écran d’accueil via le menu “Partager” → *Ajouter à l’écran d’accueil*.  
- Sur **ordinateur (Chrome/Edge/Brave)**, tu peux cliquer sur l’icône “Installer” dans la barre d’adresse.  
Une fois installée, elle fonctionne même sans connexion internet.

---

##  Utilisation

- **Ajouter un joueur** : saisir un nom puis cliquer sur *Ajouter*.
- **Saisir les scores** : entrer les valeurs directement dans les champs ; les totaux et bonus se mettent à jour instantanément.
- **Clôturer une manche** : conserve les données dans l’historique et vide la grille pour la manche suivante.
- **Voir l’historique** : bouton *Historique* pour consulter les anciennes manches.
- **Statistiques détaillées** : cliquer sur l’icône stats à côté du nom d’un joueur.
- **Exporter / Importer JSON**, **Exporter PDF** ou **Vider le cache** via le menu Réglages.

---

##  Idées futures

- Icône visuelle (ombre ou bordure) sur la colonne sticky pour plus de clarté.
- Adaptations pour plus de petites tailles d’écran (responsive split view, etc.).
- Paramètres avancés (mode multi-rouleaux, modes de jeu variés, automatisation des lancers, etc.).
- Option de partage/export vers des services cloud (Dropbox, etc.).

---

##  Licence

Ce projet est **open-source** — libre à toi de l’utiliser et de le modifier.
