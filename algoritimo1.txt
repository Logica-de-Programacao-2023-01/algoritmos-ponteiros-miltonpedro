package main

import "fmt"

func ptr(ptr *int, n int) {
	numero := 0

	for i := 1; i <= n; i++ {
		numero += i
	}
	*ptr = numero
}

func main() {
	numero := 0
	n := 6

	fmt.Println("Antes da troca:")
	fmt.Println("O numero é:", numero)

	ptr(&numero, n)

	fmt.Println("Depois da troca:")
	fmt.Println("O numero é", numero)
}
