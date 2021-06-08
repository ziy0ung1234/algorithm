### 2021.06.08 Python string module

# 알파벳 출력하기

## 문제. 입력으로 0이 주어지면 영문 소문자 알파벳을, 입력으로 1이 주어지면 영문 대문자 알파벳을 사전 순으로 출력하는 코드를 짜세요.

## 문제 풀이. 알파벳 a-z를 모두 치지 않아도 파이썬 string 모듈을 import 해서 사용하면 소문자, 대문자, 또는 소문자와 대문자를 모두 출력할 수 있다.
1. string.ascii_letters
- 영어 알파벳 소문자, 대문자 모두를 출력
2. string.ascii_lowercase
- 영어 소문자를 출력
3. string.ascill_uppercase
- 영어 대문자를 출력
4. string.digits
- 십진수 0 ~ 9 까지 출력
5. string.hexdigits
- 16진수 출력
6. string.punctuation
- 특수 문자 출력

```py
import string

num = int(input().strip())
if num == 0:
    print(string.ascii_lowercase)
if num == 1:
    print(string.ascii_uppercase)

# 처음 작성한 답안
num = int(input().strip())
if num == 0:
    print(str('ABCDEFGHIJKLMNOPQRSTUVWXYZ').lower())
if num == 1:
    print(str('ABCDEFGHIJKLMNOPQRSTUVWXYZ').upper())
```
