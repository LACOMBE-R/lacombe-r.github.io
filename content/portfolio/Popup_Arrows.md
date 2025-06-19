+++
draft = false
image = "img/portfolio/Popup_Arrows/ARROW_BASE.jpg"
date = "2025-02-15T00:00:00+02:00"
title = "Flèches à apparition – dispositif scénique"
weight = 3
+++

Développement d’un ensemble de flèches à apparition, pour une illusion scénique dans une comédie musicale.
<!--more-->

---

## Présentation

Dans le cadre d'une consultation sur une comédie musicale, j'ai été sollicité par les **French Twins**, un duo de magiciens, pour la conception d'un ensemble de **bases mécaniques** permettant l'**apparition de flèches** sur scène.

Dans la **mise en scène**, ces flèches apparaissent après le **tir d'une volée de flèches** dans un **contenu vidéo** à l’arrière de la scène, donnant l’illusion qu’elles viennent se **planter physiquement** en avant-scène.

Chaque flèche est montée sur une base indépendante, activée via un **hub de contrôle DMX**, permettant une synchronisation précise avec les effets lumière.


---

## Conception mécanique

Les **bases de flèches** sont imprimées en 3D (PETG) et intègrent :

- un **ressort de torsion**,
- un **axe de rotation** avec une **pièce pivotante interchangeable**
- un **loquet coulissant** maintenu par un **solénoïde 12V**

---

#### **Premier test du mécanisme**

{{< video src="/img/portfolio/Popup_Arrows/FIRST_TEST.mp4" title="Premiers tests du mécanisme" no-sound="true">}}  

---
  
Les flèches, achetées dans le commerce et modifiées, s’insèrent dans la base par une **rotation d’un quart de tour**, qui verrouille mécaniquement leur position. Une fois abaissées, elles sont maintenues en tension jusqu’au déclenchement électrique. Un **loqueteau à bille réglable** permet d’atténuer le rebond lors de l’éjection.

{{< video src="/img/portfolio/Popup_Arrows/Rotate_Lock.mp4" title="Verouillage de la flèche" no-sound="true">}}  

Les flèches sont surmontées **d’ailerons imprimés en plastique flexible blanc (TPU)**, pour une plus grande durabilité et impact visuel que des plumes réelles.

---

{{< video src="/img/portfolio/Popup_Arrows/fins.mp4" title="Ailerons en TPU" no-sound="true">}}  

{{< video src="/img/portfolio/Popup_Arrows/Arrow_Base_Show.mp4" title="Ailerons en TPU" no-sound="true">}}  

---

## Connectique et modularité

Les bases sont alimentées via des **fiches audio standard**, offrant une **grande souplesse de longueur** et un **montage rapide** sur scène. Ce choix garantit une connectique robuste, détachable, et facilement remplaçable.

![Câblage des bases avec fiches audio](/img/portfolio/Popup_Arrows/Audio_Connector.png)

<img src="{{ $resized.RelPermalink }}" alt="Câblage des bases avec fiches audio">



Chaque base peut être installée indépendamment, avec une longueur de câble adaptée à son emplacement.

---

## Contrôle par DMX

Un **hub de contrôle** dédié (similaire a un switchpack) permet de piloter jusqu’à **12 bases** via **DMX512**. Une valeur supérieure à 127 sur un canal envoie une impulsion 12V à la base concernée.

J'ai utilisé pour cela une carte électronique du commerce ainsi qu'une alimentation 12V 30A.

![DMX Board](/img/portfolio/Popup_Arrows/DMX_Board.png)

Le hub est configuré par **DIP switches** pour définir l’adresse de départ, les sorties suivantes étant affectées automatiquement aux canaux consécutifs.

Le tout est integré dans un boitier composé de pièces imprimées et de carters découpés et gravés au laser. Une LED orange signale chaque déclenchement actif.

![Vues DMX Hub](/img/portfolio/Popup_Arrows/DMX_Hub_2.png)
---

## Intégration scénique

Les bases sont conçues pour être **dissimulées** en position couchée dans un **coffrage scénique frontal**. Lors du déclenchement, les flèches surgissent verticalement, créant l'effet d'une apparition.

![Coffrage](/img/portfolio/Popup_Arrows/Coffrage.jpg)

## Effet

{{< video src="/img/portfolio/Popup_Arrows/DEMO.mp4" title="Demo" no-sound="true">}}

---

>#### Technologies utilisées
>
>- **Impression 3D**  
>- **Découpe Laser**  
>- **Contrôle DMX512**

---

>#### Outils logiciels
>
>- **Onshape** (CAO des bases)
>- **Chataigne** (Tests et développement)

---