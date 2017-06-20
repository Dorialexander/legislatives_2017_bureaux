# legislatives_2017_bureaux
Résultat par bureaux de vote des élections législatives françaises de 2017 (premier tour)

Les données proviennent de data.gouv.fr (licence ouverte) : https://www.data.gouv.fr/fr/datasets/elections-legislatives-des-11-et-18-juin-2017-resultats-par-bureaux-de-vote-du-1er-tour/

Elles étaient présentées dans un format "large" et libre. Pour chaque bureau de vote (représentant une ligne), les résultats de chaque candidats sont listés continuellement (ce qui ne permet pas de les trier).

En accord avec les principes des "données bien rangées" ("tidy data") d'Hadley Wickam, j'ai opté pour un format "long". 

Pour avoir des fichiers plus légers et manipulables, j'ai  dissocié les métadonnées propre à chaque bureau de vote des résultats proprement dit. Il est toujours possible de les joindre a posteriori sur l'identifiant du bureau, "bureau_id".

L'indication du numéro du bureau de vote était apparemment problématique dans certaines circonscriptions : des communes différentes, parfois en grand nombre, portaient le même numéro (0001). Pour définir l'identifiant du bureau de vote, j'ai intégré également le numéro de la commune (séparé par un tiret).
