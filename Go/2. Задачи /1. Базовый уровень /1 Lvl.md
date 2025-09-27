# 1. Сумма четных чисел в диапазоне

Программа считывает два числа a и b. Найти сумму всех четных чисел в заданном диапазоне от a до b включительно.

## Входные данные

```
5 12
```

## Выходные данные

```
42
```


# Решение
<details>
<summary>Solution (Click) </summary>

```go
package main

import "fmt"

func main() {
	var a, b int
	fmt.Scan(&a, &b) // два числа a и b через пробел или Enter

	if a > b { // если первое число больше второго, меняем местами
		a, b = b, a
	}

	sum := 0
	for i := a; i <= b; i++ { // <= чтобы включить b (важно!)
		if i%2 == 0 {
			sum += i
		}
	}

	fmt.Println(sum)
}
```
</details> 


# 2. Проверка четности числа

Напишите программу, которая определяет, является ли введенное целое число четным или нечетным.

## Входные данные

```
8
```

## Выходные данные

```
четное
```


# Решение
<details>
<summary>Solution (Click) </summary>

```go
package main

import "fmt"

func main() {
	num := 0
	fmt.Scan(&num)

	if num%2 == 0 {
		fmt.Println("четное")
	} else {
		fmt.Println("нечетное")
	}
}
```
</details> 


# 3. Максимум из трех чисел

Напишите программу, которая находит наибольшее из трех введенных целых чисел.

## Входные данные

```
12 7 19
```

## Выходные данные

```
19
```

# Решение
<details>
<summary>Solution (Click) </summary>

```go
package main

import "fmt"

func main() {
	var a, b, c int
	fmt.Scan(&a, &b, &c)

	if a > b && a > c {
		fmt.Println((a))
	} else if b > c && b > a {
		fmt.Println(a)
	} else {
		fmt.Println(c)
	}
}
```
</details> 

