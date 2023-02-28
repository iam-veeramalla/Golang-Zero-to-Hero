package main

import "fmt"

func main() {
    for i := 1; i <= 100; i++ {
        if (i%3 == 0 || i%5 == 0) && i%15 != 0 {
            fmt.Println(i)
        }
    }
}
