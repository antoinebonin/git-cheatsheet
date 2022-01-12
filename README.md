# Git cheatsheet

# Sommaire

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

## Git flow

### Initialiser Git Flow

```Shell
git flow init
```

### Features

#### Démarrer une feature

```Shell
git flow feature start MYFEATURE
```

#### Terminer une feature

```Shell
git flow feature finish MYFEATURE
```

### Features (collaboration)

#### Push une feature

Très utile lors de collaboration à plusieurs sur une même feature

```Shell
git flow feature publish MYFEATURE
```

#### Pull une feature

```Shell
git flow feature pull origin MYFEATURE
```

### Release

#### Démarrer une release

```Shell
git flow release start RELEASE
```

#### Push une release

Très utile lors de collaboration à plusieurs sur une même release

```Shell
git flow release publish RELEASE
```

#### Pull une release

```Shell
git flow release pull origin RELEASE
```

#### Terminer une release

```Shell
git flow release finish RELEASE
```

Ne pas oublier de push les tags après chaque livrason sur la branch principale

```
git push --tags
```

### Hotfix

#### Démarrer un hotfix

```Shell
git flow hotfix start VERSION
```

#### Push un hotfix

Très utile lors de collaboration à plusieurs sur un même hotfix

```Shell
git flow hotfix publish VERSION
```

#### Pull un hotfix

```Shell
git flow hotfix pull origin VERSION
```

#### Terminer un hotfix

```Shell
git flow hotfix finish VERSION
```

## Génération de ce cheatsheet

Pour générer ce cheatsheet, j'utilise [gh-md-toc](https://github.com/ekalinin/github-markdown-toc).
