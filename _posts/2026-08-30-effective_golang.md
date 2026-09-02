---
layout: post
title: "Effective golang"
date: 2026-08-30
---

![Golang fuck you](/assets/images/posts/headers/golang_fuck.png)

Bueno, aprendiendo golang, este es mi base de recursos:

- [Effective golang](https://go.dev/doc/effective_go)
- [Common golang errors](https://100go.co/)
- [Golang tests](https://quii.gitbook.io/learn-go-with-tests)
- [Golang further](https://lets-go-further.alexedwards.net/)

## Indice

## Fundamentos

```go
package main

import "fmt"

func main(){
   fmt.Print("Halo Zyrrex")
}
```

### Variables y constantes

```go
// Declaración y asignación
var x int
x = 16

// Asignación e inferencia de tipado
z := "Zyrrex"

// Declaración| Asignación e inferencia múltiple
var(
   a int
   b bool
)
a, b := 14, 15

// Constantes
const a int = 14
const (
   b = 15
   c bool = true
)
```

### Tipos de datos

- int
- string
- bool
- rune (investigar)
- complex (investigar)

### Operadores

- Aritméticos: (`+`, `-`, `*`, `/`, `%`)
- Relacionales: (`&&`, `||`)
- Lógicos:

## Sentencias de control

```go
x := 19
if x > 18 {
   fmt.Print("mayor de edad")
} else {
   fmt.Print("es menor")
}
```

```go
```

## Bucles

```go
for i := 0; i < 10; i++ {
   fmt.Print(i)
}
```

```go
```

## Products| Practice

- CLI tools (Go blueprint, React AWS Go)
- GRPC
- Pipeline jobs/ scripts

## User interface

- [Fyne](https://fyne.io/)
- [Wails](https://wails.io/)

## Referencias

- [Buble](https://github.com/charmbracelet/bubbletea) -> No se que carajos hace