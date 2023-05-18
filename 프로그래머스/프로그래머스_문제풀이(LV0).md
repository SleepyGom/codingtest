## LV 0

### 대문자 만들기


```python
# 알파벳으로 이루어진 문자열 myString이 주어집니다. 
# 모든 알파벳을 대문자로 변환하여 return 하는 solution 함수를 완성해 주세요.

# 입출력 예
# myString	result
# "aBcDeFg"	"ABCDEFG"
# "AAA"	"AAA"

# 풀이
def solution(myString):
    
    return myString.upper()
```

### 정수찾기


```python
# 정수 리스트 num_list와 찾으려는 정수 n이 주어질 때, 
# num_list안에 n이 있으면 1을 없으면 0을 return하도록 solution 함수를 완성해주세요.

# 입출력 예
# num_list	n	result
# [1, 2, 3, 4, 5]	3	1
# [15, 98, 23, 2, 15]	20	0

# 풀이
def solution(num_list, n):
    if n in num_list:
        return 1
    else:
        return 0
```

### 문자열을 정수로 변환하기


```python
# 숫자로만 이루어진 문자열 n_str이 주어질 때, 
# n_str을 정수로 변환하여 return하도록 solution 함수를 완성해주세요.

# 입출력 예
# n_str	result
# "10"	10
# "8542"	8542

# 풀이
def solution(n_str):
    
    return int(n_str)
```

### 부분 문자열인지 확인하기


```python
# 부분 문자열이란 문자열에서 연속된 일부분에 해당하는 문자열을 의미합니다.
# 예를 들어, 문자열 "ana", "ban", "anana", "banana", "n"는
# 모두 문자열 "banana"의 부분 문자열이지만,
# "aaa", "bnana", "wxyz"는 모두 "banana"의 부분 문자열이 아닙니다.

# 문자열 my_string과 target이 매개변수로 주어질 때,
# target이 문자열 my_string의 부분 문자열이라면 1을,
# 아니라면 0을 return 하는 solution 함수를 작성해 주세요.

# 입출력 예
# my_string	target	result
# "banana"	"ana"	1
# "banana"	"wxyz"	0

# 풀이
def solution(my_string, target):
    if target in my_string:
        return 1
    else:
        return 0
    
```

### n 번째 원소까지


```python
# 정수 리스트 num_list와 정수 n이 주어질 때, 
# num_list의 첫 번째 원소부터 n 번째 원소까지의 모든 원소를 담은 리스트를 return하도록 solution 함수를 완성해주세요.

# 입출력 예
# num_list	n	result
# [2, 1, 6]	1	[2]
# [5, 2, 1, 7, 5]	3	[5, 2, 1]

# 풀이
def solution(num_list, n):
    
    return num_list[:n]
```

### 문자열의 뒤의 n글자


```python
# 문자열 my_string과 정수 n이 매개변수로 주어질 때,
# my_string의 뒤의 n글자로 이루어진 문자열을 return 하는 solution 함수를 작성해 주세요.

# 입출력 예
# my_string	n	result
# "ProgrammerS123"	11	"grammerS123"
# "He110W0r1d"	5	"W0r1d"

# 풀이
def solution(my_string, n):
    
    return my_string[-n:]
```

### 공백으로 구분하기 1


```python
# 단어가 공백 한 개로 구분되어 있는 문자열 my_string이 매개변수로 주어질 때,
# my_string에 나온 단어를 앞에서부터 순서대로 담은 문자열 배열을
# return 하는 solution 함수를 작성해 주세요.

# 입출력 예
# my_string	result
# "i love you"	["i", "love", "you"]
# "programmers"	["programmers"]

# 풀이
def solution(my_string):
    
    return my_string.split(' ')
```

### 조건에 맞게 수열 변환하기 3


```python
# 정수 배열 arr와 자연수 k가 주어집니다.
# 만약 k가 홀수라면 arr의 모든 원소에 k를 곱하고, k가 짝수라면 arr의 모든 원소에 k를 더합니다.
# 이러한 변환을 마친 후의 arr를 return 하는 solution 함수를 완성해 주세요.


# 입출력 예
# arr	k	result
# [1, 2, 3, 100, 99, 98]	3	[3, 6, 9, 300, 297, 294]
# [1, 2, 3, 100, 99, 98]	2	[3, 4, 5, 102, 101, 100]

# 풀이
def solution(arr, k):
    if k % 2 == 1:
        return [k*i for i in arr]
    else:
        return [k+i for i in arr]
```

### n 번째 원소부터



```python
# 정수 리스트 num_list와 정수 n이 주어질 때,
# n 번째 원소부터 마지막 원소까지의 모든 원소를 담은 리스트를
# return하도록 solution 함수를 완성해주세요.

# 입출력 예
# num_list	n	result
# [2, 1, 6]	3	[6]
# [5, 2, 1, 7, 5]	2	[2, 1, 7, 5]

# 풀이
def solution(num_list, n):
    
    return num_list[n-1:]
```

### 첫 번째로 나오는 음수


```python
# 정수 리스트 num_list가 주어질 때,
# 첫 번째로 나오는 음수의 인덱스를 return하도록 solution 함수를 완성해주세요.
# 음수가 없다면 -1을 return합니다.

# 입출력 예
# num_list	result
# [12, 4, 15, 46, 38, -2, 15]	5
# [13, 22, 53, 24, 15, 6]	-1

# 내 풀이
def solution(num_list):
    answer = []
    for i in range(len(num_list)):
        if int(num_list[i]) < 0:
            answer.append(num_list.index(num_list[i]))
    
    if len(answer) >= 1:
        return answer[0]
    else:
        return -1

# 다른 사람 풀이
def solution(num_list):
    for i in range(len(num_list)):
        if num_list[i]<0:return i
    return -1

```

### 주사위 게임 1


```python
# 1부터 6까지 숫자가 적힌 주사위가 두 개 있습니다.
# 두 주사위를 굴렸을 때 나온 숫자를 각각 a, b라고 했을 때 얻는 점수는 다음과 같습니다.

# a와 b가 모두 홀수라면 a2 + b2 점을 얻습니다.
# a와 b 중 하나만 홀수라면 2 × (a + b) 점을 얻습니다.
# a와 b 모두 홀수가 아니라면 |a - b| 점을 얻습니다.
# 두 정수 a와 b가 매개변수로 주어질 때, 얻는 점수를 return 하는 solution 함수를 작성해 주세요.

# 입출력 예
# a	b	result
# 3	5	34
# 6	1	14
# 2	4	2

# 내 풀이
def solution(a, b):
    if a % 2 != 0 and b % 2 != 0:
        return (a ** 2) + (b ** 2)
    elif a % 2 != 0 or b % 2 != 0:
        return 2 * (a + b)
    else:
        return abs(a - b)
```
