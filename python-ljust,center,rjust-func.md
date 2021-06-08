### 2021.06.08 Python ljust, center, rjust 함수

# 문자열정렬하기

## 문제. 문자열 s와 자연수 n이 입력으로 주어집니다. 문자열 s를 좌측 / 가운데 / 우측 정렬한 길이 n인 문자열을 한 줄씩 프린트해보세요.

## 문제 풀이. ljust, center, rjust와 같은 `str`메서드를 사용해 for문을 사용하지 않고 코드를 획기적으로 줄여 문자열을 정렬할 수 있다.

```py
s, n = input().strip().split(' ')
n = int(n)

def solution(s):
    print(s.ljust(n)) # 좌측 정렬
    print(s.center(n)) # 가운데 정렬
    print(s.rjust(n)) # 우측 정렬
    return s

solution(s)
```
