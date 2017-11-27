# Variable

### Default Value 

```go
package main

import "fmt"

func main() {
    var a int // Default value is always 0 upon declaration
    var b string // Default value is always "" upon declaration
    var c bool // Default value is always false upon declaration
    var d float32 // Default value is always 0 upon declaration
    var e float64 // Default value is always 0 upon declaration

    fmt.Println(a) // 0
    fmt.Println(b) // ""
    fmt.Println(c) // false
    fmt.Println(d) // 0
    fmt.Println(e) // 0
}
```

* In above code example we are learning the different data types supported by go language.


### Declaration and Definition

```go
package main

import "fmt"

func main() {
    var a int
    var b string = "Hello World"
    var c, d string = "Hello", "World"
    var (
        e int = 20
        f string = "Hello"
    )
    g := 12.5
    var h = 10 // Go will identify h as int during compile time when type is not specified 

    const pi = 3.14 // This is constant we can't change this value ever again

    fmt.Println(a) // 0
    fmt.Println(b) // "Hello World"
    fmt.Println(c) // "Hello"
    fmt.Println(d) // "World"
    fmt.Println(e) // 20
    fmt.Println(f) // "Hello"
    fmt.Println(g) // 12.5
    fmt.Println(pi) // 3.14
    fmt.Println(h) // 10
}
```

* In above code example we are learning the different ways to declare a variable.

* `var b string = "Hello World"`
  
  Here the `b` is declared and defined as `string`

* `var c, d string = "Hello", "World"`

  Here we are declaring two variable on a single line with same data type

* Here we are declaring two variable at a time with different data types.
    ```go
    var (
        e int = 20
        f string = "Hello"
    )
    ```


* `g := 12.5`
  
  This is the shortest way to declare and define a variable, Go will automatically identify the data type by looking at the value on right side at the compile time.

* `const pi float32 = 3.14`

   This is how you declare and define a `const` in Go language.

### Error

```go
package main

import "fmt"

func main() {
    var a int = 10

    a = 10.5 // We cannot do this a is already defined as int so we can't reassign it to float

    var a = 20 // We cannot do this a is already declared, we can't redeclare it again

    const pi = 3.14

    pi = 4.14 // Error constant can't be redefined
    
}
```

* Go language is a statically typed language, that means once a variable defined as a int, float, or bool it can never be changed into another type later on the other parts of the code.

* Once a variable is declared we can't redeclare it again.

* We can't change the value of constant ever, Go will throw error in compile time if the value of const is found to be redefined.