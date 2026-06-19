+++
draft = false
image = "portfolio/opentallyesp32/icon.jpg"
date = "2025-12-01T00:00:00+01:00"
title = "OpenTallyEsp32"
weight = 2
+++

Boîtiers lumineux sans fil pour indiquer aux caméramans si leur caméra est en direct conçus et fabriqués pour un événement esport live.

<!--more-->

---

{{< mediagrid src="side.jpg" alt="Boîtier OpenTally" >}}

## Contexte

En production télévisée ou vidéo, un **tally** est un indicateur lumineux fixé sur une caméra : rouge quand elle est à l'antenne, vert quand elle est en prévisualisation. C'est le moyen pour un caméraman de savoir, sans communication radio, si son image est diffusée en direct.

La **[LCE](https://lce.gg/)** est le championnat esport organisé par l'**[association orKs](https://www.orks.fr)**, une structure basée à Poitiers qui fédère plusieurs clubs et équipes compétitives. Les finales sont produites comme un véritable événement télévisé : plateau, régie, caméramans, commentateurs, diffusion en direct.

Pour cette production, l'équipe technique d'orKs avait déjà mis en place un **serveur WebSocket**, gérant, entre autre, l'état de chaque caméra en temps réel depuis la régie. Il manquait l'autre bout de la chaîne : des boîtiers physiques, sans fil capables de s'y connecter et d'afficher l'état sur des leds.

{{< github-card repo="LACOMBE-R/OpenTallyESP32" >}}
---

## Le boîtier

Chaque unité se monte sur l'attache griffe d'une caméra et communique en Wi-Fi avec un serveur central. Deux LEDs à l'arrière sont visibles par le caméraman, une troisième à l'avant est tournée vers le sujet filmé.

{{< mediagrid src="Front_Back.jpg" alt="Face avant et arrière" >}}

L'électronique repose sur un **XIAO ESP32-C3**, choisi pour sa taille compacte et son Wi-Fi intégré. J'ai conçu un **PCB dédié sous KiCad** pour loger l'ensemble proprement, avec une lecture de tension batterie et un bouton multifonction.

{{< kicanvas src="https://raw.githubusercontent.com/LACOMBE-R/OpenTallyESP32/main/ECAD/OpenTallyESP32/OpenTallyESP32.kicad_pcb" src2="https://raw.githubusercontent.com/LACOMBE-R/OpenTallyESP32/main/ECAD/OpenTallyESP32/OpenTallyESP32.kicad_sch" controls="full" >}}


J'ai fabriqué ce circuit grâce a un Laser Fibre Xtool F2 Ultra.

{{< mediagrid src="CUT.gif" alt="Gravure laser" src2="PCB_Off_Side.jpg" alt2="PCB" >}}

---

## Ce qui se passe sous le capot

Les boîtiers communiquent avec un serveur via **WebSocket** : chaque unité s'abonne à une caméra et reçoit ses mises à jour en temps réel.

Pour l'autonomie, le CPU est bridé dès la connexion établie, et un appui sur le bouton plonge l'unité en **deep sleep**. La tension batterie est remontée automatiquement au serveur toutes les 30 secondes.

La configuration se fait sans toucher au code : un appui long au démarrage crée un point d'accès Wi-Fi et ouvre une **interface web** pour renseigner le réseau, le serveur et l'identifiant de caméra. Tout est sauvegardé en flash.

---

>### Outils logiciels
>
>- **[KiCad](https://www.kicad.org)**
>- **[PlatformIO](https://platformio.org)**
>- **VSCode**

---

>### Technologies
>
>- **Programmation embarquée (C++ / Arduino)**
>- **Conception de PCB**
>- **WebSocket / Wi-Fi**
