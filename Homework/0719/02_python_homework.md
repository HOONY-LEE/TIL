1. Mutable & Immutable
주어진 컨테이너들을 각각 변경 가능한 것(mutable)과
변경 불가능한 것(immutable)으로 분류하시오.
String, List, Tuple, Range, Set, Dictionary

mutable : List, Dictionary, Set
immutable : String, Tuple, Range


1. Dictionary 만들기
반 학생들의 정보를 이용하여 key는 이름, value는 나이인 dictionary를 만드시오.
내 자리를 기준으로 앞, 뒤 좌, 우에 앉아 있는 학생의 정보를 참고하시오.

```
student = { '이정범' : 25 , '한기현' : 28, '서지윤' : 24 , '정예지' : 25 }
```


3. 평균 구하기
주어진 list에 담긴 숫자들의 평균값을 출력하시오.

```
scores = [80, 89, 99, 83] # => 8
sum = 0
for i in range(len(scores)):
    sum += scores[i]
avg = sum / len(scores)
print(avg)
```
