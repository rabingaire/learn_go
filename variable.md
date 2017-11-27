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