---
title: Scenarii, liste des questions
tags: rero-ils, scenario, questions
---

## Questions

### Résolues

Q1. Faut-il afficher le nom de la bibliothèque connectée sur tous les écrans ou
   uniquement dans l'interface d'administration ?    
A1. Oui. L'information est indiquée dans le scénario *Un bibliothécaire se
   connecte en tant que professionnel*.

Q2. Faut-il avoir un profil pour un bibliothécaire (standard et système) lui
   permettant de déterminer sa bibliothèque par défaut lors de la connexion ?    
A2. Non.

### Non encore résolues

Q3. Faut-il une interface professionnelle, pour la recherche et l'affichage des vues détaillées ?    
    C'est une question qui se pose dans le cas du catalogage (chercher une
    notices existantes à laquelle se racrocher ou pour la dupliquer), mais
    aussi pour la recherche de document, la possibilité d'éditer un
    enregistrement que le bibliothécaire consulte.
    
Une vue admin dédiée permettrait par exemple:
* un affichage plus condensé ou plus détaillé (imagettes, vue JSON/MARC...)
* des facettes différentes (données de gestion)
* des boutons d'actions "admin"
    * sur un document (éditer, supprimer, dupliquer...)
    * sur une holding (éditer, recevoir un fascicule...)
    * sur un exemplaire (ajouter, demander pour un lecteur, suivi du transit...)
* affichage des notices masquées

Q4. Si il existe une interface professionnelle pour la recherche de documents,
    est-elle par défaut filtrée à l'organisation du bibliothécaire connecté ?    
    Selon la réponse à cette question, comment le bibliothécaire doit-il étendre ou restreindre sa recherche ?
    
Possibilités:
* A priori: un "toggle button" (ON/OFF) à côté de la barre de recherche
* A posteriori:
    * option d'élargir les résultats affichés à tout RERO ILS
    * option de restreindre les résultats affichés à son organisation

Q5. Si la recherche professionnelle existe, fonctionne-t-elle avec un seul
    champ de recherche ou avec un masque de recherche de type recherche avancée ?

Q6. Faut-il avoir des interfaces de recherches dédiées à certaines actions
   (catalogage, circulation) ?    
   Par exemple, selon que l'on cherche une manifestation, une œuvre ou
   autorité, faut-il une interface spécifique ?    

* Catalogage: recherche dans tous RERO ILS (et au-delà) pour raccrochage
* Prêt: recherche d'abord dans organisation/bibliothèque
* Types d'entités: il s'agit déjà de recherche avancée


Q7. Après création, modification, ou raccrochage à une ressource bibliographique
    (œuvre, manifestation, exemplaire, autorité), où faut-il rediriger le
    bibliothécaire ?    

* Cf. [issue 376](https://github.com/rero/rero-ils/issues/376

Q8. Du point de vue des notices bibliographiques, est-ce que des zones locales
    sont nécessaire, où est-ce que le niveau des holdings suffit ?    
    Selon la réponse à la question, d'autres scénarios pourront être rédigés.


## Missing scenarii

1. Le bibliothécaire voudrait momentanément interrompre l'édition d'une notice
   et la retrouver plus tard.
1. Le bibliothécaire ajoute une notice d'acquisition, sommaire, pour des
       raisons de gestions et ne désire pas que celle-ci soit visible par les
       lecteurs.
1. Lors du catalogage, un bibliothécaire veut importer une notice depuis un
   réservoir externe.
1. Un bibliothécaire veut créer un *template* pour le catalogage, le sauver et
   l'utiliser plus tard.
1. Le bibliothécaire cherche un exemplaire pour un patron, mais à la fois dans
   les exemplaires physiques et dans les exemplaires numériques.
1. Le professionnel désire *bookmarker* des accès rapide à des recherches
   spécifiques, par exemple dans telle vue, avec tel filtre déjà ajouté, par
   exemple dans le libre accès où il travaille le plus souvent.
1. Le bibliothécaire recherche un exemplaire pour un patron, mais il n'en
   trouve pas de disponible :
   - Il fait une demande sur un exemplaire emprunté.
   - Il fait une demande de PEB.
   - Il fait une suggestion d'achat.
