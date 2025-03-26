#kotlin/basic
- Một phần của [[Kotlin in a nutshell]]
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
- Sử dụng : \<type> = để khai báo kiểu biến và giá trị, sử dụng to\<Type>  để cast type
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
## Variable
- var thay đổi được (mutable), val không thay đổi được (immutable)
```kotlin
val a = 2
a = 3
=> Error: val cannot be reassinged
```
## Conditional
- If else
```kotlin
if (condition) {
	do1
}
else if{
	do2
}
else {
	do3
}
```
- When - switch case trong kotlin, sử dụng condition -> do mỗi case
```kotlin
when (variable) {
	0 -> do1
	in 1..39 -> do2
	else -> do3
}
```
- For loop, không cần định nghĩa iterator, sử dụng .withIndex() để lấy ra index từng phần tử
```kotlin
//Auto iterate
val pets = arrayOf("dog", "cat", "canary") 
for (element in pets) { 
	print(element + " ") 
}
⇒ dog cat canary
//withIndex()
for ((index, element) in pets.withIndex()) { 
	println("Item at $index is $element\n") 
}
⇒ Item at 0 is dog 
Item at 1 is cat 
Item at 2 is canary
//Step
for (i in 5 downTo 1) print(i)
for (i in 3..6 step 2) print(i)
for (i in 'd'..'g') print (i)
```
- While
```kotlin
while (condition) {}
do {} while (condition)
```
- Repeat - chỉ định số lần lặp
```kotlin
repeat(10) {}
```
## Lists and arrays
### Lists
- Có thứ tự, có thể truy cập index, có thể lặp
```kotlin
//Immutable list
listOf("","","")
//Mutable list
mutableListOf("","","")
//Mutable list can be editted with method
myList.remove(value)
```
### Arrays
- Có thể truy cập index, size fixed, nhanh hơn nhưng kém linh hoạt về kiểu và size
```kotlin
arrayOf("","","")
```
## Null safety
- BIến trong Kotlin mặc định không Null
- Muốn gán null cần safe call operator (?)
```kotlin
var a: Int? = null
```
- Throw exception nếu null với !!
```kotlin
val len = s!!.length
```
- Elvis operator (?:): nếu giá trị đầu không null thì gán, không thì gán giá trị 2
```kotlin
val a = b ?: 0
```

