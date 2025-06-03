# 🏙️ SmartSafeCity

[![Node-RED](https://img.shields.io/badge/Node--RED-8F0000?logo=nodered&logoColor=white)](https://nodered.org/)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)](https://firebase.google.com/)
[![MQTT](https://img.shields.io/badge/MQTT-660066?logo=mqtt&logoColor=white)](https://mqtt.org/)

> **Une solution IoT intelligente pour la sécurité urbaine en temps réel**

SmartSafeCity est un système de surveillance urbaine intelligent qui combine capteurs IoT, intelligence artificielle et notifications mobiles pour détecter et signaler instantanément les incidents de sécurité dans les espaces urbains.

![Architecture SmartSafeCity](https://github.com/user-attachments/assets/4abf066a-c413-49da-bd2c-2c9b6f0bccaa)

## 🎯 Objectifs du Projet

Le projet SmartSafeCity vise à :

### ✅ **Démonstration Technique**
- Prouver la faisabilité d'un système unifié combinant capteurs IoT simulés, IA et notifications mobiles
- Valider l'efficacité d'une architecture distribuée pour la sécurité urbaine

### 🔄 **Chaîne de Traitement Complète**
- **Détection** : Simulation d'événements critiques (fumée, vibrations, violence)
- **Transmission** : Communication via protocole MQTT
- **Orchestration** : Filtrage et gestion des alertes avec Node-RED
- **Notification** : Diffusion instantanée via Firebase Cloud Messaging
- **Stockage** : Archivage structuré des incidents dans Firestore

### ⚡ **Performance**
- Obtenir des temps de latence optimisés pour une intervention rapide
- Garantir une réactivité compatible avec les situations d'urgence

### 🛠️ **Expertise Technologique**
- Maîtriser l'intégration de technologies open source (Mosquitto, Node-RED)
- Exploiter les solutions cloud (Firebase FCM, Firestore) dans un contexte de ville intelligente

## 🏗️ Architecture

```
┌─────────────┐    MQTT     ┌─────────────┐    FCM      ┌─────────────┐
│   Capteurs  │────────────▶│  Node-RED   │────────────▶│   Mobile    │
│     IoT     │             │ Orchestrateur│             │    App      │
└─────────────┘             └─────────────┘             └─────────────┘
                                   │
                                   ▼ Firestore
                            ┌─────────────┐
                            │   Base de   │
                            │   Données   │
                            └─────────────┘
```

## 🚀 Fonctionnalités

### 🔍 **Détection Multi-Capteurs**
- **Détecteurs de fumée** : Surveillance incendie
- **Capteurs de vibration** : Détection d'activités suspectes
- **Analyse vidéo IA** : Reconnaissance de comportements violents

### 📱 **Notifications Intelligentes**
- Alertes push instantanées
- Géolocalisation précise des incidents
- Classification automatique des urgences

### 📊 **Tableau de Bord**
- Monitoring en temps réel
- Historique des événements
- Analyse des tendances de sécurité

## 🛠️ Technologies Utilisées

| Composant | Technologie | Description |
|-----------|-------------|-------------|
| **IoT Communication** | MQTT (Mosquitto) | Protocole léger pour capteurs |
| **Orchestration** | Node-RED | Workflow automation |
| **Notifications** | Firebase FCM | Push notifications |
| **Base de Données** | Firestore | NoSQL cloud database |
| **Interface Mobile** | Android/iOS | Application mobile native |

## 📋 Prérequis

- Node.js (v14+)
- Node-RED
- Mosquitto MQTT Broker
- Compte Firebase configuré
- Android Studio / Xcode (pour l'app mobile)

## 🚀 Installation Rapide

1. **Cloner le repository**
   ```bash
   git clone https://github.com/Aagi1/SmartSafeCity.git
   cd SmartSafeCity
   ```

2. **Installer les dépendances**
   ```bash
   npm install
   ```

3. **Configurer Firebase**
   - Créer un projet Firebase
   - Télécharger le fichier de configuration
   - Configurer FCM et Firestore

4. **Lancer les services**
   ```bash
   # Démarrer Mosquitto
   mosquitto -c mosquitto.conf
   
   # Lancer Node-RED
   node-red
   ```

## 📱 Application Mobile

L'application mobile companion permet de :
- Recevoir les notifications d'urgence
- Visualiser la carte des incidents
- Consulter l'historique des alertes
- Signaler des incidents manuellement

## 🔒 Sécurité

- Chiffrement des communications MQTT
- Authentification Firebase sécurisée
- Validation des données capteurs
- Logs d'audit complets

## 👥 Équipe

- AKPINFA AKOTCHAYE GILLES-INGRID (https://github.com/Aagi1)
- KOFFI PIERRE DAMIEN
- LORO TRIOMPHE
- TIDO TAMEKENG BOREL

<div align="center">
  <p><strong>🏙️ Construisons ensemble des villes plus sûres et intelligentes</strong></p>
  <p>⭐ N'hésitez pas à star le projet si vous le trouvez utile !</p>
</div>
