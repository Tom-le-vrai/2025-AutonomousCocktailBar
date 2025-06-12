---
layout: default
nav_order: 4
title: Études et choix techniques
---

# Études et choix techniques

 Études et choix techniques
Cette partie présente les différentes solutions étudiées pour chaque composant ou sous-système du projet, ainsi que les raisons motivant les choix finaux. Elle justifie l’architecture retenue du point de vue mécanique, électronique et logiciel.

1. Choix du système d’automatisation
🔍 Étude :
Plusieurs plateformes ont été envisagées : Arduino UNO, Raspberry Pi, ESP32.

Critères : connectivité, puissance de calcul, nombre d’E/S, consommation.

✅ Choix : ESP32
Microcontrôleur double cœur performant.

Connectivité Wi-Fi et Bluetooth intégrées.

Suffisamment de broches PWM, digitales et UART.

Idéal pour héberger un serveur web local sans matériel supplémentaire.

2. Choix du moteur
🔍 Étude :
Moteur DC : rotation continue mais nécessite un encodeur pour le contrôle précis.

Servo-moteur : précis, mais rotation limitée.

Moteur pas à pas : parfait pour les déplacements linéaires avec précision.

✅ Choix : Moteur pas à pas NEMA 17
Précision de déplacement sans besoin de capteur de position.

Couple suffisant pour déplacer un verre sur rail.

Facilement contrôlable via un driver dédié.

3. Choix du driver moteur
🔍 Étude :
A4988 : économique, mais bruyant et peu de fonctions intelligentes.

DRV8825 : plus puissant mais sans détection de blocage.

TMC2209 : silencieux, intelligent, configurable.

✅ Choix : TMC2209
StallGuard : détecte les blocages sans capteur.

CoolStep : adapte le courant pour réduire la consommation.

StealthChop2 : permet un fonctionnement très silencieux.

4. Choix de la structure mécanique
🔍 Étude :
Structures imprimées en 3D : légères mais moins robustes.

Châssis en bois : facile à usiner mais peu modulaire.

Profilés aluminium V-slot : solides, modulables et adaptés aux courroies.

✅ Choix : Profilés aluminium + courroie crantée
Permet un déplacement fluide et précis.

Modularité pour ajuster la taille ou ajouter des composants.

Facile à assembler avec des pièces standards (roues, pignons, etc.).

5. Choix du système de contrôle
🔍 Étude :
Interface via bouton physique (simple mais non connectée).

Application mobile (nécessite un développement externe).

Serveur web intégré sur ESP32 (léger, local, accessible).

✅ Choix : Interface web intégrée
Aucune application à installer, fonctionnement via navigateur.

Interface HTML/CSS simple avec deux boutons de commande (gauche / droite).

Contrôle du moteur en temps réel via Wi-Fi.

6. Choix du système de mesure (option non finalisée)
🔍 Étude :
Capteurs de débit : coûteux, difficiles à calibrer.

Cellules de charge : précises mais nécessitent un traitement du signal.

Mesure optique : solution envisagée (barre optique) pour détecter un volume servi.

🧪 Statut : en cours de test
Objectif futur : activer automatiquement l’arrêt du dosage à 50 mL.