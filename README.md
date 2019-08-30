# study-python
just study

파이썬은 인터프리터언어! 공짜! 생산성이 좋음! 초보자 교육에 좋음!
활용-A.i 등등

(o)
>>> print("Hello_World!")
Hello_World!

(x)
>>> Print("Hello_World!")
Traceback (most recent call last):
  File "<pyshell#8>", line 1, in <module>
    Print("Hello_World!")
NameError: name 'Print' is not defined

(o)
>>> ("Hello_World!")
'Hello_World!'

(o)
>>> "Hello_World!"
'Hello_World!'

파이썬의 데이터 type
-숫자->정수=1,실수=1.0,0.3등등

>>> print(123456789)
123456789

사칙연산
더하기 + 뺴기 - 곱하기 * 나누기/
>>> print(1+2)
3

>>> print(3-2)
1

>>> print(2*4)
8

>>> print(6/3)
2.0

>>> print(6/0)
Traceback (most recent call last):
  File "<pyshell#18>", line 1, in <module>
    print(6/0)
ZeroDivisionError: division by zero         -뷉!
  
  >>> print(3*(2+1)-5)
4
-연산에서 우선순위 있음!

제곱** 몫// 나머지%

>>> print(3*(2+1)-5)
4

>>> print(5**2)
25

>>> print(5//2)
2

>>> print(5 % 2)
1

홀수 짝수 구분하기!
-2로 나눈 나머지가 0이면 짝수 1이면 홀수!
>>> print(1%2)
1                   -홀!
>>> print(2%2)
0                   -짝!
>>> print(3%2)
1                   -홀!
>>> print(4%2)
0                   -짝!

문자형에 대한 이야기

>>> print('박보검 잘생겼다')
박보검 잘생겼다

>>> print('12박보검12')
12박보검12

-참고
>>> print('1234')
1234
>>> print(1234)
1234
둘의 값이 같을까?? ㄴㄴ!!!!!!!! *다르다!!!!*
>>> print('12+34')
12+34
>>> print(12+34)
46
요렇듯 문자값과 숫자값으로 다름!

""와'' 의 차이!!!!!

>>> print("얘들이 '공부 좀 했으면..'하고 생각했다.")
얘들이 '공부 좀 했으면..'하고 생각했다.
>>> print('얘들이 '공부 좀 했으면..'하고 생각했다.')
SyntaxError: invalid syntax                           '=EOF!

>>> print('허재 아저씨가 말했다."그거슨 아니지~"')
허재 아저씨가 말했다."그거슨 아니지~"
>>> print("허재 아저씨가 말했다."그거슨 아니지~"")
SyntaxError: invalid syntax                           "=EOF       End OF mark
                                              
변수
-변할 수 있는 수
-값을 저장 할 수 있다.
-사용법 : >>> 변수이름 = 값-> *숫자, 문자 다 들어갈 수 있음.*

변수 이름 짓기!
-원래있는 명령어 같이 이미 있는 이름은 불가능
-문자와 숫자 ,_ 는 사용가능.
-대/소문자 구분
-공백 사용 금지
-숫자로 시작 금지
*이름 사용가능 한지 알아 보려면 쳤을때 색깔 안 입혀지면 됨.*

>>> a = 20
>>> print(a)
20
>>> a = 30
>>> print(a)
30
-변수 선언 한 번 더해주면 나중에 선언한 값으로 저장됨.

1씩 증가시키자!
>>> a= 30
>>> a= a+1
>>> a
31
+번외!
>>> a=50
>>> a=a/2 두구두구두구!
>>> a
25.0 빠밤!

복습!
>>> num=1024
>>> str="수고했어 오늘도!!"
>>> print(3618)          이거 밖에 안했네...ㅋ
 
+파이썬에서 주석!
>>> print('Hello Python')
Hello Python
>>> # print('Hello Python')

나중에 협업이나 그냥 수정 할때 주석을 써서 유용하게 사용하자!(팁:오류 났을 때 주석으로 처리해서 오류난데 찾기!)
