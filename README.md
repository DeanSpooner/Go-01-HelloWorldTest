# Go 01

## How to run code

Go needs a `.go` file to start. In the terminal, navigate to the folder and run

    go run main.go

## Go terminal commands

Other CLI commands for Go exist:

- go build: compiles a bunch of Go source code files;

- go run: compiles and executes one or two files;

- go fmt: formats all the code in each file in the current directory;

- go install: compiles and "installs" a package;

- go get: downloads the raw source code of someone else's package;

- go test: runs any tests associated with the current project.

## What does "package main" mean?

A package is a collection of files, like a module or project. At the start of each file, if it is part of "package main", the first line should be `package main`.

### Types of Packages

- Executable: generates a file that we can run;
- Reusable: code used as 'helpers'; a good place to put reusable logic.
  The name `main` is used to build an executable file: any other name will **NOT** generate an executable file. So the word `main` is used very often in Go!

### Executable package

`package main` => defines a package that can be compiled and then executed. **Also, it must have a func called 'main' within the file.**

### Reusable package

`package calculator, package uploader etc.` => defines a package that can be used as a dependency (helper code).

## What does 'import fmt' mean?

`import "fmt"`: give the current package all the library files from the package "fmt". Like importing pre-made methods and functionality in JavaScript, Python etc., except they need to be explicitly imported. Other standard Go library packages that could be imported included `debug, math, encoding, crypto, io` as well as packages from other developers.

## func main()

`func` is short for function, just like in Python and JavaScript. `func` keyword, followed by its name, then an argument list.

`func main (list of arguments to pass the function) { function body, that will run when the function is called }`

## main.go file organisation

    package.main

    import "fmt"

    func main() {
    fmt.Println("Hello world!")
    }
