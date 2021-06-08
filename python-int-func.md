### 2021.06.08 Python Int 함수

# n진법으로 표기된 string을 10진법 숫자로 변환하기

## 문제. `base`진법으로 표기된 숫자를 10진법 숫자 출력해보세요

## 문제풀이. python에는 int()함수가 있다. 단순히 문자열을 int형식으로 바꾸는 기능도 하지만, 뒤에 조건(base)을 입력해주면 그 진수로 변환해주는 역할도 한다.

```py
num, base = map(int, input().strip().split(' '))
output = int(str(num), int(base))
print(output)
```
