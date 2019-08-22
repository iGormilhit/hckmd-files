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

A) Vérification de la présence dans RERO ILS
* Recherche par ISBN dans tous les documents RERO ILS
	* Si document présent > voir C
* Recherche par mots de l'auteur et du titre dans tous les documents RERO ILS
	* Si document présent > voir C
* Applique B1, B2, B3, B4 selon préférence et résultats des recherches précédentes

B1) Import d'une base externe
* Recherche par ISBN dans bases externes
	* Si document absent > applique B2, B3, B4 selon préférence et résultats des recherches précédentes
* Importe le document, parmi les records disponibles, qui convient le mieux aux règles de description de sa bibliothèque
* [Système] Ouvre le document pour édition dans RERO ILS
* Vérifie les liens aux autorités, valide et sauve le document
* voir C

B2) Création à partir d'un formulaire vide
* Crée une nouveau document
* [Système] Ouvre un formulaire vierge pour édition
* Complète les données
* Ajoute les liens aux autorités, valide et sauve le document
* voir C

B3) Création par duplification
* Sélectionne un document proche de celui à décrire (même collection ou même auteur par exemple)
* Copie le document
* [Système] Ouvre une copie du document pour édition
* Vérifie les liens aux autorités, valide et sauve le document
* voir C

B4) Création à partir d'une oeuvre pré-existante
* Recherche par mots de l'auteur et du titre dans toutes les oeuvres RERO ILS
* Sélectionne l'oeuvre correspondante à son document
* Ajoute un document à cette oeuvre
* [Système] Ouvre le nouveau document pour édition, avec champs préremplis de l'oeuvre
* Complète les données manquantes
* Vérifie les liens aux autorités, valide et sauve le document
* voir C

C) Raccrochage
* Depuis la vue détaillée du document, ajoute un exemplaire
* Complète les données de l'exemplaire et sauve
* [Système] Affiche la vue détaillée du document avec la liste de ses exemplaires

## Questions soulevées

* Vue admin: dans la recherche de document, les résultats seront par défaut filtrés avec l'organisation du bibliothécaire connecté?
	* Si oui, il serait intéressant d'avoir
		* un bouton "Etendre la recherche à tout RERO ILS".
		* une option permettant de rechercher directement dans tout RERO ILS
	* Si non, il serait intéressant d'avoir un bouton permettant au préalable de restreindre la recherche à son organisation, voire à sa bibliothèque
* Notices masquées: certaines notices peuvent être masquées sur volonté du catalogueur:
	* en cours de création (brouillon/draft)
	* en cours d'acquisition
	* en cours de suppression
	* etc.
* Zones locales: les zones locales peuvent être traitées par une ressource liée au document, et appartenant à une organisation ou à une bibliothèque

Les notices privées ne représentent pas un problème, étant donné qu'il s'agit plutôt d'un type de document (cf. [documentation RERO](https://www.rero.ch/page.php?section=aacr2&pageid=chap_16))