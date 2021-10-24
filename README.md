# 20211024_-

47.7. 실수 값이 서로 같은지 판단하기
  - 부동 소수점 반올림 오차(rounding error)
  
  >>> import math, sys
  >>> x = 0.1 + 0.2
  >>> math.fabs(x - 0.3) <= sys.float_info.epsilon
  True
  
  >>> round(x, 0) == 0.3


5.2.2. 값을 실수로 만들기
  >>> float(숫자)
  >>> float(계산식)
  >>> float('문자열')
  
  * 값을 정소루 만들기
  >>> int(숫자)
  >>> int(계산식)
  >>> int('문자열')
  
  6.1.1. 변수의 자료형 알아내기
  >>> type(변수)
  >>> 변수이름1, 변수이름2, 변수이름3 = 값1, 값2, 값3
  
  * 변수 삭제하기
  >>> x = 10
  >>> del x
  
  * 빈 변수 만들기
  >>> x = None
  
  * 부호 붙이기: +를 붙이면 값에 변화가 없고, -를 붙이면 부호가 바뀜.
  >>> x = -1
  >>> +x
  -1
  >>> -x
  1
  
6.3. 변수 입력 받기
 >>> x = input()
 
 >>> a = input('첫 번째 숫자를 입력하세요:')
 >>> b = input('두 번째 숫자를 입력하세요:')
 >>> print(a+b)
 
 * input으로 입력받은 값은 항상 '문자열'임. 

변수1, 변수2 = input('문자열').split('기준문자열')
>>> a, b = input('숫자 두 개를 입력하세요:').split()

>>> a, b = map(int, input('숫자 두 개를 입력하세요:').split(','))
숫자 두 개를 입력하세요: 10,20(입력)
30

6.6. 연습문제
  >>> a, b, c = map(int, input().split())

#Unit7 출력방법
7.1. 값을 여러 개 출력하기
  >>> print(값1, 값2, 값3)
  >>> print(변수1, 변수2, 변수3)

  >>> print('Hello', 'Python')
  Hello Python  # 공백으로 띄워짐
  
  >>> print(1, 2, 3, sep=', ')
  1, 2, 3       # ', '로 띄워짐
  
  >>> print('1/n2/n3')    # print(1, 2, 3, sep'\n')과 같음 
                          # \n은 문자열
                          
* 제어문자
  \n: 다음 줄로
  \t: 탭 문자
  \\: \ 문자 자체를 출력할 때는 \를 두 번 쳐야 한다

7.2. end 사용하기
  >>> print(1)
  >>> print(2)
  >>> print(3)
  1
  2
  3
  
  print(값, end='문자 또는 문자열')
  print(변수, end='문자 또는 문자열')
  
  >>> print(1, end='')    # end에 빈 문자열 할당
  >>> print(2, end='')
  >>> print(3, end='')

7.4. 연습문제
  >>> year = 2021
  >>> month = 10
  >>> day = 24
  >>> hour = 14
  >>> minute = 58
  >>> second = 59
  >>> print(year, month, day, sep='/', end=' ')
  >>> print(hour, minute, second, sep=':')

  
  
