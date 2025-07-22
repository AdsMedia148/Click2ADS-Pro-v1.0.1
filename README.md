# 🔔 Click2ADS Pro – Extension Chrome Click-to-Call

**Click2ADS Pro** est une extension Chrome professionnelle conçue pour les centres d’appels, commerciaux et équipes terrain. Elle permet de téléphoner en un clic via WebRTC ou téléphone IP (Yealink), avec des outils puissants comme un AutoDialer, un softphone intégré, des statistiques d’activité, et un tableau de bord SIP multi-comptes.

---

## 🚀 Fonctionnalités disponibles

### 🏠 Popup principal (Click2Call)
- 📲 Saisie manuelle du numéro à appeler
- 🎛️ Sélection du compte SIP par défaut
- ☎️ Appel en un clic via :
  - WebRTC (navigateur)
  - AMI → Téléphone IP (ex. Yealink)
- 🔁 Démarrage et arrêt d’un **AutoDialer**
- ✅ Détection automatique du canal d’émission
- 🌐 Case à cocher "WebRTC activé"
- 🪟 Ouverture automatique du softphone WebRTC dans une popup
- 📤 Enregistrement du dernier numéro utilisé
- 📊 Accès direct à la page **Statistiques**
- ⚙️ Accès direct à la page **Options**

### ⚙️ Options (Gestion des comptes SIP)
- ➕ Formulaire d’ajout de comptes SIP
- 📝 Champs pris en charge :
  - Nom, Extension, Domaine, Utilisateur, Mot de passe, Port
- ✅ Activation WebRTC individuelle par compte
- 🌟 Définition du **compte par défaut**
- 📋 Affichage des comptes en tableau responsive
- ✏️ Édition des comptes existants
- 🗑️ Suppression immédiate de comptes
- 🟢🔴 Badges de statut par compte :
  - SIP (enregistré)
  - AMI (connecté)
  - WebSocket (WebRTC actif)
- 🔐 Masquage du mot de passe dans l’interface
- ⚠️ Limitation à 10 comptes (sécurité/UX)

### 📞 Softphone WebRTC (popup dédiée)
- 📡 Connexion automatique au serveur SIP WebSocket (WSS)
- 🧠 Récupération dynamique du numéro à appeler
- 📞 Appeler / Raccrocher
- 🔇 Mute / Unmute en direct
- 🎹 Clavier numérique masqué (toggle)
- 🧾 Affichage du compte SIP actif
- 🔁 Reconnexion automatique en cas d’erreur réseau
- ✅ Indicateur de statut : Connecté, En appel, Terminé

### 📊 Statistiques (stats.html)
- 🕒 Lecture des appels passés (stockés localement)
- 🔎 Filtres disponibles :
  - Période (date de début/fin)
  - Statut (réussi, échoué, répondeur…)
  - Indicatif (ex : +33, +44)
  - Extension utilisée
- 📈 Graphiques dynamiques :
  - 📊 Camembert des statuts
  - 📉 Ligne d’évolution par jour
- 🗂️ Tableau détaillé des appels :
  - Date, numéro, durée, statut, extension
- ⬇️ Export CSV
- 🖨️ Export PDF (via impression)
- ♻️ Nettoyage automatique si >1000 appels

### 🔁 AutoDialer intégré
- 🎯 Lecture automatique d’une liste de numéros
- ⏩ Passage au contact suivant après réponse ou raccrochage
- 🧠 Intégration **AMD (Answering Machine Detection)**
  - Détection des répondeurs (HUMAN / MACHINE)
- 🛑 Bouton STOP pour interrompre la séquence
- 📝 Mise à jour automatique du statut des appels dans les logs

### 🔒 Sécurité & stockage
- 🔐 Sauvegarde locale via `chrome.storage.local`
- 🔒 Aucune donnée transmise hors navigateur sans consentement
- 🧼 Nettoyage automatique des anciens logs
- 🧠 Validation de tous les champs (formulaires sécurisés)
- 🛡️ Encodage visuel des mots de passe SIP
- 🧩 Architecture modulaire, sans dépendance serveur imposée

---

## 📁 Structure du projet

click2ads-pro/
├── manifest.json
├── popup.html / popup.js
├── options.html / options.js
├── stats.html / stats.js
├── webrtc_ui.html / webrtc_ui.js
├── dialer.js / utils.js
├── img/ (icônes 16, 48, 128 px)
└── docs/ (PDF utilisateur)

---

## 📄 Documentation complète

📘 Guide illustré : `docs/Click2ADS-Pro-Guide.pdf`  
Contient toutes les étapes d'installation, de configuration, et de déploiement Chrome Web Store.

---

## 🧠 Technologies utilisées

- JavaScript (vanilla)
- SIP.js (WebRTC)
- Chart.js (statistiques)
- Chrome Extension – Manifest V3
- Local Storage (`chrome.storage.local`)
- FreePBX / Asterisk (via API AMI)

---

## 📜 Licence

© 2025 – Ads Media Consulting Ltd  
Produit propriétaire. Toute reproduction, modification ou diffusion sans autorisation est interdite.
