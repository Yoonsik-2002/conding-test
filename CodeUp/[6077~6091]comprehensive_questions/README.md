# [코드업 100제] 종합 문제 - 6081
[문제 링크](https://codeup.kr/problem.php?id=6081)

16진수 구구단 - `A`, `B`, `C`, `D`, `E`, `F`중, 하나가 입력될 때, `1`부터 `F`까지 곱한 16진수 구구단의 내용 출력하기<br>

- ###### 문자열 표맷팅이란?
  문자열 포맷팅은 문자열 안에 변수나 값을 삽입하여 원하는 형식으로 출력하는 방법이다.<br>
  python에서의 가장 일반적인 문자열 포맷팅 방법은 `%`연산자를 사용하는 방법과 `format()`메서드를 사용하는 방법이 있다.

  - ###### `%`연산자를 사용한 문자열 포맷팅
    문자열 안에 `%`을 사용하여 포맷 코드를 지정하고, 해당 포맷 코드에 맞는 값을 변수나 값의 형태로 전달한다.<br>
    ex)
    `print('%d'%3.5) # 3`<br>
    `print('%s'%'Hello) # Hello`<br>
    `print('%X'%10) # A`<br>

  - ###### `format()`메서드를 사용한 문자열 포맷팅
    format() 메서드를 사용한 문자열 포맷팅에서는 중괄호 {}를 사용하여 변수나 값을 표시하고, format() 메서드를 호출할 때 인자로 전달한다.<br>
    ex)
    `"Hello, {}!".format("World") # "Hello, World!"`<br>
    `"Hello, {}!".format("World") # "Hello, World!"`<br>
<br>

`%` 연산자를 이용한 문자열 포맷팅을 통해 문제를 해결해 보면 다음과 같다.<br>
```python
n = int(input(), 16) # 입력된 16진수값을 10진수로 변환하여 변수 n에 저장

if(n < 10 & n > 15):
  exit()
else:
  for i in range(1, 16):
    print('%X'%n, '*%X='%i, '%X'%(n*i), sep='') #,을 기준으로 한 각 요소를 구분자 없이 이어서 출력
```
<br>

해당 코드의 실행 결과는 아래와 같다.<br>

![스크린샷(2)](https://github.com/Yoonsik-2002/coding-test/assets/83572199/9acae075-34cd-483a-bdda-19b1f395b8b3)<br>

---

<br><br>



    
