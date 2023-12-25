---
sidebar_position: 6
title:  06 - Class & Interface
sidebar_label:  06 - Class & Interface
description: Class & Interface
keywords: [golang]
---
# Class & Interface
## Class 
Go không phải ngôn ngữ lập trình hướng đối tượng(OOP) như Java, C#, PHP, Python,... Nhưng có hỗ trợ struct ,methods, interfaces.

## Method
```go
package main

import "fmt"

type person struct {
	name string
	age  int
}

func (p person) sayHello() {
	fmt.Println("Hello", p.name)
}
```

## Interface
```go
type Namer interface {
    Name() string
}

// Struct
type Person struct {
    name string
}

// method
func (p Person) Name() string {
    return p.name
}

```

## Generics 