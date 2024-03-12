### 1.  Valor da variável SOMA após o processamento:
```go
package main

import "fmt"

func main() {
	INDICE := 13
	SOMA := 0
	K := 0

	for K < INDICE {
		K = K + 1
		SOMA = SOMA + K
	}

	fmt.Println(SOMA)
}
```
### 2. Verifica se um número pertence à sequência de Fibonacci:
```go
package main

import "fmt"

func isFibonacci(num int) bool {
	a, b := 0, 1

	for b <= num {
		if b == num {
			return true
		}
		a, b = b, a+b
	}

	return false
}

func main() {
	num := 13 // Você pode alterar o número conforme necessário
	if isFibonacci(num) {
		fmt.Println("O número pertence à sequência de Fibonacci.")
	} else {
		fmt.Println("O número NÃO pertence à sequência de Fibonacci.")
	}
}
```

### 3. Descubra a lógica e complete o próximo elemento:
```plaintext
a) 1, 3, 5, 7, 9
b) 2, 4, 8, 16, 32, 64, 128
c) 0, 1, 4, 9, 16, 25, 36, 49
d) 4, 16, 36, 64, 100
e) 1, 1, 2, 3, 5, 8, 13
f) 2, 10, 12, 16, 17, 18, 19, 20
```
### 4. Solução para o problema dos interruptores e lâmpadas:
```plaintext
1. Ligue o primeiro interruptor e aguarde alguns minutos.
2. Desligue o primeiro interruptor e ligue o segundo interruptor.
3. Entre na sala com as lâmpadas.

- A lâmpada acesa está conectada ao segundo interruptor.
- A lâmpada apagada e quente está conectada ao primeiro interruptor.
- A lâmpada apagada e fria está conectada ao terceiro interruptor.
```

### 5. Programa para inverter os caracteres de uma string
```go
package main

import "fmt"

func reverseString(input string) string {
	runes := []rune(input)
	for i, j := 0, len(runes)-1; i < j; i, j = i+1, j-1 {
		runes[i], runes[j] = runes[j], runes[i]
	}
	return string(runes)
}

func main() {
	str := "Hello, World!" // Você pode alterar a string conforme necessário
	reversedStr := reverseString(str)
	fmt.Println(reversedStr)
}
```
