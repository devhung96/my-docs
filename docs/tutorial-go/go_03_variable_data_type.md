---
sidebar_position: 4
title:  03 - Variables & DataType
description: Variables & DataType
keywords: [golang]
---
# Variables & DataType

## Variables
Dưới đây cách khai báo biến phổ biến trong Go:
1. Khai basic:
```go
    var name string
    var age int
```
2. Khai báo có giá trị khởi tạo:taoạo:
```go
    var name string = "name"
    var age int = 1
```
3. Short variable declaration:
```go
    name := "name"
    age := 1
```
4. Mutiple variable declaration:
```go
    var (
        name string = "name"
        age int = 1
    )
```
5. Khai báo consttant:
```go
    const name string = "name"
    const age int = 1
```

## DataType
Các kiểu dữ liệu phổ biến trong go (10):
```go
    bool : true or false
    string
    int  int8  int16  int32  int64
    uint uint8 uint16 uint32 uint64 uintptr (Kiểu số nguyên có kích thước cố định)
    float32 float64
    array: Kích thước cố định.
    struct: Kiểu dữ liệu custom có thể theo í người dùng.
    slice: Kiểu dữ liệu array mà không có kích thước cố định.
    map : Key-value giống dictionary trong c#
    function
   
```
Ví dụ dùng thực tế:
   1. Array
   ```go
   // Khai báo khởi tạo mảng cố định
   var number [8]int =  [8]int{1,2,3,4,5,6,7,8}
   number[0] = 10;
   ```
   2. Slice
   ```go
   // Khai báo khởi tạo slice
   var number []int = []int{1,2,3,4,5,6,7,8}
   number[0] = 30;
   ```
   3. Map:
   ```go
   // Khai báo khởi tạo map
   var number map[string]int = map[string]int{
       "one": 1,
       "two": 2,
       "three": 3
   }
   ```
   4. Struct:
   ```go
   // Khai báo khởi tạo struct
   type Person struct {
       name string
       age int
   }

   person := Person{
        Name: "Alice",
        Age:  25,
        City: "New York",
    }
   ```
   5. Constants:
   ```go
   // Khai báo khởi tạo constant
   const (
        Red    = "red"
        Green  = "green"
        Blue   = "blue"
    )
    // Cách khai báo Gender enum giống c#
    type Gender int
    const (
        Male Gender = iota
        Female
    )
    // iota là từ khóa giúp tự động tăng giá trị của biến 0,1,2
   ```


## Naming conventions:
1. Không sử dụng các từ khóa trong go:
```go
    break    default     func     interface    select
    case     defer       go      map          struct
    chan     else         goto    package      switch
    const    fall
```
2. Sử dụng quy tắc đặt tên biết CameCase, PascalCase, SnakeCase:
```go
    // CamelCase
    var name string = "name"
    // PascalCase
    var Name string = "name"
    // SnakeCase
    var name_string string = "name
```
3. Constant đặt tên theo quy tắc:
```
    MAX_SIZE, PI, DEFAULT_VALUE
```
4. Tên hàm theo nguyên tắc: 
```
    <chức năng>+ <hoạt động>
    VD: calculateTotal, getUserByID, validateInput
```