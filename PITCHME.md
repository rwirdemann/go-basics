# Go Basics

Ralf Wirdemann - Software Coaching

---

## Installation

https://golang.org/dl

```
$ go version
go version go1.11 darwin/amd64
```

---

## Workspace

```
bin/
    restvoice	
pkg/
    linux_amd64/
        github.com/rwirdemann/restvoice/
            usecase.a
src/
    github.com/rwirdemann/restvoice/
        main.go
        usecase/
            create_invoice.go 
```

---

## Workspace einrichten

```
$ cd $HOME
$ mkdir -p go/bin go/pkg go/src
$ export GOPATH=$HOME/go
```

---

## Installation testen

```
// $GOPATH/src/main.go
package main

func main() {
    println("Hello, Jo")
}

$ cd $GOPATH
$ go run main.go
```

---

## Command-Line Arguments

```
import os

var args []string = os.Args
```

---

## Exercise

Schreibe ein EUR -> Dollar Konverter. Alle als Kommandozeilenparameter übergebenen Eurowerte werden in Dollar umgerechnet und ausgegeben.

### Hints
- https://golang.org/pkg
- strconv.ParseFloat
