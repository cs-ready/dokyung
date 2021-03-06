# Structure 

## 1. 구조체
* 하나 이상의 변수를 묶어서 하나의 새로운 자료형으로 만들어 사용하는 것
* 복잡한 데이터를 표현할 수 있음
* 다양한 타입의 변수 집합을 하나의 타입으로 나타낸 것 (각각은 멤버 변수)
* ex) 학생 정보, 책 정보 등

--- 
## 2. 구조체 정의 선언하기 

```c
struct book //구조체 이름

{

    char title[30];

    char author[30];

    int price;

} my_book; //구조체 변수 이름
```
--- 
## 3. typedef 키워드
*  typedef 키워드를 사용해 이름을 선언하면 struct 키워드를 다시 사용하지 않아도 됨 
* (그렇지 않으면 변수 사용할 때마다 'struct'를 사용하여 구조체임을 명시해야 됨)
> typedef struct 구조체이름 구조체의새로운이름;


* 구조체의 정의와 typedef 선언을 동시에 할 때에는 구조체의 이름을 생략할 수 있음

```c
typedef struct // 구조체 이름 생략
{ 

    char title[30];

    char author[30];

    int price;

} TEXTBOOK; // 여기에서 
```
--- 
## 4. 구조체 멤버로의 접근 
* 구조체에서 구조체 멤버로 접근하려고 할 때  

* > 구조체변수이름.멤버변수이름

---

## 5. 구조체 변수의 초기화
* 구조체 변수를 초기화할 때에는 멤버 연산자(.)와 중괄호({})를 사용함

1. 구조체 변수 초기화 방법 1 
>구조체변수이름 = {.멤버변수1이름 = 초깃값, .멤버변수2이름 = 초깃값, ...};

2. 구조체 변수 초기화 방법 2
> 구조체변수이름 = {멤버변수1의초깃값, 멤버변수2의초깃값, ...};
