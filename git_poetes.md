# Git et GitHub pour les poètes 

1.1: [Introduction](#git)

1.2: [Branches](#branche)

1.3- [Forks and Pull Requests](#fork)

1.4- [GitHub Issues](#issues)

# 1.1: Introduction - Git et GitHub pour les poètes <a name="git"></a>

https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV

Pourquoi Git et GitHub ?
. Version control 
. Collaboration

Git
Version control software 

GitHub
web service

**Repository**
Créer un compte sur Github
Créer un dépot 
Créer un new file de nom poemes.txt

**Commit new file**  ( Commit directly to the main branch)
Le poeme est dans le dépot. 

**Commmit change**
Cliquer sur poeme.txt
Il manque la couleur verte.
Cliquer sur le crayon --> Edit this file
Remplir en bas "Commit change" par "j'ai ajouté la couleur verte" puis cliquer sur "Commit changes"

Il manque la couleur jaune.
Cliquer sur le crayon --> Edit this file
Remplir en bas "Commit change" par "j'ai ajouté la couleur jaune" puis cliquer sur "Commit changes"

**Bilan :**
Création d'un dépot.
Plusieurs commit

Nous allons pouvoir voir l'historique
Cliquer sur **History** pour voir l'historique.
En cliquant sur un des commit, on peut voir ce qui a été modifié (solugné, biffer)
On voit aussi "commit d8f911b0c32226239ff7bb95e40306014b6386be" commit hash meaning, identifiant unique du commit
On le voit aussi dans l'URL https://github.com/Charles-depot/rainbow/commit/d8f911b0c32226239ff7bb95e40306014b6386be

# 1.2: Branches - Git and GitHub for Poets <a name="branche"></a>

Repository Poemes

J'ai effectué des commit de façon linéaire en apportant 
des modifications. Chaque commit possède un identifiant unique.
C'est la branche "master ou main". C'est la racine de notre arbre.

Je souhaite maintenant faire des modifications mais je ne sais pas si 
je vais les garder. Je souhaite faire une expérience sur mon poème qui va
parler de licornes.
Je souhaite bifurquer (branch) à partir d'un commit en créant une nouvelle branche.

Vous pouvez toujours continuer à travailler sur la branche master.
Vous pouvez faire des commit sur la nouvelle branche.
Vous pouvez aussi faire une autre branches "fées" à partir d'un autre commit.
Etc...

Et comment peut-on fusionner (merge) tout cela.


Créer la nouvelle branche "licorne" 
Vérifier que vous êtes bien sur la branche "licorne"
Modifier le poème en ajoutant des mots.
Ensuite on a le choix :

 Commit directly to the licorne branch.
 Create a new branch for this commit and start a pull request
 
 On choisit Commit directly to the licorne branch. Et on sauvegarde.
 
 Si on switch sur la branche main, on voit le poème l'ancienne version.
 On aurait pu faire un commit à partir de la branche main mais on a choisit
 de faire un chemin différent. On a deux chemins que l'on peut travailler séparément.
 
 Maintenant si je trouve que le chemin licorne est valable et je souhaite que ce travail aille
 dans la branche "main"
 Revenir dans le dépot "rainbow" puis Insights puis Network.
 Cela permet de visualiser les différents branches.
 ![graph_network](graph_network.PNG)
 
 push : pousser (envoyer) quelque chose à quelqu'un 
 pull : tirer quelque chose	à quelqu'un
 
 pull request : prendre les changements et les tirer vers la branche master
 merge
 
 Je retourne sur la branche "main" pour voir :
 ![pull_request](pull_request.PNG)
 
 Cliquer sur le bouton : Compare & pull request
 Je suis en train de faire un pull request cad
 une requète pour fusionner les changements faits de "licorne"
 à "main".
 On peut voir les changements en bas de page.
 Cliquer sur le bouton "create pull request"
 
 Cliquer sur le bouton "Merge pull request" pour finaliser. Puis "Confirm merge"

 Revenir dans le dépot "rainbow" puis Insights puis Network.
 Cela permet de visualiser ce qui s'est passé.
 On peut voir que la branche licorne a fusionné avec la branch "main".
 ![graph_network_merge](graph_network_merge.PNG)
 
 Créer une nouvelle "poneys" à partir de main.
 Modifier le poème.
 Faire un commit

Revenir à la branche "main"
Faire un changement.
Faire un commit

Revenir dans le dépot "rainbow" puis Insights puis Network.
On peut voir les différents actions.
![graph_fin](graph_fin.PNG)


Commnent fusionner le tout.

Branche "main"
Cliquer sur le bouton : Compare & pull request
Cliquer sur le bouton "Merge pull request" pour finaliser. Puis "Confirm merge"

Revenir dans le dépot "rainbow" puis Insights puis Network.
On peut voir le résultat.
![graph_fin_2](graph_fin_2.PNG)


# 1.3- Forks and Pull Requests - Git and GitHub for Poets <a name="fork"></a>

Nous allons voir comment une autre personne et vous peuvent contribuer/collaborer
au dépot.

Deux concepts à ajouter.

Fork

une instance compléte de mon dépot sur un autre compte
On aura une exacte réplication du dépot avec les commit et les branches.
Je peux travailler sur le fork (commit, branches) sans modifier le dépot original.


Pull request

Cela signifie que par exemple si une branche de mon travail sur le fork est superbe
et que je souhaite contribuer dans le dépot original. 
Je vais envoyer ce travail dans le dépot original.
Et c'est au dépot original d'accepter ou rejeter d'où le pull request.


Actions

Aller sur charlestuteur, chercher charles-depot puis fork.
On peut le voir sur ce compte d'où provient le fork :
![fork-1](fork-1.png)

Modifier le poeme
Faire un commit en choisissant *Create a new branch for this commit and start a pull request.*
On peut aussi faire juste un commit
Ensuite faire un pull request pour ajouter à la brancher master du fork
Verifier sur Insights/Network

Créer un pull request vers charles-depot.
Et attendre la réponse.

Aller sur charles-depot et cliquer sur *Pull requests*

![fork-2](fork-2.png)

En cliquant sur la demande on peut voir les changements

![fork-3](fork-3.png)

Remplir le commentaire
Cliquer sur *Merge pull requests*

Aller sur charlestuteur pour voir la péponse.

# 1.4- GitHub Issues <a name="issues"></a>

Vous pouvez utiliser GitHub Issues pour planifier pour suivre les idées, les commentaires, les tâches 
ou les bogues et suivre votre travail.

Cliquer sur *New Issue* pour créer un nouveau problème.

Remplir les informations

Donner à votre problème un titre descriptif. Le titre doit indiquer en un coup d'œil de quoi il s'agit.
Ajoutez une description qui explique le but du problème, y compris tous les détails qui pourraient aider à résoudre le problème. 

Vous pouvez utiliser Markdown pour ajouter une mise en forme, des liens, des emojis, etc. 
Pour plus d'informations, consultez [« Écrire sur GitHub »](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

**Ajouter une liste de tâches.**
- [] #50
- [] faire les modifications

**Ajouter des étiquettes (labels)**
Ajouter une étiquette pour catégoriser votre problème. 
GitHub fournit des étiquettes par défaut.

Vous pouvez utiliser ces libellés par défaut ou créer les votres.

Cliquer sur *issues* puis *Labels* puis *New label*.
Donner un nom, une description et une couleur.
[Etiquettes](https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/managing-labels)

**Associer les issues au commit ou au pull request ?**
Créer un commit et associer dans le titre le numéro de l'issue comme  ... per #8 
On crée un commit particulier à cette issue.
En revenant sur les issues :
Charles-depot added a commit that referenced this issue 1 minute ago

![issues1](issues.PNG)
On peut cliquer sur commit lié per #8 pour suivre les changements.

Je peux ensuite clore l'issue. 

ou directement dans le commit en écrivant dans le titre fixes #8

On peut faire une issue à partir d'un commit.

commit 21f9ba806f57fd947586de3517a469fe41af2157

![issues](issues2.PNG)

## Bilan
référence au numéro de l'issue
référence à l'identifiant d'un commit ou description de l'issue.

