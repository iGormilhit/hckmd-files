---
title: Un bibliothécaire se connecte en tant que professionnel 
tags: rero-ils, scenario
---

## Intervenants

* Charbonnet, Virgile: bibliothécaire standard
* Müller, Astrid: bibliothécaire système
* Système: RERO ILS

## Résumé

Ce scénario décrit la façon dont l'utilisateur professionnel est identifié sur le système RERO ILS. Il s'agit de trouver ce qui se passe.

## Étapes

* Connexion à RERO ILS via le menu *Se connecter*, depuis n'importe quelle page de l'instance RERO ILS.
    - En cas d'un accès direct à une page protégée, Virgile est redirigé automatiquement sur le formulaire de login.
* Le système RERO ILS connecte Virgile à sa bibliothèque.
    - Si Virgile travaille dans plusieurs bibliothèques:
        - La première fois il est connecté à la première bibliothèque de ses affiliations.
        - Les fois suivantes il est connecté à la dernière bibliothèque à laquelle il a été connecté.
        - Il peut ensuite basculer d'une bibliothèque à l'autre au moyen d'un menu.
    * Astrid peut basculer vers n'importe quelle bibliothèque de son organisation.
        - Si Astrid travaille dans plusieurs organisations, l'organisation dans laquelle elle agit est définie par la bibliothèque active.
* Le système doit prendre en compte la bibliothèque à laquelle Virgile est connecté pour adapter l'interface (fonctionnalités et données accessibles).
* Virgile se retrouve sur la page de son point d'entrée.
- La bibliothèque active est indiquée d'une manière ou d'une autre sur l'interface.

## Questions

* Faut-il afficher le nom de la bibliothèque connectée sur tous les écrans ou uniquement dans l'interface d'administration ?
    - Oui. L'information est indiquée dans le scénario.
* Faut-il avoir un profil pour un bibliothécaire (standard et système) lui permettant de déterminer sa bibliothèque par défaut lors de la connexion ?
    - Non.