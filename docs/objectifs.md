---
layout: default
nav_order: 3
title: Objectifs du projet
---

# Introduction
Dans les environnements festifs ou événementiels, la rapidité et la précision de service sont essentielles. Ce projet vise à automatiser la distribution de boissons à l’aide d’un système motorisé précis, pour garantir un dosage fiable et répétable.

# Contexte du Projet
Dans le cadre des environnements festifs, événementiels ou de restauration, la rapidité et la précision dans la distribution de boissons sont des éléments clés pour améliorer l’expérience utilisateur et optimiser le service. Cependant, la distribution manuelle est souvent sujette à des erreurs de dosage, des temps d’attente et des risques d’hygiène.

Ce projet vise à concevoir et réaliser un bar automatique, capable de verser une quantité précise de boisson (50 mL) de façon automatisée, rapide et répétable. L’objectif est de garantir un service efficace tout en réduisant l’intervention humaine.

Le système repose sur :

Un moteur pas à pas assurant le contrôle précis du positionnement pour le versement.

Une structure en profilés aluminium, solide et modulaire, permettant un montage fiable et évolutif.

Un dispositif de mesure ou de calibration, garantissant la quantité exacte de boisson à chaque cycle.

Ce projet s’inscrit dans une démarche de robotisation de tâches simples mais essentielles, et constitue une base de travail adaptable à différents types de boissons, contextes d’utilisation et extensions (paiement sans contact, interface utilisateur, capteurs de niveau, etc.).

# Objectifs du Projet
Objectifs: Créer une machine capable de verser automatiquement une boisson.

Utiliser un moteur pas à pas pour contrôler la position.

S’assurer d’un volume précis (50 mL) à chaque service.

Construire une structure solide et modulaire en profilés aluminium.

# Existant
Voici quelques projets déjà existant:


Nous nous sommes inspirés de ces différents dans la conception, la modélisation et aussir pour comprendre comment le coder.

# Cahier des Charges
 Cahier des charges – Projet de bar à cocktail automatique
1. Contexte du projet
Le projet consiste à concevoir un bar à cocktail automatique, capable de préparer des boissons de manière autonome. Ce système vise à simplifier la préparation de cocktails en assurant précision, rapidité, et interaction simple via une interface utilisateur connectée. Ce projet s’inscrit dans une démarche d’automatisation ludique, combinant électronique, programmation et mécanique.

2. Objectifs fonctionnels
Le système doit être capable de :

Déplacer automatiquement un verre le long d’un rail.

Distribuer des doses précises de différentes boissons.

Contrôler les déplacements du verre via une interface web.

Offrir une interaction simple et en temps réel via Wi-Fi.

Permettre l’ajout de plusieurs recettes/cocktails différents.

3. Contraintes techniques
Précision du dosage : ±5 mL par service.

Motorisation : moteur pas à pas piloté par un driver TMC2209.

Structure : châssis en profilés aluminium (V-slot) avec support mobile pour le verre.

Capteurs : système de mesure optique pour contrôler le volume servi (non finalisé).

Microcontrôleur : ESP32 avec Wi-Fi intégré.

Interface : serveur web embarqué, accessible via smartphone ou PC.

Alimentation : batterie ou alimentation 12V.

4. Contraintes matérielles
Dimensions compactes (transportable sur une table).

Utilisation de composants abordables et facilement disponibles.

Robustesse de l’assemblage (support verre stable).

Modularité : possibilité d’ajouter d’autres moteurs ou bouteilles.

5. Contraintes logicielles
Utilisation de l’environnement Arduino IDE.

Programmation en C++ (Arduino).

Interface HTML/CSS simple intégrée dans le code ESP32.

Réponse en temps réel aux commandes utilisateur (latence minimale).

6. Performances attendues
Déplacement du verre précis et fluide.

Fonctionnement silencieux grâce au StealthChop2 du TMC2209.

Réduction de la consommation électrique (CoolStep activable).

Interaction utilisateur intuitive via page web (interface responsive).

7. Critères de validation
Le verre peut se déplacer automatiquement de gauche à droite.

Un moteur peut distribuer une dose fixe de liquide (mesure simulée si nécessaire).

L’utilisateur peut contrôler le système via Wi-Fi.

Le support assure la stabilité du verre pendant les déplacements.

8. Améliorations possibles
Intégration d’un système de levage du verre pour le service.

Ajout d’un écran de contrôle local (OLED ou TFT).

Automatisation complète de la préparation de recettes.

Ajout de capteurs de niveau de liquide ou fin de course.