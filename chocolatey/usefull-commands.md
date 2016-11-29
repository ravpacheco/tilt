# Usefull commands with chocolatey

## How to list only a local chocolatey packages

```shel
chocolatey list -localonly
chocolatey list -lo
clist -lo
```

## How to know if you have some package to be updated

```shel
choco outdated
```

## How to upgrade some (or all) package(s)

```shel
choco upgrade <package-name>
cup <package-name>
```

* For all packages

```shel
cup all
```
