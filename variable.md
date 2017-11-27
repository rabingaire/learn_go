# Variable

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

    fmt.Println(a) // 0
    fmt.Println(b) // "Hello World"
    fmt.Println(c) // "Hello"
    fmt.Println(d) // "World"
    fmt.Println(e) // 20
    fmt.Println(f) // "Hello"
    fmt.Println(g) // 12.5
}
```

```go
package main

import "fmt"

func main() {
    var a int = 10

    a = 10.5 // We cannot do this a is already defined as int so we can't reassign it to float

    var a = 20 // We cannot do this a is already declared, we can't redeclared it again
    
}
```