<h1 align="center">Test №6 for 💯 points</h1>
<h3 align="right">Автор: Бобренко Александр</h3>

<p align="center">
  <img src="https://github.com/user-attachments/assets/72c699bf-8855-4377-b055-1b68bb26f384" alt="hasbula">
</p>

<h2></h2>

1) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int main() {
    int i = 1;
    int i = 1;
    std::cout << i;
}
```

### Ответ:
- `⛔️ a. 1`
- `✅ b. Ошибка`

2) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace D{
    int i = 1;
}

namespace C{
    using namespace D;
    int i = 2;
}

namespace A {
    namespace B {
        using namespace C;
        void print() {
            std::cout << i;
        }
    }
    int i = 3;
}

int main() {
    A::B::print();
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 3`
- `⛔️ d. 1`

3) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    std::cout << A::i;
}
```

### Ответ:
- `✅ a. 1`
- `⛔️ b. Ошибка`

4) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int i = 2;

int main() {
    int i = 3;
    {
      using namespace A;      
      std::cout << i;
    }
}
```

### Ответ:
- `✅ a. 3`
- `⛔️ b. Ошибка`
- `⛔️ c. 2`
- `⛔️ d. 1`

5) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int i = 2;

int main() {
    using namespace A;
    std::cout << i;
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 1`

6) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int i = 1;

namespace A {
    namespace B {
        void print() {
            std::cout << i;
        }
        int i = 2;
    }
}

int main() {
    int i = 3;
    A::B::print();
}
```

### Ответ:
- `⛔️ a. 2`
- `⛔️ b. Ошибка`
- `✅ c. 1`
- `⛔️ d. 3`
  
7) Язык Go. Пакет импортирован следующим образом:
`import example "github.com/vigo5190/example/name"`
Каким образом можно использовать экспортируемые имена из этого пакета в своём коде?


### Ответ:
- `⛔️ a. Имена объявленные в пакете name НЕ доступны для использования`
- `⛔️ b. Имена объявленные в пакете name доступны для использования просто по своему имени`
- `✅ c. Имя из пакета name можно использовать так: example.требуемое_имя`
- `⛔️ d. Имя из пакета name можно использовать так: name.требуемое_имя`

8) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
inline namespace A{
    int i = 1;
}

int main() {
    std::cout << i;
    int i = 2;
}
```

### Ответ:
- `⛔️ a. 2`
- `⛔️ b. Ошибка`
- `✅ c. 1`

9) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace {
    int i = 1;
}

int main() {
    std::cout << i;
}
```

### Ответ:
- `⛔️ a. Ошибка`
- `✅ b. 1`

10) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A {
    namespace B {
        void print() {
            std::cout << i;
        }
    }
}

int i = 1;

int main() {
    A::B::print();
}
```

### Ответ:
- `✅ a. Ошибка`
- `⛔️ b. 1`

11) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int A(){
    int i = 1;
}

int main() {
    int i = 2;
    std::cout << A::i;
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 1`

12) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int main(){
    bool i = true;
    {
        int i = 5;
        i = !i;
    }
    std::cout << i;
}
```

### Ответ:
- `⛔️ a. 5`
- `⛔️ b. Ошибка`
- `⛔️ c. false`
- `✅ d. 1`
- `⛔️ e. true`
- `⛔️ f. 0`

13) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int main() {
    const int i = 1;
    {
        int i[i] = {};
    }
    std::cout << i;
}
```

### Ответ:
- `⛔️ a. 5`
- `⛔️ b. Ошибка`
- `⛔️ c. false`
- `✅ d. 1`
- `⛔️ e. true`
- `⛔️ f. 0`

14) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int i = 1;
int main() {
    int i = 1;
    std::cout << i;
}
```

### Ответ:
- `⛔️ a. Ошибка`
- `✅ b. 1`

15) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int i = 1;

namespace A {
    namespace B {
        void print() {
            std::cout << i;
        }
    }
}

int main() {
    A::B::print();
}
```

### Ответ:
- `⛔️ a. Ошибка`
- `✅ b. 1`

16) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    std::cout << i;
    int i = 2;
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 1`

17) Язык Go. Код программы написан полностью в одном файле. Какое имя пакета должно быть указано в начале файла.


### Ответ:
- `⛔️ a. Любое имя пакета`
- `✅ b. main`
- `⛔️ c. executable`
- `⛔️ d. В Go не используются пакеты`
- `⛔️ e. include`

18) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int A = 1;

int A(){
    return 2;
}

int main() {
    std::cout << A();
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 1`

19) Дан фрагмент кода на Go. Что будет напечатано в результате его выполнения?

```go
package main
import "fmt"

func main() {
    fmt.Print(i)
}

var i int = 1
```

### Ответ:
- `⛔️ a. Ошибка`
- `✅ b. 1`

20) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    std::cout << i;
}
```

### Ответ:
- `✅ a. Ошибка`
- `⛔️ b. 1`

21) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int i = 1;

namespace C{
    int i = 2;
}

namespace A {
    namespace B {
        void print() {
            std::cout << i;
        }
    }
    int i = 3;
}

int main() {
    A::B::print();
}
```

### Ответ:
- `⛔️ a. 2`
- `⛔️ b. Ошибка`
- `✅ c. 1`
- `⛔️ d. 3`

22) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
void A(){
    std::cout << i;  
}

int i = 1;

int main() {
    A();
}
```

### Ответ:
- `✅ a. Ошибка`
- `⛔️ b. 1`

23) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    int i = 2;
    std::cout << i;
}
```

### Ответ:
- `✅ a. 2`
- `⛔️ b. Ошибка`
- `⛔️ c. 1`

23) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int main(){
    const int i = 1;
    {
        int i = i;
        std::cout << i;
    }
}
```

### Ответ:
- `✅ a. Мусор. Т.к. i неинициализированная переменная`
- `⛔️ b. 1`
- `⛔️ c. true`
- `⛔️ d. false`
- `⛔️ e. 0`
- `⛔️ f. 5`

25) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    using A::i;
    std::cout << i;
    int i = 2;
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 1`

26) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    using namespace A;
    int i = 2;
    std::cout << i;
}
```

### Ответ:
- `✅ a. 2`
- `⛔️ b. Ошибка`
- `⛔️ c. 1`

27) Язык Go. Пакет импортирован следующим образом:

`import . "github.com/vigo5190/example/name"`

Каким образом можно использовать экспортируемые имена из этого пакета в своём коде?

### Ответ:
- `✅ a. Имена объявленные в пакете name доступны для использования просто по своему имени`
- `⛔️ b. Имя из пакета name можно использовать так: name.требуемое_имя`
- `⛔️ c. Имя из пакета name можно использовать так: example.требуемое_имя`
- `⛔️ d. Имена объявленные в пакете name НЕ доступны для использования`

28) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int i = 1;

namespace C{
    int i = 2;
}

namespace A {
    namespace B {
        using namespace C;
        void print() {
            std::cout << i;
        }
    }
    int i = 3;
}

int main() {
    A::B::print();
}
```

### Ответ:
- `⛔️ a. 2`
- `✅ b. Ошибка`
- `⛔️ c. 1`
- `⛔️ d. 3`

29) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
int i = 1;

namespace A {
    namespace B {
        int i = 2;
        void print() {
            std::cout << i;
        }
    }
}

int main() {
    int i = 3;
    A::B::print();
}
```

### Ответ:
- `✅ a. 2`
- `⛔️ b. Ошибка`
- `⛔️ c. 1`
- `⛔️ d. 3`

30) Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?

```cpp
namespace A{
    int i = 1;
}

int main() {
    using namespace A;
    std::cout << i;
    int i = 2;
}
```

### Ответ:
- `⛔️ a. 2`
- `⛔️ b. Ошибка`
- `✅ c. 1`
