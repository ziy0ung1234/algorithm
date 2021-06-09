### 2021.06-08 Python zip 함수

# 2차원 리스트 뒤집기

## 문제. 다음을 만족하는 함수, solution을 완성해주세요.
- solution 함수는 이차원 리스트, mylist를 인자로 받습니다
- solution 함수는 mylist 원소의 행과 열을 뒤집은 한 값을 리턴해야합니다.

## 문제 풀이. 파이썬에서는 zip함수와 unpacking(*)을 이용해 2중 for문을 돌리지 않고 2차원 배열을 뒤집을 수 있다. 
```py
def solution(mylist):

    new_list= list(map(list, zip(*mylist)))
    return new_list
```
