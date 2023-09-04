## Command-Line Interface (CLI) de Go
La Command-Line Interface (CLI) de Go offre un ensemble de commandes utiles pour diverses tâches liées au développement en Go. Cette section vous présente les commandes fondamentales que vous devriez connaître pour travailler efficacement avec Go en ligne de commande.

##### go version
La commande go version affiche la version actuelle de Go installée sur votre système. Cela permet de vérifier rapidement si Go est correctement installé.

Exemple :

```bash
$ go version
go version go#####17.2 linux/amd64
```
##### go help
La commande go help affiche une liste de sous-commandes disponibles et fournit une brève description de leur utilisation. Elle est utile pour découvrir d'autres commandes Go et obtenir de l'aide sur leur utilisation.

Exemple :

```bash
$ go help


Go is a tool for managing Go source code.

Usage:

    go command [arguments]

The commands are:

    build       compile packages and dependencies
    clean       remove object files and cached files
    doc         show documentation for package or symbol
    env         print Go environment information
    fix         update packages to use new APIs
    fmt         gofmt (reformat) package sources
    generate    generate Go files by processing source
    get         download and install packages and dependencies
    install     compile and install packages and dependencies
    list        list packages or modules
    mod         module maintenance
    run         compile and run Go program
    test        test packages
    tool        run specified go tool
    version     print Go version
    vet         report likely mistakes in packages

Use "go help [command]" for more information about a command.
```

##### go run
La commande go run permet de compiler et d'exécuter un fichier Go en une seule étape. Elle est souvent utilisée pour tester rapidement des programmes Go sans avoir à générer un exécutable séparé.

Exemple :

```bash
$ go run main.go
```

##### go build
La commande go build est utilisée pour compiler un programme Go et générer un exécutable. L'exécutable sera créé dans le même répertoire que le fichier source.

Exemple :

```bash
$ go build main.go
$ ./main
```

##### go install
La commande go install compile et installe un programme Go dans le répertoire $GOPATH/bin. Vous pouvez ensuite exécuter le programme depuis n'importe quel endroit de votre système.

Exemple :

```bash
$ go install myapp.go
$ myapp
```

##### go get
La commande go get est utilisée pour télécharger et installer des packages Go depuis des référentiels distants tels que GitHub. Elle est également utilisée pour mettre à jour des packages existants.

Exemple pour télécharger un package :

```bash
$ go get github.com/golang/example/hello
```

##### go fmt
La commande go fmt reformate le code source Go selon les conventions de formatage standard. Cela garantit que votre code est cohérent et lisible.

Exemple :

```bash
$ go fmt mycode.go
```

##### go test
La commande go test exécute les tests unitaires pour un package Go. Elle recherche les fichiers de test avec le préfixe _test.go dans le package et exécute les fonctions de test.

Exemple :

```bash
$ go test mypackage
```

Ces commandes CLI de base vous aideront à démarrer rapidement avec Go et à effectuer des tâches courantes liées au développement Go. Vous pouvez obtenir plus d'informations sur chaque commande en utilisant go help [commande].