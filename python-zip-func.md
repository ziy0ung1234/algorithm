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

# i번째 원소와 i+1번째 원소

## 문제. 숫자를 담은 리스트 mylist가 solution 함수의 파라미터로 주어집니다. solution 함수가 mylist의 i번째 원소와 i+1번째 원소의 차를 담은 일차원 리스트에 차례로 담아 리턴하도록 코드를 작성해주세요.

단, 마지막에 있는 원소는 (마지막+1)번째의 원소와의 차를 구할 수 없으니, 이 값은 구하지 않습니다.

```py
def solution(mylist):
    answer = []
    for i,j in zip(mylist, mylist[1:]):
        answer.append(abs(i - j))
    return answer

# 처음 작성한 풀이
def solution(mylist):
    answer = []
    for i in range(len(mylist)-1):
        if mylist[i] > mylist[i+1]:
            answer.append(mylist[i] - mylist[i+1])
        else:
            answer.append(mylist[i+1] - mylist[i])
    return answer

# 처음 작성한 풀이 -> 절댓값 함수 abs를 사용해 if문 줄일 수 있음
def solution(mylist):
    answer = []
    for i in range(len(mylist)-1):
        answer.append(abs(mylist[i] - mylist[i+1]))
    return answer
```

