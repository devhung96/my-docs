---
sidebar_position: 5
title:  04 - Conditions & Loops
sidebar_label: 04 - Conditions & Loops
description: Variables & DataType
keywords: [golang]
---

# Conditions & Loops & Switch case

## Conditions
1. If else statement:
```go
if condition1 {
    // Thực hiện hành động nếu điều kiện 1 đúng
} else if condition2 {
    // Thực hiện hành động nếu điều kiện 2 đúng
} else {
    // Thực hiện hành động nếu cả hai điều kiện trên sai
}
```
3. Switch statement:
```go
switch codition {
    case value1: 
        // Excute when condition is value1
    case value2:
        // Excute when condition is value2
    default:
        // Excute when condition is not value1 or value2
}
```
## Loops
1. for
```go
for i := 0; i < 10; i++ {
    // Excute when i < 10
}

// Vòng lặp chỉ sử dụng điều kiện:
i := 0
for i < 5 {
    // Thực hiện hành động trong vòng lặp
    i++
}

// Vòng lặp với range:
for index, value := range array {
    // Excute when index < len(array)
}
```
2. while
3. do-while

