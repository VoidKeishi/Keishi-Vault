---
tags:
  - programming_language
  - mobile_development
type: pernament
time created: 29-10-2024
last modified: 29-10-2024
---
# Basics
## Operator
- Mathematical: + - * / %
- Increment and decrement: ++ --
- Comparison: < <= > >= == !=
- Assignment: = 
### Operator methods
- Kiểu số trong kotlin là kiểu dữ liệu nguyên thủy (primitives) nhưng có thể call methods như object
```kotlin
3.5.div(7)
=> kotlin.Double = 0.5
```
## Data types
- Integer: Long(64 bit) > Int(32 bit) > Short(16 bit) > Byte (8 bit)
- Floating-point: Double(64 bit) > Float (32 bit)
- Char: 16-bit Unicode character
- Boolean: 8-bit True/False
### Type casting
```kotlin
val i: Int = 6
println(i.toByte())
=> 6
```
### Long number
- Sử dụng gạch dưới để giúp hằng số lớn dễ đọc
```kotlin
val oneMillion = 1_000_000
```
### String
- Sử dụng ngoặc kép hoặc 3 dấu ngoặc kép
```kotlin
val s1 = "Hello world!"
val s2 = """
	var bikes = 50
"""
```
- String template
```kotlin
val s = "abc"
println("$s.length is ${s.length}")
=> abc.length is 3
```
- String concatenation
```kotlin
val number = 3
"The number is $number "
=> The number is 3
```
### Specifying type
- Sử dụng : <type> = để khai báo kiểu biến và giá trị
```kotlin
```