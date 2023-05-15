# 42-ft_printf

42-ft_printf는 42 Seoul의 과정에서 진행되는 프로젝트로, C 프로그래밍 언어를 사용하여 `printf` 함수를 `write`와 `malloc`만을 사용하여 구현하는 것을 목표로 합니다. 이 프로젝트에서는 출력 형식을 처리하고, 서식 지정자와 옵션을 지원하여 다양한 출력 기능을 제공합니다.

## 주요 특징

- `printf` 함수의 재구현: 42-ft_printf는 C 표준 라이브러리에 포함된 `printf` 함수를 `write`와 `malloc`만을 사용하여 직접 구현합니다. 이를 통해 출력 형식의 처리 방식과 서식 지정자의 동작 원리를 이해할 수 있습니다.
- `write`와 `malloc`의 활용: 42-ft_printf는 출력을 위해 저수준의 시스템 콜인 `write`를 사용하고, 메모리 할당을 위해 `malloc`을 사용합니다. 이를 통해 C 프로그램에서의 입출력 작업과 메모리 관리에 대한 이해를 높일 수 있습니다.
- 다양한 서식 지정자 지원: 42-ft_printf는 `%d`, `%s`, `%c`, `%x` 등 다양한 서식 지정자를 지원하여 정수, 문자열, 문자, 16진수 등의 데이터를 원하는 형식으로 출력할 수 있습니다.
- 옵션 및 변환 지정자 제공: 서식 지정자에 옵션과 변환 지정자를 사용하여 출력의 정밀도, 너비, 정렬 등을 제어할 수 있습니다.

## 사용 방법

1. 프로젝트를 클론합니다:

```shell
git clone https://github.com/hyuntall/42-ft_printf.git
```

2. 프로젝트 폴더로 이동합니다:

```shell
cd 42-ft_printf
```

3. `libftprintf.a`라는 라이브러리 파일을 컴파일합니다:

```shell
make
```

4. 컴파일된 라이브러리를 사용하여 프로젝트를 개발하실 수 있습니다. 필요한 헤더 파일은 `ft_printf.h`에 정의되어 있습니다.

5. `ft_printf()` 함수를 호출하여 원하는 형식의 출력을 수행할 수 있습니다. 서식 지정자와 옵션을 사용하여 출력을 제어할 수 있습니다.

## 사용 예시
```C
#include "ft_printf.h"

int main() {
    ft_printf("Hello, %s!\n", "world");
    ft_printf("The answer is %d.\n", 42);
    return 0;
}
```



## 참고 사항

- 42-ft_printf는 42 Seoul의 과정에서 요구되는 프로젝트로, 특정한 규칙과 제약 사항을 따르고 있습니다.
