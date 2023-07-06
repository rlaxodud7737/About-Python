아래의 글은 유튜브 "조코딩"님의 강의를 바탕으로 정리한 글입니다.
https://youtu.be/KL1MIuBfWe0  
https://wikidocs.net/book/1
# 점프 투 파이썬 

## 1장. 파이썬이란 무엇인가?

### 파이썬 이란?

파이썬은 컴퓨터 프로그래밍 교육 뿐만 아니라 기업에 실무에서도 자주 사용 되는 언어로 
구글,인스타그램,넷플릭스,아마존 등 우리가 아는 대형 IT 기업들이 사용하는 언어이다.

파이썬은 공동 작업과 유지 보수가 매우 쉽고 편리한데 이로 인해 사용자층이 넓어지고 있고,
다른 언어로 작성된 프로그램이 파이썬으로 재구성 되는 경우가 많다고 한다.

### 파이썬의 특징

#### 파이썬은 인간다운 언어이다.
파이썬은 "사람이 생각하는 방식을 그대로 표현할 수 있는 언어" 이다. 
따라서 컴퓨터의 사고 체계에 맞추어 생각해야 할 필요가 없고 나의 생각을 있는 그대로 표현할 때
가장 적합한 언어라고 할 수 있다.

#### 문법이 쉽다.
파이썬의 문법은 사람의 사고체계와 매우 닮아 있기에 배우고 활용하는데에도 매우 쉽다.

#### 무료 하지만 강력하다.
* 파이썬은 '오픈 소스' 이므로 무료이다.

* '시스템 프로그래밍' 이나 '하드웨어 제어' 같은 복잡하고 반복 연산이 많은 프로그램을 파이썬으로 작성하기에는 힘들다.
하지만 파이썬은 다른 언어로 만든 프로그램을 자신의 프로그램에 포함시킬 수 있기에 간단하면서도 강력한 프로그램이라 할 수 있다.
또한 파이썬과 'C' 언어의 조합은 환상적인데, 프로그램의 뼈대는 파이썬으로 만들고 빠른 실행 속도는 C언어가 담당하여 
최적의 프로그램을 만들 수 있다.

#### 간결하며 개발 속도가 빠르다.
"Life is too short, You need Python."

### 파이썬으로 무엇을 할 수 있을까?

#### 할 수 있는 일 
웹 프로그래밍, 인공지능과 머신러닝, 수치 연산 프로그래밍, 데이터 분석, 데이베이스 프로그래밍, 시스템 유틸리티 제작, GUI 프로그래밍, C/C++ 와 결합, 사물 인터넷

#### 할 수 없는 일
시스템과 밀접한 프로그래밍 영역, 모바일 프로그래밍

## 2장. 파이썬 프로그래밍의 기초, 자료형
### 숫자형
#### 정수형
#### 실수형
#### 8진수
```
(숫자0) + (알파벳 소문자 o 또는 알파벳 대문자 O)  
    a = 0o117  
    print(a)  
    127
```
#### 16진수
```
(숫자0) + (알파벳 소문자 x)  
    b = 0xABC  
    print(b)  
    2748
```
#### x의 y제곱을 나타내는 '**' 연산자
    a = 3  
    b = 4  
    a ** b  
    81
#### 나눗셈 후 나머지를 리턴하는 '%' 연산자
    7 % 3  
    1
#### 나눗셈 후 몫을 리턴하는 '//' 연산자
    7/4  
    1.75  
    7//4  
    1
### 문자열 자료형
_따옴표로 둘러싸였으면 모두 문자열!_  
문자열 자료형 예시
```
"Life is too shrot, You need Python."
"a"
"123"
```
#### 문자열을 만드는 4가지 방법
1. 큰따옴표로 둘러싸기
   ```
   "Hello World"
   ```
2. 작은따옴표로 둘러싸기
   ```
   'Hello World'
   ```
3. 큰따옴표 3개를 연속으로 써서 둘러싸기
   ```
   """Hello World"""
   ```
4. 작은따옴표 3개를 연속으로 써서 둘러싸기
   ```
   '''Hello World'''
   ```
#### 문자열 안에 작은따옴표 or 큰따옴표를 포함시키고 싶을 때
1. 문자열에 작은따옴표 포함하기
   -> 큰 따옴표를 마진에
   ```
   ex) food = "Python's favorite food is perl"
   ```
2. 문자열에 큰따옴표 포함하기
   -> 작은 따옴표를 마진에
   ```
   ex) say = '"Python is very easy." he says.'
   ```
3. 역슬래시 사용
   ```
   ex) food = 'Python\'s favorit food is perl'
   ex) say = "\"Python is very easy.\" he says."
   ```
#### 문자열이 여러줄인 경우
1. '\n' 사용
   ```
   ex) multiline = "Life is too short\nYou need python"
   ```
2. 작은 따옴표 3개 or 큰 따옴표 3개
   ```
   ex) multiline = '''  
       Life is too short  
       You need python  
       '''
   ```
   ```
   ex) multiline = """
       Life is too short
       You need python
       """
   ```

print(multiline) 입력시
```
Life is too short  
You need python
```
#### 문자열 연산하기
* 문자열 더해서 연결하기
  ```
  head ="Python"  
  tail =" is fun!"  
  total = head + tail  
  print(total)  
  --> Python is fun!
  ```
* 문자열 곱하기
  ```
  a = "python"  
  print(a*2)  
  --> pythonpython
  ```
* 문자열 곱하기 응용
  ```
  print("="*50)
  print("My Program")
  print("="*50)
  -->
  =================================================(50개)
  My Program
  =================================================(50개)
  ```
#### 문자열 길이 구하기
  'len' 함수
  ```
  a = "Life is too short"
  len(a)
  -> 17
  ```
#### 문자열 인덱싱과 슬라이싱
  * 문자열 인덱싱
    ```
    a = "Life is too short, You need Python"
    ```
    위 코드에서 변수 'a' 에 저장한 문자열의 각 문자마다 번호를 매겨보면 다음과 같다.
    ![image](https://github.com/rlaxodud7737/About-Python/assets/129059558/0f2902d0-3c5b-4f1b-b32b-748f4288a117)
    ```
    a = "Life is too short, You need Python"
    print(a[3])
    --> e
    ```
    **"파이썬은 0부터 숫자를 센다."**
  * 문자열 인덱싱 활용하기  
    인덱스 중 '-1'은 '뒤'에서 첫 번째 문자의 인덱스 번호이다.  
    _0 = -0_
    ```
    a = "Life is too short, You need Python"
    print(a[0])
    --> L
    print(a[12])
    --> s
    print(a[-1])
    --> n
    ```
 * 문자열 슬라이싱  
   원초적인 방법
   ```
   a = "Life is too short, You need Python"
   b = a[0] + a[1] + a[2] + a[3]
   print(b)
   --> Life
   ```
   슬라이싱 기법
   ```
   a = "Life is too short, You need Python"
   print(a[0:4])
   --> Life
   ```
   이 때, a[0:4] 의 의미는 다음과 같다.
   ```
   0 <= a < 4
   ```
   슬라이싱 기법 응용('print' 생략)
   ```
   a[0:5]
   --> 'Life '
   a[5:7]
   --> 'is'
   a[12:17]
   --> 'short'
   ```
   끝번호 생략(시작번호 ~ 문자열 끝)
   ```
   a[19:]
   --> 'You need Python'
   ```
   시작번호 생략(문자열 첨 ~ 끝 번호)
   ```
   a[:17]
   --> 'Life is too short'
   ```
   시작번호, 끝 번호 생략(전체)
   ```
   a[:]
   --> 'Life is too short, You need Python'
   ```
   -(빼기) 기호 사용
   ```
   a[19:-7]
   --> 'You need'
   ```
   a[19:-7] 은 a[19]에서 a[-8] 까지를 의미한다.(a[-7]은 포함X)
   ```
   a = "20230331Rainy"
   year = a[:4]
   date = a[4:8]
   weather = a[8:]
   --> year = 2023
   --> day = 0331
   --> weather = Rainy
   ```
   **"Pithon" 문자열을 "Python" 으로 바꾸려면?**
   잘못된 예시
   ```
   a = "Pithon"
   a[1] = 'y'
   ```
   *문자열의 요솟값은 바꿀 수 없다!*
   올바른 예시
   ```
   a = "Pithon"
   new_a = a[:1] + 'y' + a[2:]
   --> 'Python'
   ```
#### 문자열 포매팅
   ```
   "현재 온도는 18도 입니다."
   "현재 온도는 20도 입니다."
   ```
   이처럼 문자열 안의 특정한 값을 바꿔야하는 경우가 있는데 이것을 가능케 하는것이
   '문자열 포매팅' 이다. 문자열안에 어떤 값을 삽입하는 방법.  
#### 문자열 포매팅 따라하기
1. 숫자 바로 대입
   ```
   "I eat %d apples." %3
   --> I eat 3 apples.
   ```
2. 문자열 바로 대입
   ```
   "I eat %s apples." % "five"
   --> I eat five apples.
   ```
3. 숫자 값을 나타내는 변수로 대입
   ```
   number = 3
   "I eat %d apples." % number
   --> I eat 3 apples.
   ```
4. 2개 이상의 값 넣기
   ```
   number = 10
   day = "three"
   "I ate %d apples. so I was sick for %s days." %(number,day)
   --> I ate 10 apples. so i was sick for three days.
   ```
#### 문자열 포맷 코드
|코드|설명|
|:----|:--------------|
|%s|문자열(string)|
|%c|문자 1개(character)|
|%d|정수(integer)|
|%f|부동소수(floating-point)|
|%o|8진수|
|%x|16진수|
|%%|Literal %(문자 % 자체)|

여기서 '%s' 는 어떤 코드든 상관 없이 변환 가능하다.
```
"I have %s apples" % 3
--> I have 3 apples.
"rate is %s" % 3.234
--> rate is 3.234
```
'%s' 는 자동으로 '%' 뒤에 있는 값(3 or 3.234) 를 문자열로 바꾸어 대입한다.
   

    
  
  

   
   










