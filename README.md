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

나중에 협업이나 그냥 수정 할때 주석을 써서 유용하게 사용하자!(팁:오류 났을 때 주석으로 처리해서 오류난데 찾기!) _2019/8/30_

_2019/9/27_

tip_ 8421? 이진수
0001 ->1
0010 ->2
0011 ->3

8421
****
1001 -> 9 <- 8+0+0+1

함수!
input : 값을 받아줌
>>> x = input("첫번째 수:")
첫번째 수:9
>>> y = input("두번째 수:")
두번째 수:16
>>> print("합은", x+y)
합은 916
??-인풋은 문자로 받음 그래서!

>>> x = int(input("첫번째 수:"))
첫번째 수:9
>>> y = int(input("첫번째 수:"))
첫번째 수:16
>>> print("합은", x+y)
합은 25
이러면 숫자로 받지~! (int도 함수! 얘가 문자를 숫자로!)

>>> name = input("당신의 이름은?")
당신의 이름은?동준
>>> print("저는"+name+"입니다.")  -> print 안에서 + +기호로 문자랑 섞어서 쓸수 있다!
저는동준입니다.

>>> max(10,20)
20
>>> min(50, 30, 20, 40)
20                                     tip 괄호 여는건 함수!

>>> sqrt(4.0)
Traceback (most recent call last):
  File "<pyshell#11>", line 1, in <module>
    sqrt(4.0)
NameError: name 'sqrt' is not defined           ?? 이건 임포트가 안되어 있거나 진짜 기능이 없는 것이다!

>>> from math import*
>>> sqrt(4.0)
2.0

문자열!~!~!
문자열 연결하기 -> +
-BTS가 UN연설에서 말했다
-LOVE YOURSELF
>>> print('BTS가 UN연설에서 말했다.'+'LOVE YOURSELF')
BTS가 UN연설에서 말했다.LOVE YOURSELF

>>> print('BTS멤버 수는'+7)
Traceback (most recent call last):
  File "<pyshell#16>", line 1, in <module>
    print('BTS멤버 수는'+7)
TypeError: can only concatenate str (not "int") to str
  -문자랑 숫자 안 더해짐! string=문자
그래서! str 쓰자
>>> print('멤버수는'+ str(7))
멤버수는7

문자열 숫자로 변환
>>> age = int("100")
>>> height = float("168.7")

문자열 길이 함수
-len
>>> len("student")
7

문자열 줄바꿈
-BTS는
-쵝오다!
(\n \-이거 돈표시임)
>>> print('BTS는 \n쵝오다!')
BTS는 
쵝오다!     (\-돈표시는 이스케이프문자!)

문자열 특수문자 제외하기! ->r
>>> print(r'C:\admin\download')
C:\admin\download

문자열 반복 -> OR= *
>>> print("="*30)
==============================
>>> equal = "="*30
>>> print(equal)
==============================

문자열의 고급 출력 -> %s
>>> mem = 7
>>> print("BTS는 %s명이다." %mem)
BTS는 7명이다.         여기서! 파이썬은 %mem 앞에 , 안찍음

>>> mem = 7
>>> fan = 75
>>> print("BTS는 %s명이고 팬은 %s억 명이다."%(mem, pan))
BTS는 7명이고 팬은 75억 명이다.

>>> sentence = "BTS는 %s명이고 팬은 %s억 명이다."
>>> print(sentence %(mem, fan))
BTS는 7명이고 팬은 75억 명이다.

문자열 중 문자 하나 추출하기 -> []
-BTS가 짱이야! (에서 s만!)
>>> sent = "BTS가 짱이야!"
>>> sent[2]
'S'
공백출력 해보까?
>>> sent[4]
' '
>>> sent[10]
Traceback (most recent call last):
  File "<pyshell#3>", line 1, in <module>
    sent[10]
IndexError: string index out of range     - 인덱스 넘어가지 마라!
  +파이썬은 문자하나만 못 바꿈

문자열 조합해보기

>>> first = input("첫번째 문자열을 입력하세요:")
첫번째 문자열을 입력하세요:B
>>> second = input("첫번째 문자열을 입력하세요:")
첫번째 문자열을 입력하세요:T
>>> third = input("첫번째 문자열을 입력하세요:")
첫번째 문자열을 입력하세요:S
>>> print(first+second+third)
BTS

>>> first = input("첫번째 문자열을 입력하세요:")
첫번째 문자열을 입력하세요:Beyond
>>> second = input("첫번째 문자열을 입력하세요:")
첫번째 문자열을 입력하세요:Teacher
>>> third = input("첫번째 문자열을 입력하세요:")
첫번째 문자열을 입력하세요:Star
>>> print(first[0]+second[0]+third[0])
BTS

인덱스!!

>>> 오늘뭐먹지 = ['우삼겹', '계란찜', '쌈채소', '된장찌개']
>>> 오늘뭐먹지
['우삼겹', '계란찜', '쌈채소', '된장찌개']
>>> 오늘뭐먹지[0]
'우삼겹'
>>> 오늘뭐먹지[3]
'된장찌개'
- 얘는 리스트 중 항목 하나만 변경가능
>>> 오늘뭐먹지[1] = '계란말이'
>>> 오늘뭐먹지[1]
'계란말이'

다양한 조건물들! - 맛보기!
>>> value = 90
>>> if(value >=80):
	print("마스크를 쓰세요")
else:
	print("미세먼지 지수가 좋습니다")

	
마스크를 쓰세요

_2019-10-25_ 
오늘!! 다양한 조건문들!

: -> 은 아직 문장 안 끝났다는 거! 
참고: 조건문을 쓸 때 들여쓰기 주의 하시오!!! 안그럼 에러뜹니다!
조건문에 else없어도 사용가능!

관계연산자 
== 같은가?
!= 다른가?
>  큰가?
<  작은가?
>= 이상
<= 이하

그럼 TRUE VS FALSE ?
>>> 1 == 1
True
>>> 1 != 2
True
>>> 1 >= 5
False

>>> 'Apple' == 'apple'
False
>>> 'Apple' == 'Apple'
True
>>> 1 == '1.0'
False

>>> val=10
>>> val>=5
True

>>> score = 95
>>> if score >= 90 :
	print('뚜뚠 가수!!')

	
뚜뚠 가수!!
----1---
number = int(input('숫자를 입력하세요!'))
num = number%2

if num == 0:
    print("짝수 입니다")
else:
    print("홀수입니다")
----2---
number = int(input('숫자를 입력하세요!'))

if ((number %2)==0):
    print("짝수 입니다")
else:
    print("홀수입니다")

2번째께 메모리를 덜 씀..

점수 등급표 만들어 보기!!

score = int(input('점수를 입력하세요!'))

if score >= 90:
    print("A 입니다")
elif score >= 80:
    print("B 입니다")
elif score >= 70:
    print("C 입니다")
elif score >= 60:
    print("D 입니다")
elif score >= 50:
    print("E 입니다")
else :
    print("F 입니다")

이중 if문 사용!!
rain = int(input('강수량을 입력하세요!'))

if rain >0 :
    if rain >=50:
        print("우비 준비는 필수!")
    else :
        print("우산 챙기기!")
else :
    print("맘 편히~ 외출~!")


논리연산자!!
A and B
A or B
not A - 만약 연산자로 나온 값이 false가 나오면 not때문에 true값으로 나옴!

num = int(input('정수를 입력하세요!'))

if num >= 0 and num == 0:
    print("이 수는 0입니다")
elif num > 0:
    print("이 수는 양수 입니다")
else :
    print("이 수는 음수 입니다")


Finally!!!!  id랑 pw입력 받고 일치여부 확인 프로그램 만들기!

users = ['choi','lee','kim']
id = input('아이디를 입력하세요!')

if id in users:
    pw=input('비밀번호를 입력해주세용')
    if pw == '1111':
        print("사용자가 맞습니다")
    else:
        print("비밀번호가 틀렸습니다")
else:
    print("입력된 사용자가 아닙니다!!")
    
업그레이드 버전!!

users = ['choi','lee','kim']
pws = ['1111','2222','3333']

id = input('아이디: ')
if id in users:
    pw=input('비밀번호: ')
    if pw in pws :
        print("사용자가 맞습니다")
    else:
        print("비밀번호가 틀렸습니다")
else:
    print("입력된 사용자가 아닙니다!!")


2019/11/15

다양한 반복문!!
for vs while
for 정해진 횟수 만큼 반복
while 조건이 만족될 때까지 반복

for 변수 in 시퀀스:
    반복할 문장

이제부턴 newfile로 만든다음에 저장하고 F5눌러서 테스트 하기!!
for fruit in ["바나나","사과","배","감"]:
	print("과일이름:" +fruit)
F5누르면!!

과일이름:바나나
과일이름:사과
과일이름:배
과일이름:감

그리고 숫자 나열
for number in [0,1,2,3,4,5,6,7,8,9]:
	print(number)
-F5!!!-
0
1
2
3
4
5
6
7
8
9
다른 버젼~!
for number in [0,1,2,3,4,5,6,7,8,9]:
	print(number,end="")
-F5!-
0123456789

for num in [0,1,2,3,4,5,6,7,8,9]:
	print("정수 %d 입니다." %num)
--F5--
정수 0 입니다.
정수 1 입니다.
정수 2 입니다.
정수 3 입니다.
정수 4 입니다.
정수 5 입니다.
정수 6 입니다.
정수 7 입니다.
정수 8 입니다.
정수 9 입니다.


for num in [0,1,2,3,4,5,6,7,8,9]:
	print("%d번째 값 정수 %d 입니다." %(num+1,num))
-F5!!-
1번째 값 정수 0 입니다.
2번째 값 정수 1 입니다.
3번째 값 정수 2 입니다.
4번째 값 정수 3 입니다.
5번째 값 정수 4 입니다.
6번째 값 정수 5 입니다.
7번째 값 정수 6 입니다.
8번째 값 정수 7 입니다.
9번째 값 정수 8 입니다.
10번째 값 정수 9 입니다.

range()함수?

--------range(숫자)-얘는 -1까지 출력 해 줌

for num in range(10):
	print(num)
0
1
2
3
4
5
6
7
8
9
-------range(start,stop)

for num in range(0,10):
	print(num)       0세서 9까지
0
1
2
3
4
5
6
7
8
9 

-활용!

sum=0

for num in range(1,11):
  sum = sum+num
print(sum)

-F5-
55

-------range(start,stop,step)

for num in range(0,10,2):
    print(num)
-F5-
0
2
4
6
8

---문자!
for cha in "abcde":
    print(cha, end=" ")
-F5-
a b c d e 

--------while

i = 0
while i<10:
    print(i)
    i = i + 1
    
0
1
2
3
4
5
6
7
8
9

while로 구구단 5단 출력!!

i = 1
while i<10:
    print("5*%d = %d" %(i,5*i))
    i = i + 1
-F5-
5*1 = 5
5*2 = 10
5*3 = 15
5*4 = 20
5*5 = 25
5*6 = 30
5*7 = 35
5*8 = 40
5*9 = 45

