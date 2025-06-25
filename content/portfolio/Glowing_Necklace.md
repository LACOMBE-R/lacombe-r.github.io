+++
draft = false
image = "img/portfolio/Glowing_Necklace/Icon.gif"
date = "2025-02-15T00:00:00+01:00"
title = "Collier lumineux pour la scène"
weight = 10
+++

Accessoire lumineux conçu sur mesure pour la scène, mêlant électronique embarquée, illusion et exigence d'encombrement.
<!--more-->

---

## Présentation

À la demande des **French Twins**, duo de magiciens et consultants en effets visuels, j’ai conçu un **collier lumineux interactif** pour la scénographie d’une comédie musicale. Une pierre inerte en apparence, renfermant des LED haute puissance controlées par un boitier accroché à la ceinture.

![Collier lumineux](/img/portfolio/Glowing_Necklace/necklace.jpg)

---

## Architecture technique

Le système repose sur une architecture compacte autour d’un **XIAO ESP32-C3**, un microcontrôleur miniature mais puissant, intégrant des sorties PWM et un module de charge de batterie integré.

L’ensemble est organisé autour de trois éléments :

- une **pierre en résine translucide** abritant la matrice LED,
- une **boîte de contrôle ceinture**, contenant l’électronique et la batterie,
- un **faux collier** intégrant les fils d’alimentation de manière invisible.

---

## Conception d’un PCB sur mesure

Pour répondre aux contraintes d’usage scénique (fiabilité, discrétion, compacité), j’ai conçu un **circuit imprimé dédié**, intégrant :

- Le **XIAO ESP32-C3**,
- Une **sortie PWM** vers les LEDs haute puissance,
- Un connecteur pour **bouton** déclenchant la séquence lumineuse après appui prolongé.
- Une batterie.

Le tout est pensé pour une **installation rapide et robuste** dans la boîte de ceinture, avec gestion thermique, polarité protégée et fixation mécanique des câbles.

---

## Contrôle de la séquence : firmware embarqué

Le firmware est écrit en **Arduino C++**, optimisé pour garantir une **séquence fluide** et une activation fiable dans un environnement scénique.

L’animation lumineuse est orchestrée par **une fonction de fondu progressif**, qui interpole automatiquement entre plusieurs valeurs définis dans un tableau de séquence facilement modifiable.

```cpp
// Exemple de séquence : chaque étape représente une variation d’intensité dans le temps
const AnimationStep sequence[] = {
  {20, 2.0},   // Monter à 20% sur 2 secondes
  {0, 2.0},    // Redescendre à 0% sur 2 secondes
  {50, 2.0},   // Monter à 50% sur 2 secondes
  {0, 2.0},    // Revenir à 0%
  {100, 3.0},  // Monter à 100% sur 3 secondes
  {100, 3.0},  // Rester à 100% pendant 3 secondes
  {20, 2.0},   // Descendre à 20%
  {100, 2.0},  // Rebond à 100%
  {0, 2.0}     // Retour au noir
};
```

---

## Un objet de scène sur mesure

Le collier devait non seulement s’illuminer selon une séquence précise, mais aussi **pouvoir léviter** à l’aide d’un fil quasiment invisible, fixé grâce à un **aimant intégré dans la pierre**.

L’effet scénique repose donc sur l’**illusion visuelle**, rendue possible par une **miniaturisation de l’électronique**, une **autonomie suffisante** (5 à 10 utilisations), et une **activation parfaitement contrôlée** par l’artiste sur scène.

---

## Une démarche Addastra

Ce projet incarne pleinement la démarche d’**Addastra** : concevoir des objets **à la croisée de l’art et de la technique**, en réponse à des besoins **créatifs, scéniques et sensibles**, avec un fort souci de **fiabilité en situation réelle**.

---

> #### Technologies
>
> - XIAO ESP32-C3  
> - Circuit imprimé custom  
> - Régulation et gestion d’alimentation  
> - LEDs haute puissance  
> - Recharge USB-C  

---

> #### Outils logiciels
>
> - KiCad  
> - Fusion 360  
> - VSCode / Arduino  
