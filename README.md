# Détecteur des émotions par les expressions faciales

Un détecteur des émotions permet de détecter et d’analyser les émotions capturées à un instant t à partir d’une simple photo où une vidéo. Ce service peut identifier jusqu’à 7 émotions : la colère, le dégoût, la peur, le bonheur, neutre, la tristesse et la surprise. 
On va construire un modèle IA qui permet de réaliser cette tâche sur des images et des vidéos.

### Contexte du projet

Les expressions du visage peuvent naturellement servirent à évaluer la satisfaction d’un client aux prises avec un service après-vente ou à face à un produit récemment acquis dont il 
s’agit de comprendre le fonctionnement. On peut encore mentionner les applications suivantes :

La détection d’un manque d’attention chez un conducteur en vue d’augmenter la sécurité de la conduite.
L’évaluation du niveau de stress de passagers à l’atterrissage ou à l’arrivé en gare ou la détection de comportements suspects.
L’humanisation des robots dans leurs interactions avec les humains dont ils prendraient en compte l’état psychique.

Les expressions faciales humaines peuvent être facilement classées en 7 émotions de base: heureuse, triste, surprise, peur, colère, dégoût et neutre. 
Nos émotions faciales sont exprimées par l'activation d'ensembles spécifiques de muscles faciaux. Ces signaux parfois subtils, mais complexes, dans une expression contiennent 
souvent une quantité abondante d'informations sur notre état d'esprit. Grâce à la reconnaissance des émotions faciales, nous sommes en mesure de mesurer les effets du contenu et 
des services sur le public / les utilisateurs grâce à une procédure simple et peu coûteuse. Par exemple, les détaillants peuvent utiliser ces mesures pour évaluer l'intérêt des clients. Les prestataires de soins de santé peuvent fournir un meilleur service en utilisant des informations supplémentaires sur l'état émotionnel des patients pendant le traitement. Les producteurs de divertissement peuvent surveiller l'engagement du public dans les événements pour créer de manière cohérente le contenu souhaité.

Les émojis ou avatars sont des moyens d'indiquer des signaux non verbaux. Ces indices sont devenus une partie essentielle du chat en ligne, de l'examen des produits, de l'émotion de la 
marque et bien d'autres. Cela a également conduit à une augmentation de la recherche en science des données dédiée à la narration basée sur les emojis.

Grâce aux progrès de la vision par ordinateur et de l'apprentissage en profondeur, il est désormais possible de détecter les émotions humaines à partir d'images. 
Dans ce projet d'apprentissage en profondeur, nous classerons les expressions faciales humaines pour filtrer et mapper les emojis ou avatars correspondants.

L'ensemble de données reconnaissance des expressions faciales se compose d'images de visage en niveaux de gris de 48 * 48 pixels. Les images sont centrées et occupent un espace égal. 
Cet ensemble de données comprend les émotions faciales des catégories suivantes:

* 0: colère
* 1: dégoût
* 2: peur
* 3: heureux
* 4: neutre
* 5: triste
* 6: surpris

Nous allons créer un modèle d'apprentissage en profondeur pour classer les expressions faciales à partir des images. 
Ensuite, nous mapperons l'émotion classée à un emoji ou un avatar.

Par conséquent, on va construire une architecture de réseau de neurones à convolution et on va entraîner le modèle sur l'ensemble de données pour la reconnaissance d'émotion à 
partir d'images.

Après compilation et entraînement du modèle, On obtient une accuracy de notre modèle de 87%, ce qui est un résultat plutôt bon.

Notre modèle sera sauvegardé afin de pouvoir être utilisé sans l'interface graphique.

On utilise pour celà, openCV haarcascade xml, afin de définir les boîtes englobantes du visage dans la webcam et on prédit les émotions.

L'interface graphique nous permet de détecter instantanément l'émotion de la personne sur la webcam et de lui associer l'émotion et l'émoji correspondant.
[resultat_interface](https://github.com/celine29730/D-tecteur-des-motions-par-les-expressions-faciales/blob/main/imageinterface.png)




