---
title: Créer un nouveau document
tags: rero-ils, scenario
---

## Intervenants

* Virgile: bibliothécaire standard
* Système: RERO ILS

## Résumé

Virgile vient d'acheter un roman pour ado au libraire du coin pour sa bibliothèque. Il souhaite à présent la signaler dans le système. Tout d'abord, il va vérifier si elle existe déjà dans le système. Le cas échéant, il y a raccrochera un exemplaire. Sinon, il créera d'abord le document avant d'y ajouter un exemplaire.

## Étapes

* Virgile ouvre son navigateur sur la page de recherche des documents afin de déterminer si le document à rajouter existe déjà. Il peut s'y prendre de différentes manières:
    - recherche par ISBN ou autre identifiants ou par champs libres par ex. auteur titre
    - il pourra rechercher depuis l'interface de recherche des œuvres ou des auteurs
* différents cas se présentent:
    - Virgile a trouvé une manifestation
        - raccrochage depuis la vue détaillée du document: Virgile ajoute un exemplaire
        - Virgile complète les données de l'exemplaire et sauve
    - Virgile a trouvé une œuvre
        - ajoute un document à cette œuvre
        - [système] ouvre le nouveau document pour édition, avec champs préremplis de l'œuvre
        - Virgile complète les données manquantes
        - Virgile vérifie les liens aux autorités, valide et sauve le document
    - Virgile a trouvé une manifestation similaire
        - il duplique la manifestation depuis la vue détaillée
        - le [système] ouvre une copie du document pour édition
        - Virgile vérifie les liens aux autorités, valide et sauve le document
    - Virgile ne trouve aucune manifestation approchante
        - depuis le menu de l'interface, il ouvre l'éditeur vide
        - il peut importer la notice depuis une source externe
        - il remplit ou complète les informations
        - il ajoute les liens aux autorités, valide et sauve le document

## Questions soulevées

* lors de l'édition d'une ressource: raccrochage ou création où est-il redirigé dans les différents cas œuvres, manifestations, autorités
* pour rechercher si une manifestation existe, doit-on disposer d'une interface recherchant dans différentes ressources (manifestation, œuvre, autorités)?
* est-ce que Virgile va utiliser l'interface de recherche publique? Faut-il une interface admin spécifique? Va-t-il utiliser la vue détaillée publique ou en faut-il une spécifique admin?
* dans le cas d'une interface de recherche manifestations admin: les résultats seront-ils filtrés par défaut avec l'organisation du bibliothécaire connecté?
	* si oui, il serait intéressant d'avoir
		* un bouton "Étendre la recherche à tout RERO ILS"
		* une option permettant de rechercher directement dans tout RERO ILS
	* si non, il serait intéressant d'avoir un bouton permettant au préalable de restreindre la recherche à son organisation, voire à sa bibliothèque
* notices masquées pour le lecteur sur volonté du catalogueur (pour diverses
  raisons, comme brouillon, acquisition...): quelles ressources peuvent être
  masquées (œuvre, manifestation, item). Doit faire l'objet d'autres
  scénarios qui intègreraient les différentes notions de notices masquées (ou autre mécanisme).
* zones locales: les zones locales peuvent-elles être traitées par une
  ressource liée au document, et appartenant à une organisation ou à une
  bibliothèque. Est-ce que elles seront liées à l'exemplaire ou à la
  manifestation? D'autres scénarios doivent (peut-être) être écrits pour traitées les
  besoins de zones locales.
- scénarios à ajouter: importation de notices externe, création et utilisation
  de *template* de catalogage
- la recherche d'une manifestation, a-t-on un seul champ de saisie, ou une
  recherche avancée (éventuellement autre scénario)?
- [à explorer peut-être] Faut-il avoir des interfaces de recherche dédiées à
  certaines tâches (ajouter un exemplaire...)?

Note: les notices privées ne représentent pas un problème, étant donné qu'il pourrait s'agir d'un type de document (cf. [documentation RERO](https://www.rero.ch/page.php?section=aacr2&pageid=chap_16))
