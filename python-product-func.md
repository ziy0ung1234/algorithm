### 2021.06-10 Python itertools product 함수

# 곱집합(Cartesian product) 구하기

## 문제. [1,2,3]과 [a,b,c]가 있을 때, 모든 각 리스트에서 1개씩 뽑아서 만들 수 있는 모든 조합의 수를 구해보세요

## 문제 풀이. 곱집합을 구하는 문제인데 곱집합이란 여러 집합들 간에 하나씩 뽑아 조합을 만들 수 있는 모든 수를 뜻한다. 파이썬에서는 for문을 사용하지 않고 itertools 라이브러리의 product 함수를 사용해 구할 수 있다.

```py
a = [1,2,3]
b = ['a', 'b', 'c']

a = product(a,b)
print(list(a))
```
