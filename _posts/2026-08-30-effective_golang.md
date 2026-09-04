---
layout: post
title: "Effective golang"
date: 2026-08-30
last_modified_at: 2026-09-03
---

{% raw %}
![Golang fuck you](/assets/images/posts/headers/golang_fuck.png)

Bueno, aprendiendo golang, este es mi base de recursos:

- [Effective golang](https://go.dev/doc/effective_go)
- [Common golang errors](https://100go.co/)
- [Golang tests](https://quii.gitbook.io/learn-go-with-tests)
- [Golang further](https://lets-go-further.alexedwards.net/)

## Indice

---

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

---

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
x := "March"
switch x {
   case "March": fmt.Println("Halo")
   default: fmt.Println("Test")
}
```

---

## Bucles

```go
for i := 0; i < 10; i++ {
   fmt.Print(i)
}

for index, elem := range listado {
   fmt.Println(elem)
}
```

---

## Arreglos

```go
var arr1 [10]int
arr1[2] = 12

arr2 := [2][2]int{{12, 16}, {1, 2}}
```

### Métodos

---

## Slices

### Métodos

---

## Maps

```go
objUser := map[string]int{
   "name": "Carlos", "age": "24"
}
```

### Métodos

---

## Functions

```go
func sayhello(string mensaje) {
   fmt.Println(mensaje)
}

// función con valor de retorno
func buildMessage(string mensaje) string {
   return mensaje
}

// Función con más de un valor de retorno
func buildMessage2(string mensaje) (string, int) {
   return mensaje, len(mensaje)
}

// Función con nro de parámetros desconocido
func allinone(arg...int){
}

// Función como valor
myFunc := func(){}
```

### Manejo avanzado

- defer
- callbacks

---

## Packages

Conjunto de funciones y de informacion

```go
```

### Packages de referencia

- fmt
- io
- bufio
- sort
- strconv
- os
- sync
- flag
- encoding/json
- html/template
- net/http
- unsafe
- reflect
- os/exec

---

## Comandos de golang

```bash
go build
go install
go test
```

---

## Mas avanzado

### Structs

### Pointers

### Allocation

### Types

### Conversions

### Interfaces

### Methods

### Paralelismo

### Concurrencia

---

## Conocimientos logicos

- Scope
   - Local
   - Global
- Pánico(page 35)

---

## Products| Practice

- CLI tools (Go blueprint, React AWS Go)
- GRPC
- Pipeline jobs/ scripts

---

## User interface

- [Fyne](https://fyne.io/)
- [Wails](https://wails.io/)

---

## Referencias

- [Buble](https://github.com/charmbracelet/bubbletea) -> No se que carajos hace
{% endraw %}