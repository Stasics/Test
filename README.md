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

12)Дан фрагмент кода на С++. Что отобразится на экране после его выполнения?
```cpp
class Point{ 
};
 
int main(){
    Point p;
    std::cout << sizeof(p);
}
```
<code>1</code>

13)Дан фрагмент кода на языке С++. Что будет на экране в результате выполнения данного фрагмента?
```cpp
class SomeClass{
public:
    int value = 1;
    void method(int value){
        value = value;
    }
} s;

s.method(5);
std::cout << s.value;
```
<code>1</code>

14)Язык Go. Что будет выведено на экран в результате работы этого кода?
```go
package main
import "fmt"

type Data struct{
    i int
}

func (d Data) method(){
    d.i = 1
}

func main() {
    var d *Data = &Data{}
    d.method()
    fmt.Print(d.i)
}
```
<code>0</code>

15)Дан фрагмент кода на С++.
```cpp
class SomeClass{
    int value = 0;
public:
    void method() const{
        value = 1;
        std::cout << value;
    }
};

int main(){
    const SomeClass s;
    s.method();
}
```
<code>Добавить ключевое слово mutable к объявлению value;</code>

16)Дан фрагмент кода на С++. Каким образом можно получить доступ к полю x переменной p?
```cpp
struct Point{
    double x, y;
} p;
```
<code>p.x;</code>

17)Дан фрагмент кода на С++. Что будет содержать переменная container после его выполнения?
```cpp
std::map<std::string, int> container{{"1", 2}, {"3", 2}};
container[-1] = 5;
```
<code>Ошибка компиляции - недопустимый тип</code>

18)Дан фрагмент кода на С++. Что будет содержать переменная container2 после его выполнения?
```cpp
std::set<int> container1{4, 3, 2, 1, 2, 3, 4};
std::vector<int> container2(container1.begin(), container1.end());
```
<code>1, 2, 3, 4</code>

19)Дан фрагмент кода на языке С++. Что выведется на экран в результате его работы?
```cpp
enum class Color {
    YELLOW,
    BLACK,
    PINK,
    GREEN
};

Color color = Color::BLACK;
std::cout << color;
```
<code>Ошибка. Для Color не определён оператор <<</code>

20)Дан кода на Go. Что будет выведено на экран в результате его выполнения:
```go
package main
import "fmt"

func change(abc []int) {
    abc = append(abc, 4)
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
<code>[4 4 4 4]</code>/<br>
<code>[1 2 3]</code>

21)Язык С++. Что будет напечатано в результате исполнения следующего кода?
```cpp
#include <iostream>

class A{
public:
    virtual void get(){
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
<code>C</code>

22)Язык Go. Дан фрагмент кода:
```go
type A struct{
    value int
}

func (a A) get() int{
    return a.value
}

func (a A) set(val int){
    a.value = val
}

type Accessor interface{
    get() int
    set(val int)
}

func main() {
    var obj A
    g := Accessor(obj)
    g.set(10)
    
    fmt.Print(obj.get())
}
```
<code>0</code>

23)Язык Go. Что будет выведено на экран в результате работы этого кода?
```go
package main
import "fmt"

type Data struct{
    i int
}

func (d *Data) method(){
    d.i = 1
}

func main() {
    var d Data = Data{}
    d.method()
    fmt.Print(d.i)
}
```
<code>1</code>

24)Какое, из перечисленных, ключевых слов нужно использовать при объявлении структуры в С++?</br>
<code>struct</code>

25)Дан код на языке Go:
```go
#include <iostream>
#include <map>

void add(std::map<int, int> c, int value){
    c[c.size()] = value;
}

int main(){
    std::map<int, int> container;
    add(container, 10);
    std::cout << container.size();
}
```
<code>Переменная container не изменится;</code>

26)Дан фрагмент кода на Go. Каким образом можно получить доступ к полю x переменной var p *Point = &Point{}?
```cpp
type Point struct{
    x float64
    y float64
}
```
<code>fmt.Print( (*p).x )</code></br>
<code>fmt.Print( p.x )</code>

27)Дан фрагмент кода на С++. Что будет содержать переменная container2 после его выполнения?
```cpp
std::vector<int> container1{4, 3, 2, 1, 2, 3, 4};
std::set<int> container2(container1.begin(), container1.end());
```
<code>1, 2, 3, 4</code>

28)Дан фрагмент кода на С++. Что будет содержать переменная container2 после его выполнения?
```cpp
std::vector<int> container1{4, 3, 2, 1, 2, 3, 4};
std::vector<int> container2(container1.begin(), container1.end());
```
<code>4, 3, 2, 1, 2, 3, 4</code>

29)Дан кода на Go. Что будет выведено на экран в результате его выполнения:
```go
package main
import "fmt"

func change(abc []int) {
    abc = append(abc, 4)
    for i := range abc {
        abc[i] = 4
    }
    fmt.Println(abc)
}

func main() {
    abc := []int{1, 2, 3}
    change(abc)
    abc = append(abc, 4)
    fmt.Println(abc)
}
```
<code>[4 4 4 4]</code></br>
<code>[1 2 3 4]</code>

30)Дан фрагмент кода на Go. Что будет содержать переменная container после его выполнения?
```go
var container map[int]int = make(map[int]int)
container[-1] = 1
```
<code>Ключ: -1 со значением: 1</code>

31)Язык С++. Что будет напечатано в результате исполнения следующего кода?
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
    virtual void get(){
        std::cout << 'B';
    }
};

class C: public B{
public:
    virtual void get(){
        std::cout << 'C';
    }
};

int main(){
    A* obj = new C;
    obj->get();
}
```
<code>A</code>

32)Язык Go. Дан фрагмент кода:
```go
type A struct{
    value int
}

func (a *A) get() int{
    return a.value
}

func (a *A) set(val int){
    a.value = val
}

type Accessor interface{
    get() int
    set(val int)
}

func main() {
    var obj A
    g := Accessor(&obj)
    g.set(10)
    
    fmt.Print(obj.get())
}
```
Что будет выведено в результате его работы?</br>
<code>10</code>

33)Дан фрагмент кода на С++. Что отобразится на экране после его выполнения?
```cpp
class Point{
    char i;
public:
    Point(char val):i(val){}
};
 
int main(){
    Point p;
    std::cout << sizeof(p);
}
```
<code>Ошибка. Отсутствует конструктор по умолчанию</code>

34)Дан фрагмент кода на языке С++. Что будет на экране в результате выполнения данного фрагмента?
```cpp
class SomeClass{
public:
    int value = 1;
    void method(int value){
        this->value = value;
    }
} s;

s.method(5);
std::cout << s.value;
```
<code>5</code>

35)Где можно объявить структуру в языке С++?</br>
<code>Внутри других структур;</code></br>
<code>Вне функции;</code></br>
<code>Внутри тела функции;</code>

36)Дан фрагмент кода на С++. Что будет содержать переменная container после его выполнения?
```cpp
std::map<int, int> container;
int a = container[-1];
```
<code>Ключ: -1 со значением: 0</code>

37)Дан фрагмент кода на С++. Что будет содержать переменная container2 после его выполнения?
```cpp
std::vector<int> container1{4, 3, 2, 1, 2, 3, 4};
std::unordered_set<int> container2(container1.begin(), container1.end());
```
<code>1, 2, 3, 4 но в порядке зависящем от хэш-функции</code>

38)Какое, из перечисленных, ключевых слов нужно использовать при объявлении структуры в Go?</br>
<code>struct</code>

39)Дан фрагмент кода на С++. Что будет содержать переменная container после его выполнения?
```cpp
std::vector<int> container{1, 2, 3, 2};
container[-1] = 5;
```
<code>Ошибка доступа - указанного элемента не существует</code>

40)Дан фрагмент кода на языке С++. Что выведется на экран в результате его работы?
```cpp
enum Color {
    YELLOW,
    BLACK = 0,
    PINK,
    GREEN
};

Color color = Color::BLACK;
std::cout << color;
```
<code>0</code>

41)Дан кода на Go. Что будет выведено на экран в результате его выполнения:
```go
package main
import "fmt"

func change(abc []int) {
    abc = append(abc, 4)
    for i := range abc {
        abc[i] = 4
    }
    fmt.Println(abc)
}

func main() {
    abc := []int{1, 2, 3}
    abc = append(abc, 4)
    change(abc)
    fmt.Println(abc)
}
```
<code>[4 4 4 4 4]</code></br>
<code>[4 4 4 4]</code>

42)Дан код на языке Go:
```go    
package main
import "fmt"

func add(c map[int]int, value int){
    c[len(c)] = value
}

func main() {
    var container map[int]int = make(map[int]int)
    add(container, 10)
    fmt.Print(len(container))
}
```
В результате его исполнения:</br>
<code>Переменная container изменится;</code>

43)Язык С++. Что будет напечатано в результате исполнения следующего кода?
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
    virtual void get(){
        std::cout << 'B';
    }
};

class C: public B{
public:
    virtual void get(){
        std::cout << 'C';
    }
};

int main(){
    C* obj = new A;
    obj->get();
}
```
<code>Ошибка</code>

44)Дан фрагмент кода на С++:
```cpp
class MyClass{
public:
    double i = 1.0;
};

double operator+ (MyClass a, double b){
    return a.i + b;
}

MyClass obj;
double value = 2.0;
```
Выберите все выражения, которые НЕ вызовут ошибки:</br>
<code>value + value;</code></br>
<code>obj + value;</code></br>
<code>obj + 2.0;</code>

45)Дан фрагмент кода на С++. Что отобразится на экране после его выполнения?
```cpp
class Point{
    char i;
public:
    Point(char val=0):i(val){}
};
 
int main(){
    Point p;
    std::cout << sizeof(p);
}
```
<code>1</code>

46)Язык С++. Дан класс:
```cpp
class SomeClass{
    int value = 0;
public:
    void one(){
        value = 1;
    }
    void one() const{
        std::cout << value;
    }
    
    void two(){
        value = 2;
    }
    
    void three() const {
        std::cout << 3;
    }
    
    void four() {
        std::cout << 4;
    }
};
```
и переменная созданная таким образом:
```cpp
const SomeClass s;
```
Какие из перечисленных вызовов метода НЕ приведут к ошибке?</br>
<code>s.three();</code></br>
<code>s.one();</code>

47)Каким образом можно создать переменную типа структура в языке С++?
```cpp
struct Point{
    int x,y;
} p1, p2;
```
```cpp
struct Point{
    int x,y;
};
```
```cpp
Point p1, p2;
struct{
    int x,y;
} p1, p2;
```

48)Дан фрагмент кода на языке С++. Что выведется на экран в результате его работы?
```cpp
enum Color {
    YELLOW = 1,
    BLACK = 1,
    PINK,
    GREEN
};

Color color = Color::BLACK;
std::cout << color;
```
<code>1</code>

49)Язык Go. В текущий пакет из пакета other была импортирована структура:
```go
type Book struct {
    Title       string
    author      string
    Description string
    Price       int
    pages       int
}
```
Какие поля будут доступны для использования в текущем пакете?</br>
<code>Price</code></br>
<code>Description</code></br>
<code>Title</code>

50)Дан фрагмент кода на Go. Что будет содержать переменная container после его выполнения?
```go
var container map[int]int = make(map[int]int)
var a = container[-1]
```
<code>Ключ: -1 со значением: 0</code>

51)Язык С++. Что будет напечатано в результате исполнения следующего кода?
```cpp
#include <iostream>

class A{
    char value = 'a';
public:
    virtual void get(){
        std::cout << value;
    }
};

class B: public A{
    char value = 'b';
public:
    virtual void get(){
        std::cout << value;
    }
};

void print(A* obj){
    obj->get();
}

int main(){
    print(new B);
}
```
<code>b</code>

52)Дан фрагмент кода на С++:
```cpp
struct MyClass{
    double i = 1.0;
};

double operator+ (double a, MyClass b){
    return a + b.i;
}

MyClass obj;
double value = 2.0;
```
Выберите все выражения, которые НЕ вызовут ошибки:</br>
<code>value + value;</code></br>
<code>value + obj;</code></br>

53)Язык С++. Дан класс:
```cpp
class SomeClass{
    int non_static_value = 0;
    static const int static_value = 0;
public:
    static void static_method() {
    }
    static void other_static_method() {
    }    

    void non_static_method() {
    }
    void other_non_static_method() {
    }
};
```
Выберите все верные утверждения.</br>
<code>В static_method можно использовать other_static_method;</code></br>
<code>Чтобы вызвать static_method НЕ обязательно иметь объект;</code></br>
<code>В static_method можно использовать static_value;</code></br>

54)Язык С++. Что будет напечатано в результате исполнения следующего кода?
```cpp
#include <iostream>

class A{
    char value = 'a';
public:
    void get(){
        std::cout << value;
    }
};

class B: public A{
    char value = 'b';
public:
    void get(){
        std::cout << value;
    }
};

void print(A* obj){
    obj->get();
}

int main(){
    print(new B);
}
```
<code>a</code>

55)Язык С++. Дан класс:
```cpp
class SomeClass{
    int non_static_value = 0;
    static const int static_value = 0;
public:
    static void static_method() {
    }
    static void other_static_method() {
    }    

    void non_static_method() {
    }
    void other_non_static_method() {
    }
};
```
Выберите все верные утверждения.
<code>В non_static_method можно использовать other_non_static_method;</br>
В non_static_method можно использовать static_method;</br>
В non_static_method можно использовать non_static_value;</br>
Чтобы вызвать non_static_method обязательно нужно создать объект;</br>
В non_static_method можно использовать static_value;</code>
