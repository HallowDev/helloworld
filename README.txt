Projet HelloWorld - exercice Git avance
test

MISE EN PLACE DU HOOK pre-commit
================================
Ce depot fournit un hook git "pre-commit" dans le dossier hooks/.
Comme .git/hooks n'est pas versionne, chaque developpeur doit l'installer :

    cp hooks/pre-commit .git/hooks/pre-commit
    chmod +x .git/hooks/pre-commit

A chaque commit, le hook demande si l'on veut marquer le commit comme
verifie. Si l'on repond 'y', il cree suivi/commitInfo.txt avec la date.

Variante : git config core.hooksPath hooks   (evite la copie manuelle)
test