# Garmin Workout — For Chrome, Opera and Edge Extension

<div align="center">

![GarminWO](https://img.shields.io/badge/GarminWO-v1.4.20-00c9a7?style=for-the-badge)
![Chrome](https://img.shields.io/badge/Chrome-Extension-4285F4?style=for-the-badge&logo=googlechrome)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Languages](https://img.shields.io/badge/Languages-FR%20EN%20ES%20DE%20IT%20RU-orange?style=for-the-badge)

</div>

---

## 🇫🇷 Français

### Présentation
<img width="1280" height="800" alt="screenshot-1280x800-popup-fr" src="https://github.com/user-attachments/assets/dded3ce0-72fd-43fc-9c6e-e100c4b96465" />
<img width="1400" height="560" alt="promo-marquee-1400x560-fr" src="https://github.com/user-attachments/assets/3f5fa23a-2524-4ea2-aaa3-54a5cef86d64" />

**GarminWO** est une extension Chrome gratuite qui permet d'importer des séances d'entraînement running directement dans **Garmin Connect** depuis :

- 📸 Une **photo ou screenshot** de plan d'entraînement (JPG, PNG)
- 📝 Une **sélection de texte** sur n'importe quelle page web (Facebook, forum, site coach…)
- 📂 Un **fichier JSON** exporté depuis Garmin Connect


L'analyse visuelle ou textuelle est réalisée par une IA (**Google Gemini** gratuit ou **Anthropic Claude** payant) qui détecte automatiquement les étapes, allures et conditions de chaque séance.

Une fois importé dans Garmin Connect, l'entraînement peut être **transféré vers la montre** via le câble USB connecté à l'ordinateur, ou depuis l'**application mobile Garmin Connect**.

### Fonctionnalités

| Fonctionnalité | Description |
|---|---|
| 📸 Import via image | Glisse une photo ou screenshot → l'IA analyse et importe |
| 📝 Import via texte | Sélectionne du texte → clic droit → "Envoyer à GarminWO" |
| 📂 Import JSON | Fichier JSON Garmin exporté — sans appel IA |
| 🖱️ Menu clic droit | Clic droit sur image ou texte sélectionné sur n'importe quelle page |
| 🗑️ Suppression multiple | Cases à cocher dans la liste Garmin → suppression en masse |
| 🔄 Bouton Réessayer | Relance l'analyse en cas d'erreur API temporaire |
| ❓ Aide intégrée | Bouton ? dans le modal → ouvre le guide PDF dans la langue du navigateur |
| 🌍 10 langues | Français, Anglais, Espagnol, Allemand, Italien, Russe, Portugais, Brésilien, Chinois, Japonais |
| 🔒 Vie privée | Aucun serveur — aucune donnée collectée — clé API stockée localement |
| 🆓 Gratuit | Open source — Gemini offre 1500 analyses gratuites par jour |

---

## Utilisation
<img width="370" height="203" alt="image" src="https://github.com/user-attachments/assets/1609bf55-2190-458a-b4df-3108d75a7f6f" />

<img width="748" height="832" alt="image" src="https://github.com/user-attachments/assets/4d20d770-ab38-4426-b791-2fcac907201e" />

- Sélectionner l'entrainement puis clic droit et "Envoyer à GarminWO" :

<img width="944" height="865" alt="image" src="https://github.com/user-attachments/assets/96af8cf6-4012-4d0f-8064-737d37564a1e" />


- Choisir la séance et cliquer sur "Importer dans Garmin Connect" ou "Importer et ajouter au calendrier" si une date est disponible:

<img width="640" height="400" alt="Calendar640x400" src="https://github.com/user-attachments/assets/c409d40c-ea15-4207-afef-1134182edc59" />

- L'entrainement est mis en forme avec les temps VMA si sur "AUTO" ou "TOUJOURS" sinon basculer sur "JAMAIS":

<img width="955" height="1010" alt="image" src="https://github.com/user-attachments/assets/14e50ff5-7a40-4f9d-a654-060948db3e10" />

---

## Installation

#### Option 1 — Chrome Web Store (recommandé)

1. Ouvrez le [Chrome Web Store](https://chromewebstore.google.com)
2. Recherchez **Garmin Workout**: [https://chromewebstore.google.com/detail/garmin-workout-%E2%80%94-s%C3%A9ances/amlgfnkjdpandddidpmnjdeogcoanoia?hl=fr&utm_source=ext_sidebar](url)
   
  <img width="128" height="128" alt="logo-128" src="https://github.com/user-attachments/assets/da600151-19f5-4101-b8cb-018e41f8a076" />
  <img width="220"  alt="promo-tile-440x280-fr" src="https://github.com/user-attachments/assets/04b67ff7-77e2-48ea-b313-a3b4cd44276c" />
   
5. Cliquez sur **Ajouter à Chrome**
6. Confirmez avec **Ajouter l'extension**
7. Renseignez les informations demandées:
   
   <img width="372" height="647" alt="image" src="https://github.com/user-attachments/assets/1f8098a4-9d84-4165-a186-b8358495c144" />

8. Retrouvez sur la page "Entrainements" les boutons de mise en forme des séances, de lien et les cases à cocher pour supprimer des séances:
   <img width="1261" height="925" alt="GC_Trainings" src="https://github.com/user-attachments/assets/91893b9f-1a5d-40e6-8af2-eec337038271" />

#### Option 2 — Chargement manuel (mode développeur)

1. Téléchargez et décompressez ce dépôt
2. Dans Chrome, ouvrez `chrome://extensions`
3. Activez le **Mode développeur** (bouton en haut à droite)
4. Cliquez sur **Charger l'extension non empaquetée**
5. Sélectionnez le dossier décompressé

### Configuration

#### Gemini (Gratuit — recommandé)

1. Rendez-vous sur [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. Connectez-vous avec votre compte Google
3. Cliquez sur **Créer une clé API** et copiez-la
4. Cliquez sur l'icône GarminWO dans Chrome → collez la clé → **Sauvegarder**

> 🆓 Gemini 2.5 Flash est gratuit jusqu'à **1500 requêtes/jour**

#### Claude Anthropic (~0.01€ par analyse)

1. Créez un compte sur [console.anthropic.com](https://console.anthropic.com) (5$ de crédit offerts)
2. Allez dans **API Keys → Create Key** et copiez la clé
3. Dans le popup GarminWO, sélectionnez l'onglet **Claude** → collez la clé → **Sauvegarder**

### Utilisation

1. Connectez-vous sur [connect.garmin.com](https://connect.garmin.com) → **Entraînements**
2. Cliquez sur le bouton **📸 Lire image ou JSON** (apparu automatiquement)
3. Glissez votre photo ou screenshot → **Analyser** → **Importer**
4. L'entraînement s'ouvre automatiquement dans Garmin Connect
5. Transférez-le sur votre montre via câble USB ou l'application mobile

---

## 🇬🇧 English

### Overview
<img width="1280" height="800" alt="screenshot-1280x800-popup-en" src="https://github.com/user-attachments/assets/4b78d300-fc2d-4938-8101-59e2640570fa" />

<img width="1400" height="560" alt="promo-marquee-1400x560-en" src="https://github.com/user-attachments/assets/ddcdcbba-0e27-470a-8355-2db9fc15a5fe" />

**GarminWO** is a free Chrome extension that imports running workouts directly into **Garmin Connect** from:

- 📸 A **photo or screenshot** of a training plan (JPG, PNG)
- 📝 **Selected text** from any web page (Facebook, forum, coach website…)
- 📂 A **JSON file** exported from Garmin Connect

Visual or text analysis is performed by AI (**Google Gemini** free or **Anthropic Claude** paid) which automatically detects steps, paces and conditions for each session.

Once imported into Garmin Connect, the workout can be **transferred to your watch** via USB cable connected to your computer, or from the **Garmin Connect mobile app**.

### Features

| Feature | Description |
|---|---|
| 📸 Import from image | Drop a photo or screenshot → AI analyses and imports |
| 📝 Import from text | Select text → right-click → "Send to GarminWO" |
| 📂 JSON import | Exported Garmin JSON file — no AI call required |
| 🖱️ Right-click menu | Right-click any image or selected text on any web page |
| 🗑️ Bulk delete | Checkboxes in Garmin list → delete multiple workouts at once |
| 🔄 Retry button | Re-runs analysis on temporary API errors |
| ❓ Built-in help | ? button in modal → opens PDF guide in browser language |
| 🌍 10 languages | French, English, Spanish, German, Italian, Russian, Português, Brasilian, Chinese, Japanese |
| 🔒 Privacy | No server — no data collected — API key stored locally |
| 🆓 Free | Open source — Gemini offers 1500 free analyses per day |

### Installation

#### Option 1 — Chrome Web Store (recommended)

1. Open the [Chrome Web Store](https://chromewebstore.google.com)
2. Search for **Garmin Workout**
 
   <img width="128" height="128" alt="logo-128" src="https://github.com/user-attachments/assets/9b3d76bd-7631-41d5-aaa1-e71b6d9f6e80" />
 
   <img width="220" alt="promo-tile-440x280-en" src="https://github.com/user-attachments/assets/abc0e1c5-e456-4e13-8e6c-244b2be68369" />


4. Click **Add to Chrome**
5. Confirm with **Add extension**

#### Option 2 — Manual load (developer mode)

1. Download and unzip this repository
2. In Chrome, open `chrome://extensions`
3. Enable **Developer mode** (toggle in the top right)
4. Click **Load unpacked**
5. Select the unzipped folder

### Configuration

#### Gemini (Free — recommended)

1. Go to [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. Sign in with your Google account
3. Click **Create API Key** and copy it
4. Click the GarminWO icon in Chrome → paste the key → **Save**

> 🆓 Gemini 2.5 Flash is free up to **1500 requests/day**

#### Claude Anthropic (~$0.01 per analysis)

1. Create an account at [console.anthropic.com](https://console.anthropic.com) ($5 free credit)
2. Go to **API Keys → Create Key** and copy it
3. In the GarminWO popup, select the **Claude** tab → paste the key → **Save**

### Usage

1. Sign in at [connect.garmin.com](https://connect.garmin.com) → **Workouts**
2. Click the **📸 Import from image or JSON** button (injected automatically)
3. Drop your photo or screenshot → **Analyse** → **Import**
4. The workout opens automatically in Garmin Connect
5. Transfer it to your watch via USB cable or the mobile app

---

## Privacy Policy

[🇫🇷 Politique de confidentialité](https://daryan-bit.github.io/garminwo-extension/privacy_policy_fr.html) | [🇬🇧 Privacy Policy](https://daryan-bit.github.io/garminwo-extension/privacy_policy_en.html)

---

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for the full version history.

---

## Support

- 🐛 **Bug report / Feature request** → [Open an issue](https://github.com/Daryan-bit/garminwo-extension/issues)
- ☕ **Support the project** → [Ko-fi](https://ko-fi.com/YDARLAVOIX)

---

<div align="center">
Made with ❤️ for the running community — Powered by Claude & Gemini
</div>
