# Résumé de la conférence "Angular & PWA : Mon site survit à l’apocalypse !"

## Cartouche d'identification

 - Manifestation : CodeursEnSeine 2018
 - Lieu : Kindarena Rouen
 - Conférence : Angular & PWA : Mon site survit à l’apocalypse !
 - Horaire de la conférence : 14h10 - 14h30
 - Durée de la conférence : 20min
 - Conférencier(s) :
   - Cyril Lefebvre : https://www.linkedin.com/in/cyril-lefebvre-2a818294/?originalSubdomain=fr
   - Frédéric Jammes : https://www.linkedin.com/in/fr%C3%A9d%C3%A9ric-jammes-b2991331/
 - Audience : Environ 100 participants
 - Auteur du billet : François BRUN
 - Mots-clés : Angular, PWA, Application, Apocalypse, Survie, Rapide, Installable, Fiable
 - Illustration : ![](confPWA-image.jpg)

## Support
 - Lien vers le support (diapos) présenté en conférence : https://www.youtube.com/channel/UCWujmG5rANxJI0nHbMFs08w/videos
 - Nombre de diapos du support : 14
 - Plan du support :
   - Introduction
   - Mise en contexte
   - Présentation de l'architecture utilisée
   - Démonstration
   - Présentation des avantages des PWA
   - Conclusion

## Résumé

L'apocalypse est arrivée, que faire ? Les conférenciers répondent à cette question simplement : il nous faut un site web pour continuer à informer les gens et leur proposer des guides de survie ! Le cahier des charges est simple : il faut que ce site soit rapide à mettre en oeuvre et qu'il soit fiable. Ainsi, même en cas de coupure Internet, il faut que les utilisateurs puissent continuer à utiliser l'application. La solution que présente cette conférence pour répondre à ce cahier des charges : une application Angular en Progressive Web App (PWA).

Après cette introduction et mise en contexte, l'architecture est détaillée : pour la gestion des données, l'utilisation de CouchDB au niveau du backend et PouchDB côté frontend est retenue. CouchDB s'occupera de la synchronisation avec la base de données côté backend et PouchDB se connectera à CouchDB et tentera de se synchroniser régulièrement pour mettre à jour les données affichées côté frontend.

Enfin, en ce qui concerne le frontend (en Angular), celui-ci sera découpé en 3 modules : Core (le socle de l'application), Shared (contenant tous les éléments partagés entre les différents composants de notre application) et Zombie (module fonctionnel s'occupant du routing de l'application).

Une fois l'architecture présentée, une démonstration est réalisée permettant de mettre en avant les avantages de la PWA (dont notamment l'indépendance de la connexion). La conférence se termine sur la diapo présentée en illustration de ce billet, résumant les différents avantages des PWA.



## Architecture et facteur qualité

Le facteur qualité mis en évidence dans cette conférence est le facteur Reliability (fiabilité). En effet, celui-ci se définit comme la capacité d'une application à accomplir sans défaillance l'ensemble des fonctionnalités spécifiées. Or, comme présenté dans le résumé, l'avantage des PWA est qu'elles permettent à l'utilisateur d'y accéder même hors connexion. Cette indépendance de la connexion permet donc aux PWA d'être bien plus fiables que les applications classiques puisqu'elles continuent de fonctionner (sans défaillance) même lorsque l'utilisateur passe dans des zones sans connexion (tunnels, zones blanches, ...). 
