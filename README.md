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

