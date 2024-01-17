Toujours fichier.md !

SCM :
Snapshot : 
#  Git : (2005 - Linux)
- gérer les versions
- travailler sur des fonctions différent en même temps
- sauvegardes

# Versioning :
- traçabilité
- collaboration 
- branching et merging
- backup
- majeur, mineur, correctif (2.3.1)

Commit : sauvegarder localement une version du projet (local)
Branching / Merging : pour le travail collaboratif
système distribué : téléchargement à plusieurs sources / collaborateurs (1337x / git)
système centralisé : SVN

Dif git / SCMs : ![[Capture d’écran 2024-01-15 à 10.13.13.png]]

Git : travail en local !
# Git ce charge de l'intégrité des données : 
- checksum : détecte des changements, fichiers cachés 
- impossible de modifier un fichier sans modifier la checksum !

# Peut d'opérations destructives :
- fichiers protégés 

# 3 états principaux git :

![[Capture d’écran 2024-01-15 à 10.27.04.png]]

modifier : modification d'un fichier, d'une ligne
indexé : uniquement fichiers modifié sauvegardé
validé : Aucun changement détecté

Configuration de git : 

jamais d'espace dans les nom de dossiers !!

# Commandes git :
- (~) racine répertoire utilisateur : cd ~
- (git config --global user.email marty.rabatel2@gmail.com) configurer l'email
- (i) insertion
- (esc) quitter le mode insertion
- (:) sauvegarder
- (wq) quitter
- (git config --global core.editor emacs) configurer l'éditeur de code par défaut
- (git config --global init.defaultBranch main) nom de la branch par défaut main
- (git init) initialise git dans le dossier
- (rm -rf .git/) supprimer un repo
- (git status) historique des modifications / actions
- (git diff -staged) 
- (git commit -m "message") commit les modificaitions
- (rm <fichier> --> git status --> git rm <fichier>) Effacer des fichiers
- (git rm --cached <fichier>) supprimer du tracking git
- (git log) historique des commit
- (git tag -a v1.0 -m "Version 1.0") crée un tag / version
- (git checkout -b branchname) nouvelle branche

git : logiciel local
github / gitlab : site web

# Rebase

Integrer les modifications d'une branche dans une autre :
- fusion (merge) 
- -> git checkout master
- -> git merge experiment
- rebasage (rebase) 
- -> git checkout experiemnt
- -> git rebase master

![[Capture d’écran 2024-01-17 à 09.45.49.png]]

git head --> ou on ce trouve dans le projet ?
git status --> etat du repo + branch 

exam : shema rebase deja push

npm i commitizen --> 

# Commit :
--> git add .
--> npm run commit
--> git push origin branchname
