# Hello World

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello World")
}
```

* This is a simple `Hello World` program written in go.

* First we must define a package

  Package are just like a box, they contain some functionality inclosed within them.

  In above code example we have main package, which lets go compiler know that the package should compile as an executable. So if you are writting a software then it should contain `main` package.

  Packages enable code reusability across the Go applications

  Let us take an example:
    
    We have a package name `vehicles`. Vehicles has some features that are similer to all ranges of  vehicles all those features that are similer per se can be reused are all kept inside this package and can be imported everywhere whenever we need it. Lets say we need to build a car, then we could just import `vehicles` package and use those features that are similer. 

* Here in the sample code above we have imported `fmt` package `fmt` package have some functionality that can be used anywhere on the project.

  Later on the code we have code snippet that reads `fmt.Println("Hello World")` Println is a functionality from the `fmt` package, we are just using it on our program.

* Now we can see `main` function, `main` function is the entry point of our program, our go compiler first searches for `main` function and executes it.

  `main` function is like a door of our house, we use the door to enter inside our house, likewise go compiler uses `main` function to enter inside a program. Next time you write go program don't forget to write a `main` function as well.

  *Note: If you are confused about functions don't worry I will explain them later on this note.*

* Inside `main` function there is a line that reads `fmt.Println("Hello World")`
this line is simply using the print functionality provided by `fmt` package that we imported.

* Save code with `.go` extension and run your go program from terminal using command `go run yourFileName.go`

* If no syntax error you will see `Hello World` on the console.  