---
layout: default
title: Assemblage
parent: Etapes de fabrication
nav_order: 2
---

# Étape 2 – Assemblage
Après la préparation minutieuse des matériaux, l’étape suivante consiste à assembler les différentes pièces mécaniques et électroniques du système. Cette phase est essentielle pour garantir la stabilité et la fonctionnalité globale de l’ensemble.

# Étapes d’assemblage
Organisation

Disposez tous les composants (mécaniques et électroniques) sur un espace de travail dégagé.

Classez les éléments par type : profilés, vis, pièces imprimées, courroie, électronique.

Assemblage initial

Montez la structure principale en fixant les profilés aluminium à l’aide des équerres et visseries.

Installez les roues V-slot sur le support de verre.

Positionnez la courroie crantée dans la rainure du rail et autour de la poulie.

Fixation

Fixez fermement le moteur pas à pas à son support en veillant à l’alignement de la poulie avec la courroie.

Vissez solidement le support de verre sur le chariot mobile.

Raccordez le driver TMC2209 au moteur, puis connectez-le à l’ESP32 selon le schéma de câblage.

# Vérifications à effectuer
Alignement :

Vérifiez que la poulie et la courroie sont bien alignées pour éviter toute déviation lors du déplacement.

 Stabilité :

Testez la rigidité de la structure en appliquant une légère pression.

Assurez-vous que le support de verre glisse sans accrocs sur le rail.

 Connexion :

Contrôlez chaque branchement électrique avec un multimètre (continuité, polarité, court-circuit).

| Problème                        | Cause probable                           | Solution                                          |
| ------------------------------- | ---------------------------------------- | ------------------------------------------------- |
| Courroie qui saute ou se détend | Mauvaise tension ou mauvais alignement   | Ajuster la tension, réaligner la poulie           |
| Support de verre qui coince     | Roues mal montées ou rail sale           | Resserrer les roues, nettoyer le rail             |
| Moteur ne tourne pas            | Mauvais câblage ou manque d’alimentation | Revoir le câblage, tester la tension              |
| Vibrations anormales            | Mauvais serrage des vis ou frottements   | Resserrer toutes les fixations, vérifier les axes |
