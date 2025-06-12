---
layout: default
title: Etapes de fabrication
nav_order: 6
has_children: true
---

# Étapes de Fabrication
1. Préparation des pièces
Découpe des profilés aluminium selon les dimensions souhaitées pour former la structure du rail.

Sélection et tri des composants : moteur pas à pas NEMA 17, driver TMC2209, courroie, roues V-slot, visserie, ESP32.

Impression ou fabrication du support de verre adapté aux dimensions standards d’un gobelet.

2. Assemblage mécanique
Montage de la structure du rail à l’aide de connecteurs pour les profilés.

Installation des roues V-slot sur le support mobile.

Fixation de la courroie crantée sur le support de verre et passage de celle-ci autour de la poulie.

Montage du moteur pas à pas en alignement avec la poulie pour entraîner la courroie.

3. Montage électronique
Connexion du moteur au driver TMC2209.

Raccordement du driver à l’ESP32 via les broches STEP, DIR et GND.

Alimentation séparée du moteur via une source 12V, avec ajout d’un condensateur de filtrage pour stabiliser la tension.

Vérification des connexions via un schéma de câblage réalisé au préalable.

4. Programmation de l’ESP32
Rédaction et upload du code via l’IDE Arduino.

Implémentation d’un serveur web local avec HTML/CSS embarqué.

Tests des fonctions : connexion Wi-Fi, affichage de la page, activation des boutons, déclenchement du moteur.

Réglage des temps d’impulsions et du nombre de pas pour un mouvement fluide et suffisant.

5. Tests fonctionnels
Vérification du déplacement correct du support à gauche et à droite.

Validation de la réponse de l’interface web.

Ajustement mécanique (tension de la courroie, alignement) pour assurer la fluidité du déplacement.

Test de robustesse : résistance du support, stabilité pendant le mouvement.

6. Améliorations et ajustements
Analyse des limites du système (ex : activation de la mesure optique non implémentée).

Préparation pour intégrer un second moteur ou des éléments supplémentaires (levage du verre, distributeur).

Proposition d’optimisations futures pour fiabiliser ou enrichir le projet.

## Commencer

Avant de commencer, assurez-vous de :

Bien comprendre chaque étape,

Avoir à disposition tous les outils et composants nécessaires,

Suivre l’ordre proposé pour garantir la fiabilité, la qualité et la sécurité du système

---

Pour toute question ou aide supplémentaire, n'hésitez pas à contacter notre équipe.
