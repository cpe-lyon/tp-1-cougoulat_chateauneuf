# Compte-rendu Administration Linux : TP1

# Groupe :
- Aymrick COUGOULAT
- Grégoire CHATEAUNEUF

# Exercice 1

Installation d'Ubuntu en suivant les informations indiqué sur le TP

# Exercice 2

- # Manuel

1) Pour trouver l'utilité du "which", on tape la commande "man which" ( "man" permettant d'accéder au manuel ). La commande "which" permet de renvoyer le chemin des/du fichiers indiqué à la suite de la commande.
	which [-a] nom_fichier

2) Pour accéder à une certaine catégorie de la documentation d'une commande. Il faut taper ( dans le manuel ) : /nom_catégorie (ex: /option )

3) Pour quitter le manuel, il faut appuyer qur la touche "q"

4) Pour accéder à la première page de la section 6, il faut taper la commande suivante : "man 6 intro". Intro est la première de la section. Cette section parle des jeux et petits programmes marrants disponible sur le système.

- # Navigation dans l'arborescence des fichiers

1) Pour accéder au dossier /var/log, on doit tapper la commande : cd var/log

2) Pour revenir dans le dossier /var en utilisant un chemin relatif, il faut tapper la commande "cd .."

3) Pour aller dans le dossier personnel ( Home ), il faut tapper : "cd /home"

4) Pour aller dans le dossier précedent sans utiliser de chemin, il faut taper la commande : "cd -"

5) En tapant la commande "/root", la console nous indique que nous n'avons pas l'autorisation d'accèder à ce chemin.

6) En tapant la commande "sudo cd /root", nous devons indiquer le mot de passe du serveur que nous avons configuré pendant l'installation.
Mais il est impossible ( même en indiquant le bon mot de passe ) d'accéder au chemin "/root".

7) Pour créer un dossier, il faut taper la commande "sudo mkdir nom_dossier".
   Pour créer un fichier, il faut taper la commande "sudo touch nom_fichier".
   ( Attention, il faut bien penser à mettre sudo avant la commande pour avoir la permission de créer un nouveau dossier.

8) Pour supprimer Fichier1 depuis le dossier personnel : "sudo rm Dossier1/Fichier1"
   Pour supprimer Dossier1, on ne peut pas utiliser rm puisque c'est un dossier. 

9) Pour suprimer un dossier vide (Dossier1), on utilise: "sudo rmdir Dossier1"

10) Quand on esssaie de supprimer Dossier2 avec rmdir et/ou rm, cela ne fonctionne pas car le Dossier2 n'est pas vide.

11) Pour supprimer le dossier avec son contenu : "sudo rm -r Dossier2"

- # Commandes importantes

1) Pour afficher l'heure et la date du jour: "date"
   La commande "time" permet de chronometrer le temps d'action d'une commande.

2) "ls" permet d'afficher les dossiers existants, "la" permet d'afficher les dossiers cachées.

3) Pour trouver la loalisation du programme "ls" : "which ls"

4) La commande ll existe et affiche des informations sur les dossiers existants. Mais il n'existe aucune documentation dans le manuel sur "ll".
"alias ll" permet de trouver le "vrai nom" pour chercher ensuite dans la documentation.

5) Pour afficher les fichiers du dossier /bin : "ls /bin"

6) "ls .." permet d'afficher les dossiers/fichiers du dossier un cran avant de celui ou l'on se trouve. ( Ex: on est dans le dossier personnel, en  tapant la commande ls .., on affiche les dossiers/fichiers de /home )

7) Pour afficher le chemin complet du dossier ou l'on se situe: "pwd"

8) "echo 'yo' > plop": On obtient un fichier nommé plop avec 'yo' écrit dans ce fichier. La deuxième commande ne fait que remplacer.

9) "echo 'yo' >> plop": On obtient un fichier nommé plop avec écrit : 'yo yo' écrit dans ce fichier. La deuxième commande ajoute une ligne.

10) La commande file permet de déterminé le type d'un fichier. Par exemple, "file plop", cette commande nous retourne : "plop: ASCII text".

11) On peut remarquer que titi a récupéré ce que nous avons modifié dans le fichier toto. En supprimant toto, le fichier titi est resté tel qu'il l'était.

12) Un lien symbolique réagit dans les deux sens. En modifiant titi, tutu se retrouve modifié. En modifiant tutu, titi est modifié. Pareil quand on supprime titi, tutu est alors supprimé.

13) CTRL + S pour couper le défilement
    CTRL + Q pour reprendre le défilement

14) Pour afficher les 5 premières lignes d'un fichier : head -5 nom_fichier
    Pour afficher les 20 dernières lignes d'un fichier : tail -20 nom_fichier	
    Pour afficher les lignes 10 à 20: head -20 nom_ficher | tile -10

15) La commande permet d'afficher les informations du noyeau

16) Ce fichier affiche les informations d'ou se trouve les informations d'identifications pour chaque module.

17) 

18) Pour trouver le nombre d'utilisateur sur la machine, il faut taper la commande suivante : "who"

19) 

20) Pour trouver tous les fichiers se nommant passwd sur la machine, il faut utiliser la commande : "find / -name passwd"

21)

22) Pour trouver le vrai nom de l'alias 11, il faut taper la commande "alias 11". On réutilise donc ce nom pour trouver ou il est défini dans notre dossier personnel grâce à la commande : "grep 'nom_alias_11' /home".

23) L'utilisation de "locate" pour trouver un fichier est simple, il suffit simplement de taper : "locate 'nom_fichier'". Dans notre case donc pour trouver le fichier le fichier "history.log" on tape la commande : "locate history.log".

24)

# Exercice 4


3)

4)
