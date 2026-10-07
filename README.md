# 📱 ChatFlow Mobile

[![Expo SDK](https://img.shields.io/badge/Expo-SDK%2057-000020?style=for-the-badge&logo=expo&logoColor=white)](https://expo.dev)
[![React Native](https://img.shields.io/badge/React%20Native-0.86-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactnative.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](./LICENSE)

**ChatFlow Mobile** est une application mobile moderne et réactive de messagerie instantanée en temps réel, conçue avec **React Native**, **Expo**, **TypeScript**, **Zustand** et **Socket.io**.

---

## 🚀 Fonctionnalités Principales

- 💬 **Messagerie en Temps Réel** : Envoi et réception instantanés de messages grâce à **Socket.io**.
- 🔐 **Authentification Sécurisée** : Gestion de session et stockage sécurisé des tokens avec **Expo SecureStore**.
- 👥 **Gestion des Conversations** : Liste des discussions, indicateurs de messages non lus et présence en ligne.
- ⚡ **Gestion d'État Réactive** : Store global optimisé et fluide propulsé par **Zustand**.
- 🧭 **Navigation Fluide & Native** : Navigation par onglets et pile d'écrans via **React Navigation** (Bottom Tabs & Native Stack).
- 🎨 **Interface Moderne & Ergonomique** : Prise en charge des zones de sécurité (Safe Area), du mode sombre/clair et transitions natives.
- 🛡️ **Typage Strict** : Codebase 100% TypeScript pour une robustesse et une maintenabilité optimales.

---

## 🛠️ Stack Technique

| Domaine | Technologies |
| :--- | :--- |
| **Framework Mobile** | [React Native](https://reactnative.dev/) / [Expo SDK 57](https://expo.dev/) |
| **Langage** | [TypeScript](https://www.typescriptlang.org/) |
| **Navigation** | [React Navigation 7](https://reactnavigation.org/) (Native Stack & Bottom Tabs) |
| **State Management** | [Zustand](https://zustand-demo.pmnd.rs/) |
| **Temps Réel & Réseau** | [Socket.io Client](https://socket.io/), [Axios](https://axios-http.com/) |
| **Stockage Sécurisé** | [Expo SecureStore](https://docs.expo.dev/versions/latest/sdk/securestore/) |
| **Composants Système** | `react-native-safe-area-context`, `react-native-screens`, `expo-status-bar` |

---

## 📁 Architecture du Projet

```text
chatflow-mobile/
├── assets/                  # Icônes, logos et images statiques
├── src/
│   ├── api/                 # Configuration du client HTTP Axios et requêtes REST
│   ├── components/          # Composants UI réutilisables (boutons, inputs, bulles de chat)
│   ├── hooks/               # Hooks personnalisés
│   ├── navigation/          # Navigateurs (Stacks, Tabs, Guards d'authentification)
│   ├── screens/             # Écrans applicatifs
│   │   ├── auth/            # Connexion, inscription, mot de passe oublié
│   │   ├── chat/            # Écran de discussion en direct
│   │   └── conversations/   # Liste des conversations et contacts
│   ├── sockets/             # Gestionnaire de connexion et événements Socket.io
│   ├── store/               # Stores Zustand (authentification, chat, paramètres)
│   └── types/               # Définitions des types et interfaces TypeScript
├── App.tsx                  # Composant racine de l'application
├── app.json                 # Configuration globale du projet Expo
├── index.ts                 # Point d'entrée de démarrage Expo
├── package.json             # Dépendances et scripts de développement
└── tsconfig.json            # Configuration TypeScript
```

---

## 🏁 Démarrage Rapide

### 1. Prérequis

Assurez-vous d'avoir installé sur votre machine :
- [Node.js](https://nodejs.org/) (version 18+ recommandée)
- Un gestionnaire de paquets : `npm`, `yarn` ou `bun`
- L'application **Expo Go** sur votre smartphone ([iOS](https://apps.apple.com/app/expo-go/id982107779) / [Android](https://play.google.com/store/apps/details?id=host.exp.exponent)) ou un émulateur configuré (Android Studio / Xcode).

### 2. Cloner le Projet

```bash
git clone https://github.com/votre-compte/chatflow-mobile.git
cd chatflow-mobile
```

### 3. Installer les Dépendances

```bash
npm install
# ou avec bun
bun install
```

### 4. Lancer l'Application

Démarrez le serveur de développement Metro avec Expo :

```bash
npx expo start
```

Puis choisissez votre plateforme cible :
- 📱 **Expo Go / Appareil Physique** : Scannez le QR Code affiché dans le terminal avec l'application Expo Go (ou l'appareil photo sur iOS).
- 🤖 **Android** : Appuyez sur `a` dans le terminal ou lancez `npm run android`.
- 🍏 **iOS** : Appuyez sur `i` dans le terminal ou lancez `npm run ios` (macOS requis).
- 🌐 **Web** : Appuyez sur `w` dans le terminal ou lancez `npm run web`.

---

## 📜 Scripts Disponibles

| Commande | Description |
| :--- | :--- |
| `npm run start` / `npx expo start` | Démarre le serveur de développement interactif Expo |
| `npm run android` | Lance l'application sur un émulateur ou appareil Android connecté |
| `npm run ios` | Lance l'application sur le simulateur iOS |
| `npm run web` | Démarre l'application en mode Web pour le prototypage rapide |
| `npx tsc --noEmit` | Vérifie la cohérence et l'absence d'erreurs de typage TypeScript |
| `npx expo-doctor` | Diagnostique et vérifie l'intégrité de la configuration Expo |

---

## 📄 Licence

Ce projet est distribué sous la licence **MIT**. Consultez le fichier [LICENSE](./LICENSE) pour plus d'informations.
