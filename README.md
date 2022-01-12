# Git cheatsheet

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
