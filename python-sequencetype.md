### 2021.06-09 Python sequence type의`*` 연산

# 삼각형 별찍기

## 문제. 이 문제에는 표준 입력으로 정수 n이 주어집니다. 별(*) 문자를 이용해 높이가 n인 삼각형을 출력해보세요.

## 문제 풀이. 파이썬에서는 [123, 456, 123, 456, 123, ...] 과같이 123, 456이 n번 반복되는 리스트 만들기 같이 문자열을 반복해야 할 경우 `*` 연산자를 사용해 코드를 획기적으로 줄일 수 있다. 

```py
n = int(input().strip())
for i in range(1, n+1):
    print('*' * i)

# 내가 푼 풀이
n = int(input().strip())
for i in range(n):
    print('{:<0}'.format('*' * (i+1)))
```
