# TP Git – DevOps

## Installation de Git
```bash
winget install --id Git.Git -e --source winget
```

## Documentation utilisée
- https://git-scm.com/doc
- https://docs.github.com/en/authentication/connecting-to-github-with-ssh

## Commandes Git réalisées

| Commande | Description |
|---|---|
| git config --global user.name | Définit le nom global Git |
| git config --global user.email | Définit l’email global Git |
| ssh-keygen -t ed25519 -C "mail" | Génère une clé SSH |
| ssh -T git@github.com | Teste l’authentification SSH |
| git init | Initialise un dépôt Git |
| git branch -M main | Définit la branche principale |
| git checkout -b develop | Crée et bascule sur la branche develop |
| git add . | Ajoute les fichiers à l’index |
| git commit -m "message" | Crée un commit |
| git push -u origin <branch> | Envoie les commits vers GitHub |
| git merge develop | Fusionne develop dans main |

## Diagramme du flow de commit

```
main
 └── develop
      ├── commit (création fichiers)
      ├── commit (README + modifications)
      └── merge → main
```
