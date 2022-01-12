# Git cheatsheet

## Sommaire

- [Git](#git)

  - [Initiliser un repository](#initiliser-un-repository)
  - [Changement de fichier](#changement-de-fichier)
    - [Voir les fichiers différents](#voir-les-fichiers-différents)
    - [Voir les modifications dans les fichiers](#voir-les-modifications-dans-les-fichiers)
    - [Indexer des fichiers pour les commit](#indexer-des-fichiers-pour-les-commit)
    - [Commit les fichiers](#commit-les-fichiers)
  - [Branches](#branches)
    - [Liste les branches](#liste-les-branches)
    - [Créer une branche](#créer-une-branche)
    - [Naviguer sur une branche](#naviguer-sur-une-branche)
    - [Combine une autre branche dans la branche actuelle](#combine-une-autre-branche-dans-la-branche-actuelle)
    - [Supprimer une branche](#supprimer-une-branche)
  - [Syncronisation](#syncronisation)
    - [Envoie les commits en ligne](#envoie-les-commits-en-ligne)
    - [Récupère les commits distants](#récupère-les-commits-distants)

- [Git flow](#git-flow)
  - [Initialiser Git Flow](#initialiser-git-flow)
  - [Features](#features)
    - [Démarrer une feature](#démarrer-une-feature)
    - [Terminer une feature](#terminer-une-feature)
  - [Features (collaboration)](#features-collaboration)
    - [Push une feature](#push-une-feature)
    - [Pull une feature](#pull-une-feature)
  - [Release](#release)
    - [Démarrer une release](#démarrer-une-release)
    - [Push une release](#push-une-release)
    - [Pull une release](#pull-une-release)
    - [Terminer une release](#terminer-une-release)
  - [Hotfix](#hotfix)
    - [Démarrer un hotfix](#démarrer-un-hotfix)
    - [Push un hotfix](#push-un-hotfix)
    - [Pull un hotfix](#pull-un-hotfix)
    - [Terminer un hotfix](#terminer-un-hotfix)
- [Génération de ce cheatsheet](#génération-de-ce-cheatsheet)

## Git

#### Initiliser un repository

```
git init
```

### Changement de fichier

#### Voir les fichiers différents

```
git status
```

#### Voir les modifications dans les fichiers

```
git diff
```

#### Indexer des fichiers pour les commit

```
git add <fichier>
```

#### Commit les fichiers

Le paramètre `-m` peut être répété plusieurs fois.

```
git commit -m "<message>"
```

### Branches

#### Liste les branches

On peut ajouter le paramètre `-a` pour voir en plus les branches distantes.

```
git branch
```

#### Créer une branche

```
git branch <name>
```

#### Naviguer sur une branche

```
git checkout <name>
```

#### Combine une autre branche dans la branche actuelle

```
git merge <name>
```

#### Supprimer une branche

```
git branch -d <name>
```

### Syncronisation

#### Envoie les commits en ligne

```
git push
```

#### Récupère les commits distants

```
git pull
```

## Git flow

### Initialiser Git Flow

```Shell
git flow init
```

### Features

#### Démarrer une feature

```Shell
git flow feature start <name>
```

#### Terminer une feature

```Shell
git flow feature finish <name>
```

### Features (collaboration)

#### Push une feature

Très utile lors de collaboration à plusieurs sur une même feature

```Shell
git flow feature publish <name>
```

#### Pull une feature

```Shell
git flow feature pull origin <name>
```

### Release

#### Démarrer une release

```Shell
git flow release start <name>
```

#### Push une release

Très utile lors de collaboration à plusieurs sur une même release

```Shell
git flow release publish <name>
```

#### Pull une release

```Shell
git flow release pull origin <name>
```

#### Terminer une release

```Shell
git flow release finish <name>
```

Ne pas oublier de push les tags après chaque livrason sur la branch principale

```
git push --tags
```

### Hotfix

#### Démarrer un hotfix

```Shell
git flow hotfix start <name>
```

#### Push un hotfix

Très utile lors de collaboration à plusieurs sur un même hotfix

```Shell
git flow hotfix publish <name>
```

#### Pull un hotfix

```Shell
git flow hotfix pull origin <name>
```

#### Terminer un hotfix

```Shell
git flow hotfix finish <name>
```

## Génération de ce cheatsheet

Pour générer ce cheatsheet, j'utilise [gh-md-toc](https://github.com/ekalinin/github-markdown-toc).
