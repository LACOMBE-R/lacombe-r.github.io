+++
draft = false
image = "img/portfolio/OTTO-MKS/Icon.png"
date = "2025-06-17T10:00:00+01:00"
title = "OTTO-MKS : un robot éducatif open-source pour la 1ère année"
weight = 3
+++

Développer un robot pédagogique open-source et évolutif pour initier les étudiants de première année à la robotique, à la fabrication numérique et à la programmation.

<!--more-->

---

## Présentation

Ce projet s’inscrit dans le cadre de mon **projet de fin d'étude** au sein du **MakerSpace d'UniLaSalle Amiens**, avec pour objectif général d’améliorer l’expérience des étudiants dans l’espace, notamment à travers des projets pédagogiques engageants.

Le projet **OTTO-MKS** est né d’un constat : les enseignements techniques de première année, répartis jusque-là en plusieurs modules isolés (mécanique, électronique, développement web), manquaient de cohérence et de transversalité. L’idée a donc été de concevoir un projet unique, fédérateur et concret, permettant d’aborder plusieurs compétences dans un format motivant : **la conception, la fabrication et la personnalisation d’un robot bipède.**

Ce robot, destiné à être assemblé, programmé et modifié par les étudiants, est une **version améliorée du robot OTTO original**, un projet open-source largement diffusé à l’international.

---

## Le robot OTTO original

![Otto-original](/img/portfolio/OTTO-MKS/Otto.png)

Le robot OTTO est un petit robot open-source conçu pour l’initiation à la robotique. Il est constitué :
- d’une **carte Arduino Nano** (le “cerveau” du robot),
- de **quatre servomoteurs** pour animer les jambes et les pieds,
- d’un **capteur ultrason** HC-SR04 pour détecter les obstacles,
- d’un **buzzer** pour émettre des sons,
- et d’une alimentation par **piles AA**.

Il peut marcher, danser, reculer, détecter les murs et se programme en Arduino ou en Blockly. Il est particulièrement apprécié pour son accessibilité dans les milieux éducatifs.

---

## Le projet OTTO-MKS

### Adaptation mécanique

La version **OTTO-MKS** conserve l’esprit du robot original mais en corrige plusieurs limitations, tout en restant **open-source**. Toutes les pièces ont été **modélisées sous Onshape**, une plateforme de CAO collaborative, afin que les étudiants puissent dupliquer, modifier et personnaliser leur robot.

Les principales améliorations :
- **Commutateur On/Off** déplacé sur le dessus (plus pratique que celui d’origine, situé sous le robot),
- **Fixation simplifiée** du capteur ultrason grâce à des connecteurs coudés sur mesure,
- Réduction du nombre de pièces et **assemblage possible avec une seule vis**,
- Intégration mécanique pensée pour faciliter les réparations, modifications et essais.

### Choix électroniques

- **Microcontrôleur : XIAO ESP32-C3**  
  → Compact, abordable (~4 €), Wi-Fi/Bluetooth intégré, compatible Arduino.
- **Alimentation : pile 9V rechargeable en USB-C**  
  → Recharge facile, câblage minimal.
- **Carte électronique dédiée** co-développée avec Adrien Bracq  
  → Organisation claire des branchements, évite les erreurs fréquentes chez les débutants.

### Itérations & prototypage

Le projet s’est étalé sur environ **quatre mois**, avec plusieurs versions testées et améliorées à partir du modèle OTTO original. Chaque modification est née d’une observation concrète : difficulté d’accès à un bouton, problème de câblage, temps de montage excessif, etc.

---

## Documentation et diffusion

Une **plateforme web** a été créée pour documenter entièrement le projet. On y retrouve :
- les fichiers CAO,
- les guides de montage,
- la présentation des composants,
- les bases de programmation Arduino.

Pour faciliter l’accès à cette documentation en atelier, des **QR codes** ont été apposés directement sur les boîtes de projet et les machines concernées. Ces ressources sont **mises à jour en continu** grâce aux retours des étudiants.

---

>#### Outils logiciels
>
>- **Onshape** (CAO collaborative)
>- **KiCad** (conception de la carte électronique)
>- **VSCode + Arduino IDE**
>- **Canva / Inkscape** (signalétique, schémas)
>- **Tinkercad Circuits** (simulations pédagogiques)

---

>#### Technologies
>
>- **[Impression 3D](https://makerspace-amiens.fr/pages/machines/)** (pièces du robot)
>- **[Électronique embarquée](https://makerspace-amiens.fr/pages/machines/)** (ESP32, servos, capteur)
>- **QR codes & documentation web** pour apprentissage en autonomie

---

## Conclusion

OTTO-MKS n’est pas simplement un robot : c’est un **support pédagogique transversal**, pensé pour les besoins réels des étudiants de première année. Il permet de découvrir, manipuler et modifier un objet technique tangible, tout en introduisant les outils et la culture Maker dans une logique progressive, collaborative et accessible.
