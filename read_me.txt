Le fichier initial est uplift_project, cependant il a fallu anonymiser les données présentes dans data, a savoir, des des retour de lecteurs sur un article scientifique et dans un sous fichier RecommandationData, quel lecteur a été assigné à quel article ainsi qu'un accès aux pages google scholar des articles qu'on écrit les lecteurs.


Le code à utiliser est donc uplift_post_data qui utilise un fichier bid.csv qui contient :
1ère colonne des identifiants des lecteurs
2ème colonne 1 si le lecteur à bid 0 sinon
les autres colonnes contiennent des scores lié aux mots présents dans les titres des articles qu'ont écrit les lecteurs

Dans le dossier score des fichiers scoreX.csv avec X l'identifiant de l'article qui contient :
1ère colonne les identifiants des lecteurs
2ème colonne 1 si le lecteur est satisfait, 0 sinon

et un dossier key_word qui contient des fichiers key_wordX.txt avec X l'identifiant de l'article qui contient :
une liste de mots clefs liés à l'article

pour modifier la liste des articles traités :

modifier score
modifier key_word
dans le cas d'un ajout ou suppression d'un article, penser à modifier en conséquence la liste all_num_article présente dans la ligne 348 du code