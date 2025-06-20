+++
draft = false
image = "img/portfolio/OTTO-MKS/icon.png"
date = "2025-06-17T10:00:00+01:00"
title = "OTTO-MKS : un robot éducatif "
weight = 3
+++

Développer un robot pédagogique open-source pour faire découvrir la robotique, la fabrication numérique et la programmation embarquée aux étudiant·e·s en première année d'école d'ingénieur ? C’est exactement ce qu’on a fait.

<!--more-->

---

## Présentation

Ce projet s’inscrit dans le cadre de mon **projet de fin d'étude** au sein du **MakerSpace d'UniLaSalle Amiens**. L’un de mes objectifs était de repenser entièrement les enseignements technologiques des premières années, en créant des projets concrets, motivants et accessibles.

Plutôt que d’enchaîner les modules isolés de méca, d’élec ou de dev web, j’ai proposé un fil rouge commun : **concevoir, fabriquer et programmer un robot bipède personnalisable**, pour explorer toutes ces compétences de manière intégrée et ludique.

---

### Le robot OTTO original

![Otto-original](/img/portfolio/OTTO-MKS/Otto.png)

Le robot OTTO est un petit robot open-source très répandu dans l’éducation. Il est conçu autour d’une carte Arduino Nano, de quatre servos, d’un capteur ultrason, et de quelques composants simples. Il marche, danse, évite les obstacles, et se programme en Arduino ou via Blockly.

Il a servi de point de départ… mais **beaucoup de choses méritaient d’être améliorées** pour l’adapter à un usage pédagogique moderne.

---

### Le projet OTTO-MKS

#### Adaptation mécanique

Le design du robot a été entièrement repensé pour les besoins de l’enseignement :  
**moins de pièces, un montage rapide, et une architecture facile à modifier ou réparer.** Toutes les pièces sont modélisées sur Onshape pour permettre aux étudiant·e·s de les adapter eux-mêmes en ligne, sans installation ni prérequis.

![Otto-MKS](/img/portfolio/OTTO-MKS/Otto-MKS-EXPLODED.png)

Le robot devient un vrai support d’expérimentation : on peut l’assembler en quelques minutes, l’ouvrir, le modifier, et surtout **le comprendre.**

#### Choix électroniques

- **Microcontrôleur : XIAO ESP32-C3**  
  → Ultra compact, Wi-Fi/Bluetooth intégrés, compatible Arduino, pour moins de 5 €.
- **Alimentation : pile 9V Li-ion rechargeable en USB-C**  
  → Autonomie suffisante, recharge facile, pas besoin de piles jetables.
- **Carte électronique dédiée (design KiCad)**  
  → Organisation claire des branchements, connecteurs bien identifiés, fini les câblages erronés en TP.  
  (Et c’est très satisfaisant de concevoir son propre PCB 👌)

---

### Documentation et diffusion

Une **plateforme web** accompagne le projet et centralise toutes les ressources nécessaires :

- fichiers CAO (Onshape),
- guides de montage illustrés,
- présentation des composants,
- tutoriels de programmation (Arduino, servos, capteurs…).

En atelier, l’accès est facilité par des **QR codes** collés directement sur les boîtes et les machines. Et surtout : **la doc évolue en continu**, enrichie à chaque retour d’expérience des étudiant·e·s.

---

>#### Outils logiciels
>
>- **Onshape** (CAO collaborative)
>- **KiCad** (conception de la carte électronique)
>- **VSCode + Arduino IDE**
>- **Inkscape** (illustrations des tutoriels)

---

>#### Technologies
>
>- **Impression 3D**
>- **Électronique embarquée** (ESP32, servos, capteur)
>- **Jekyll** (interpréteur Markdown pour la documentation web)
>- **GitHub Pages** (hébergement du site web)
>- **GitHub** (code source et fichiers open-source)
