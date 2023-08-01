# Python Study
Markdown을 사용해서 python study 해보자

목차

* Python 기초
----
> Python은 인터프리터 언어라서 간단하지만 느린 언어다.<br>
> 복잡하지만 빠른 C언어와 호환이 가능하며 C언어는 컴파일러 언어다.
----

1. 숫자 자료형

print(5)
print(-10)
print(3.14)
print(1000)
print(5+3)

2. 문자열 자료형

print('풍선')
print("나비")
print("ㅋㅋㅋㅋㅋㅋㅋㅋ")
print("ㅋ"*9)

3. Boolean 자료형


print(True)
print(False)
print(not True)
print(not False)
print(not (5>10))

1. 변수
animal = "강아지"
name = "연탄이"
age = 4
hobby = "산책"
is_adult = age >= 3

print("우리집 " + animal + "의 이름은 " + name + "이예요")
#print(name , "는 " , age , "살이며, " , hobby , "을 아주 좋아해요")  ; **+ 대신 콤마(,)를 사용 할수 있으며 콤마 사용시 str변수 사용 하지 않아도 되며 변수 뒤에 띄워쓰기 1회 추가됨** <br>
print(name + "는 " + str(age) + "살이며+ " + hobby + "을 아주 좋아해요")
 print(name + "는 어른일까요? " + str(is_adult))

1. 주석
#한줄
''' 여러문장 주석처리<br>
가능합니다.<br>
'''

여러 문장 선택후 ctrl + / 동시에 입력 하면
#여러문장 주석처리
#가능합니다.

# Quiz) 변수를 이용하여 다음 문장을 출력하시오

# 변수명 
# : station
# 변수값 
# : "사당", "인천공항", "신도림"
# 출력 문장 
# : XX 행 열차가 들어오고 있습니다. 

station = "사당"
print(station,"행 열차가 들어오고 있습니다.")

1. 연산자

print(1+1) # 2
print(3-2) # 1
print(5*2) # 10

print(2**3) # 2^3 = 8
print(5%3) # 나머지 구하기 2
print(10%3) # 나머지 구하기 1

print(5//3) # 몫 구하기 
print(10//3) # 3

print(10 >3) # True
print(4 >= 7) # False
print(10 <3) # False
print(5 <= 5) # True

print(3 == 3) #같다/다르다 True
print(4 == 3) # False
print(3 + 4 == 7) # True

print(1 != 3) # 같지 않다 True
print(not(1 != 3)) #not은 반대를 의미 False
print(1 != 1) # False

# And 조건은 둘다 True여야 True return
print((3 > 0) and (3 < 5)) # True
print((3 > 0) & (3 <5)) # True
# Or 조건은 둘중 하나가 True면 True return
print((3 > 0) or (3 > 5)) # True
print((3 > 0) | (3 > 5)) # True

print(5 > 3 > 2) # True
print(5 > 4 < 7) # False

1. 간단한 수식
print(2 + 3 * 4) # 14
print((2 + 3) * 4) # 20
number = 2 + 3 * 4 # 14
print(number)
number = number + 2 # 16
# number += 2 =16
print(number)
number += 2 # 18
print(number)
number *= 2 # 36
print(number)
number /= 2 # 18
print(number)
number -= 2 # 16
print(number)
# 나머지 구하기
number %= 2 # 0
print(number)

1. 숫자 처리 함수

print(abs(-5)) # 5 절대값
print(pow(4, 2)) # 16 제곱
print(max(5, 12)) # 12 최대값
print(min(5, 10)) # 5 최소값
print(round(3.14)) # 3 반올림
print(round(4.99)) # 5 반올림

1. 연산자 함수
from math import *
print(floor(4.99)) # 4 내림
print(ceil(3.14)) # 4 올림
print(sqrt(16)) # 4 제곱근

1. 랜덤 함수

# from random import *
# print(random()) # 0.0 ~ 1.0 미만의 임의의 값 생성
# print(random() * 10) # 0.0 ~ 10.0 미만의 임의의 값 생성

# print(int(random()*10)) # 0.0 ~ 10.0 미만의 임의의 값(정수) 생성
# print(int(random()*10)) # 0.0 ~ 10.0 미만의 임의의 값(정수) 생성
# print(int(random()*10)) # 0.0 ~ 10.0 미만의 임의의 값(정수) 생성

# print(int(random()*10)+1) # 1.0 ~ 10.0 미만의 임의의 값(정수) 생성
# print(int(random()*10)+1) # 1.0 ~ 10.0 미만의 임의의 값(정수) 생성
# print(int(random()*10)+1) # 1.0 ~ 10.0 미만의 임의의 값(정수) 생성

from random import *
# print(int(random() * 44) + 1) # 1 ~ 45 이하의 임의의 값 생성 , 로또
# print(int(random() * 44) + 1) # 1 ~ 45 이하의 임의의 값 생성 , 로또
# print(int(random() * 44) + 1) # 1 ~ 45 이하의 임의의 값 생성 , 로또
# print(int(random() * 44) + 1) # 1 ~ 45 이하의 임의의 값 생성 , 로또
# print(int(random() * 44) + 1) # 1 ~ 45 이하의 임의의 값 생성 , 로또
# print(int(random() * 44) + 1) # 1 ~ 45 이하의 임의의 값 생성 , 로또

print(randrange(1, 46)) # 1 ~ 46 미만의 임의의 값 생성

print(randint(1, 45)) # 1 ~ 45 이하의 임의의 값 생성

# Quiz) 당신은 최근에 코딩 스터디 모임을 새로 만들었습니다.
# 월 4회 스터디를 하는데 3번은 온라인으로 하고 1번은 오프라인으로 하기로 했습니다.
# 아래 조건에 맞는 오프라인 모임 날짜를 정해주는 프로그램을 작성하시오.

# 조건 1 : 랜덤으로 날짜를 뽑아야 함
# 조건 2 : 월별 날짜는 다름을 감안하여 최소 일수인 28 이내로 정함
# 조건 3 : 매월 1~3일은 스터디 준비를 해야 하므로 제외

# (출력문 예제)
# 오프라인 스터디 모임 날짜는 매월 x 일로 선정 되었습니다.

from random import *
study_day = randint(4,28)
print("오프라인 스터디 모임 날짜는 매월" , study_day , "일로 선정 되었습니다.")

1. 문자열
sentence = '나는 소년입니다'
print(sentence)

sentence2 = "파이썬은 쉬워요"
print(sentence2)

sentence3 = """
나는 소년이고,
파이썬은 쉬워요
"""

print(sentence3)

1. 슬라이싱


jumin = "890610-1151223"

print("성별 : " + jumin[7]) # 7번째 숫자 인덱싱
print("연 : " + jumin[0:2]) # 0 ~ 2 직전까지 인덱싱 (0,1)
print("월 : " + jumin[2:4]) # 2 ~ 5 직전까지 인덱싱 (2,3)
print("일 : " + jumin[4:6]) 
print("생년월일 : " + jumin[:6]) # 처음부터 6 직전까지 인덱싱 
print("뒤 7자리 : " + jumin[7:]) # 7번째부터 끝까지 인덱싱

print("뒤 7자리 (뒤에부터) : " + jumin[-7:])


문자열 처리함수


python = "Python is Amazing"


print(python.lower())
print(python.upper())
print(python[0].isupper()) # True
print(len(python)) # count
print(python.replace("Python", "Java")) # 치환

index = python.index("n")
print(index)
index = python.index("n", index + 1)
print(index)

print(python.find("Java")) # 원하는 값이 없을때 -1 return
#print(python.index("Java")) # 원하는 값이 없으면 프로그램 종료
print("hi")

print(python.count("n")) # n이 몇개?



문자열 포멧

#print("a" + "b")
#print("a" , "b") # 콤마를 사용할 경우 띄어쓰기



# 방법 1
print("나는 %d살입니다." % 20) # d는 정수값을 의미합니다.
print("나는 %s을 좋아해요" % "파이썬") # s(str)는 문자열을 의미합니다.
print("Apple 은 %c로 시작해요." % "A") # c(char))는 한글자를 의미합니다.

print("나는 %s살입니다." % 20)
print("나는 %s색과 %s색을 좋아해요." % ("파란", "빨간"))

# 방법 2
print("나는 {}살입니다.".format(20))
print("나는 {}색과 {}색을 좋아해요.".format("빨간","파란"))
print("나는 {1}색과 {0}색을 좋아해요.".format("빨간","파란"))

# 방법 3
print("나는 {age}살이며, {color}색을 좋아해요.".format(age = 20, color = "빨간"))
print("나는 {age}살이며, {color}색을 좋아해요.".format(color = "빨간", age = 20))

# 방법 4 (v3.6 이상~)
age = 20
color = "빨간"
print(f"나는 {age}살이며, {color}색을 좋아해요.")





탈출 문자

print("백문이 불여일견\n백견이 불여일타") # \n 줄바꿈
print('저는 "나도코딩"입니다.')
print("저는 '나도코딩'입니다.")
print("저는 \"나도코딩\"입니다.")



# \\ : 문장 내에서 \
print("C:\\Users\\sh19.park\\Desktop\\python")

# \r : 커서를 맨 앞으로 이동
print("Red Apple\rPine") # PineApple

# \b : 백스페이스 (한 글자 삭제)
print("Redd\bApple")

# \t : 탭
print("Red\tApple")





# Quiz) 사이트별로 비밀번호를 만들어 주는 프로그램을 작성하시오

# 예) http://naver.com
# 규칙1: http:// 부분은 제외 => naver.com
# 규칙2: 처음 만나는 점(.) 이후 부분은 제외 => naver
# 규칙3: 남은 글자 중 처음 세자리 + 글자 갯수 + 글자 내 'e' 갯수 + "!"로 구성
# 예) 생성된 비밀번호 : nav51!

site = "http://naver.com"
rule1 = site[7:]
rule2 = rule1[-9:5]
password = rule2[0:3]
print(password + str(len(rule2)) + str(rule2.count("e")) + "!")

url = "http://naver.com"
my_str = url.replace("http://","") # 규칙1
print(my_str)
my_str = my_str[:my_str.index(".")] # 규칙2
print(my_str)
password = my_str[:3] + str(len(my_str)) + str(my_str.count("e")) + "!"
print("{0}의 비밀번호는 {1}입니다.".format(url,password))




리스트 []


subway = [10, 20, 30]
print(subway)
print(subway.index(20))



subway = ["유재석","조세호","박명수"]
print(subway)
# 조세호씨가 몇 번째 칸에 타고 있는가?
print(subway.index("조세호"))
# 하하씨가 다음 정류장에서 다음 칸에 탐
subway.append("하하") # append "하하"를 리스트에 추가
print(subway)
# 정형돈씨를 유재석 / 조세호 사이에 태워봄
subway.insert(1, "정형돈")
print(subway)
# 지하철에 있는 사람을 한 명씩 뒤에서 꺼냄
print(subway.pop())
print(subway)
# print(subway.pop())
# print(subway)
# print(subway.pop())
# print(subway)
# 같은 이름의 사람이 몇명 있는지 확인
subway.append("유재석")
print(subway)
print(subway.count("유재석"))
# 정렬도 가능
num_list = [5,2,4,3,1]
num_list.sort()
print(num_list)
# 순서 뒤집기 가능
num_list.reverse()
print(num_list)
# 모두 지우기
num_list.clear()
print(num_list)
# 다양한 자료형 함께 사용
num_list = [5,2,4,3,1]
mix_list = ["조세호", 20, True]
#print(mix_list)
# 리스트 확장
num_list.extend(mix_list)
print(num_list)




사전 {딕셔너리}


# {Key:Value}
cabinet = {3:"유재석", 100:"김태호"}
print(cabinet[3])
print(cabinet[100])



print(cabinet.get(3))
# 대괄호로 가져오는경우 Key가 없으면 프로그램 종료되며 get으로 가져오면 Key가 없을때 None 출력
# 5번 키를 사용 가능
print(cabinet.get(5,"사용 가능"))

print(3 in cabinet) # 3이 cabinet안에 있으면 True
print(5 in cabinet) # 5가 cabinet안에 없으면 False

cabinet = {"A-3":"유재석","B-100":"김태호"}
print(cabinet["A-3"])
# 새 손님
# 유재석 -> 김종국으로 replace
cabinet["A-3"] = "김종국"
# 조세호 추가
cabinet["C-20"] = "조세호"
print(cabinet)
# 간 손님
del cabinet["A-3"]
print(cabinet)
# Key 들만 출력
print(cabinet.keys())
# value 들만 출력
print(cabinet.values())
# Key, value 전부 출력
print(cabinet.items())
# 목욕탕 폐점
cabinet.clear()
print(cabinet)

튜플 ()


# 튜플은 목록을 변경 할수는 없지만 리스트보다 처리 속도가 빠르다.
menu = ("돈까스", "치즈까스")
print(menu[0])
print(menu[1])



#menu.add("생선까스") 튜플은 add 할 수 없다.

name = "김종국"
age = 20
hobby = "코딩"
print(name, age, hobby)

(name, age, hobby) = ("김종국", 20, "코딩")
print(name, age, hobby)




교집합 {set}

# 중괄호로 처리 하거나 set(["a","b"]) 설정
# 딕셔너리와 비슷하지만 Key값만 가지고있는 것을 집합이라 함
# 중복 안됨, 순서 없음
my_set = {1,2,3,3,3}
print(my_set)



java = {"유재석","김태호","양세형"}
python = set(["유재석","박명수"])

# 교집합 (java 와 python 을 모두 할 수 있는 개발자)
print(java & python)
print(java.intersection(python))

# 합집합 (java 도 할 수 있거나 python 할 수 있는 개발자)
print(java | python)
print(java.union(python))

# 차집합 (java 할 수 있지만 python 은 할 줄 모르는 개발자)
print(java - python)
print(java.difference(python))

# python 할 줄 아는 사람이 늘어남
python.add("김태호")
print(python)

# java를 까먹었음
java.remove("김태호")
print(java)

# 자료구조의 변경
menu = {"커피", "우유", "주스"}
print(menu, type(menu))
menu = list(menu)
print(menu, type(menu))
menu = tuple(menu)
print(menu, type(menu))
menu = set(menu)
print(menu, type(menu))
# {'주스', '우유', '커피'} <class 'set'>
# ['주스', '우유', '커피'] <class 'list'>
# ('주스', '우유', '커피') <class 'tuple'>
# {'주스', '우유', '커피'} <class 'set'>





# Quiz) 당신의 학교에서는 파이썬 코딩 대회를 주최합니다.
# 참석률을 높이기 위해 댓글 이벤트를 진행하기로 하였습니다.
# 댓글 작성자들 중에 추첨을 통해 1명은 치킨, 3명은 커피 쿠폰을 받게 됩니다.
# 추첨 프로그램을 작성하시오.



# 조건1 : 편의상 댓글은 20명이 작성하였고 아이디는 1~20 이라고 가정
# 조건2 : 댓글 내용과 상관 없이 무작위로 추첨하되 중복 불가
# 조건3 : random 모듈의 shuffle 과 sample 을 활용

from random import *
#reply = int(random() * 20) + 1
reply = range(1,21)
reply = list(reply)
#print(type(reply))
print(reply)
shuffle(reply)
print(reply)
winners = sample(reply, 4) # 1명은 치킨 3명은 커피

# (출력 예제)
# -- 당첨자 발표 --
# 치킨 당첨자 : 1
# 커피 당첨자 : [2,3,4]
# -- 축하합니다. --

print("-- 당첨자 발표 --")
print("치킨 당첨자 : {0}".format(winners[0]))
print("커피 당첨자 : {0}".format(winners[1:]))
print("-- 축하합니다. --")


# (활용 예제)
# from random import *
# lst = [1,2,3,4,5]
# print(lst)
# shuffle(lst)
# print(lst)
# print(sample(lst, 1))












