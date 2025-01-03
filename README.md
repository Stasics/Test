# Дополнительный тест

1) Дана лямбда-функция на языке С++. Какой её тип возвращаемого значения?
```cpp
[](int a, int b){return a > b;};
```
<code> bool </code>

2)Дан фрагмент кода на языке С++. Что выведется на экран в результате его работы?
```cpp
enum Color {
    YELLOW,
    BLACK,
    PINK,
    GREEN
};

Color color = Color::BLACK;
std::cout << color;
```
<code>1</code>

3)Дан фрагмент кода на С++. Что будет содержать переменная container после его выполнения?
```cpp
std::map<int, int> container{{1, 2}, {3, 2}};
container[-1] = 5;
```
<code>Пары: -1:5, 1:2, 3:2</code>

4)Дан фрагмент кода на С++. Что будет содержать переменная container после его выполнения?
```cpp
std::set<int> container{1, 2, 3, 4};
container.insert(container.begin(), 4);
```
<code>1, 2, 3, 4</code>

5)Дан фрагмент кода на Go. Что будет содержать переменная container после его выполнения?
```cpp
var container map[int]int
container[-1] = 1
```
<code>Ошибка во время исполнения - под словарь не выделена память</code>

6)Дан фрагмент кода на С++. Что будет содержать переменная container после его выполнения?
```cpp
std::vector<int> container{1, 2, 3, 4};
container.insert(container.begin(), 4);
```
<code>4, 1, 2, 3, 4</code>

7)Дан фрагмент кода на С++ и класс MyClass объявленный как:
```cpp
class MyClass{};
```
Выберите все верные варианты, которые являются допустимыми объявлениям.<br>
<code>double operator+ (double a, MyClass b);</code></br>
<code>double operator+ (MyClass a, double b);</code>

8)Язык Go. Какие поля могут быть в структурном типе?</br>
<code>Анонимные поля;</code></br>
<code>Не константные поля;</code>

9)Дан кода на Go. Что будет выведено на экран в результате его выполнения:
```go
package main
import "fmt"

func change(abc []int) {
    for i := range abc {
        abc[i] = 4
    }
    fmt.Println(abc)
}

func main() {
    abc := []int{1, 2, 3}
    change(abc)
    fmt.Println(abc)
}
```
<code>[4 4 4]</code></br>
<code>[4 4 4]</code>

10)Язык С++. Что будет напечатано в результате исполнения следующего кода?
```cpp
#include <iostream>

class A{
public:
    void get(){
        std::cout << 'A';
    }
};

class B: public A{
public:
    void get(){
        std::cout << 'B';
    }
};

class C: public B{
public:
    void get(){
        std::cout << 'C';
    }
};

int main(){
    A* obj = new C;
    obj->get();
}
```
<code>A</code>

11)Язык Go. Дан фрагмент кода:
```go
type A struct{
    value int
}

type Printer interface{
    print()
}

func main() {
    var obj A
    p := Printer(&obj)
    p.print()
}
```
```cpp
func (a *A) print(){
    fmt.Print(a.value)
}
```
