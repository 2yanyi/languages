# Languages

<br>

|语言|C|Go|Js|Kotlin|
|-|-|-|-|-|

<br>

## Print format

```c
// C
#include <stdio.h>

void main() {
    char out[] = {"C string"};
    printf("print %s\n", out);
}
```
```go
// Go
package main

import "fmt"

func main() {
	var out = "Go string"
	fmt.Printf("print %s\n", out)
}
```
```js
// Js
function __main_() {
    let out = "Js string";
    console.log(`print ${out}`);
}
__main_();
```
```kotlin
// kotlin
package main

fun main() {
    var out = "Kotlin string"
    println("print $out")
}
```

<br>

## If

```c
// C
int i;
if (i == 0) {} else {}
if (i == 0) {} else if (i == 1) {} else {}
```
```go
// Go
var i int
if i == 0 {} else {}
if i == 0 {} else if i == 1 {} else {}
```
```js
// Js
let i;
if (i === 0) {} else {}
if (i === 0) {} else if (i === 1) {} else {}
```
```kotlin
// kotlin
var i = 1
if (i == 0) {} else {}
if (i == 0) {} else if (i == 1) {} else {}
```

<br>

## Switch

```c
// C
int i;
switch (i) {
case 1:
	// ...
	break;
case 2:
	// ...
	break;
default:
	// ...
}
```
```go
// Go
var i int
switch i {
default:
	// ...
case 1:
	// ...
	fallthrough // 继续执行下一个 "case"
case 2:
	// ...
}

// or
switch {
case i == 1:
	// ...
}
```
```js
// Js
let i;
switch (i) {
case 1:
    // ...
    break;
case 2:
    // ...
    break;
default:
    // ...
}
```
```kotlin
// kotlin
var i = 0
when (i) {
1 ->
    // ...
2 ->
    // ...
else ->
    // default...
}

// or
when {
i == 1 ->
    // ...
}
```

<br>

## For

```c
// C
for (int i = 1; i < 10; ++i) {
    // break; // 跳出循环
    // continue; // 忽略本次循环
    // ...
}
```
```go
// Go
for i := 0; i < 10; i++ {
    // break // 跳出循环
    // continue // 忽略本次循环
    // ...
}

// or
i = 0
for i < 10 {
	i++
	// ...
}

// or
i = 0
for {
	i++
	if i > 10 {
        break
	}
	// ...
}
```
```js
// Js
for (let i = 0; i < 10; i++) {
    // break; // 跳出循环
    // continue; // 忽略本次循环
    // ...
}
```
```kotlin
// kotlin
for (i in 0..10) {
    // break // 跳出循环
    // continue // 忽略本次循环
    // ...
}
```

<br>

## Function

```c
// C
int demo(x, y) {
    return x + y;
}

int main() {
    int x = demo(3, 5);
    printf("%d\n", x);
}
```
```go
// Go
func demo(x, y int) (int, int) {
	return x, y
}

func main() {
	x, y := demo(3, 5)
	fmt.Printf("%d,%d\n", x, y)
}
```
```js
// Js
function demo(x, y) {
    return {x, y};
}

let {x, y} = demo(3, 5);
console.log(`${x},${y}`);
```
```kotlin
// kotlin
fun demo(x: Int, y: Int): Pair<Int, Int> {
    return Pair(x, y)
}

fun main() {
    val (x, y) = demo(3, 5)
    println("$x,$y")
}
```

<br>

## List

```c
// C
```
```go
// Go
var intList = make([]int, 0)

intList = append(intList, 100)
intList = append(intList, 200)

for i, it := range intList {
	fmt.Printf("%d:%d\n", i, it)
}
```
```js
// Js
const intList = [];

intList.push(1);
intList.push(2);

for (let i = 0; i < intList.length; i++) {
    let it = intList[i];
    console.log(`${i}:${it}`);
}
```
```kotlin
// kotlin
val intList: MutableList<Int> = mutableListOf()

intList.add(1)
intList.add(2)

for (i in intList.indices) {
    val it = intList[i];
    println("$i:$it")
}
```

<br>

## Map

```c
// C
```
```go
// Go
var fruitMap = make(map[string]string)

fruitMap["001"] = "banana"
fruitMap["002"] = "orange"

if it, has := fruitMap["001"]; !has {
	fmt.Println("not found")
} else {
	fmt.Println(it)
}

delete(fruitMap, "001")
```
```js
// Js
const fruitMap = new Map();

fruitMap["001"] = "banana";
fruitMap["002"] = "orange";

let it = fruitMap["001"];
if (it === undefined) {
    console.log("not found");
} else {
    console.log(it);
}

delete fruitMap["001"];
```
```kotlin
// kotlin
val fruitMap: MutableMap<String, String> = mutableMapOf()

fruitMap["001"] = "banana"
fruitMap["002"] = "orange"

val it = fruitMap["001"]
if (it == null) {
    println("not found")
} else {
    println(it)
}

fruitMap.remove("001")
```

<br>

## String

```c
// C
```
```go
// Go
```
```js
// Js
```
```kotlin
// kotlin
```

<br>

## Time

```c
// C
```
```go
// Go
```
```js
// Js
```
```kotlin
// kotlin
```
