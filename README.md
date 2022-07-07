# 같은 숫자는 싫어


def solution(arr):
    for i in range(len(arr)):
        if i+1 == len(arr):
            break
        elif arr[i] == arr[i+1]:
            arr[i] = '*'
    arr = [i for i in arr if i != '*']
    return arr

#print(solution([4,4,4,3,3]))
#ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ


def no_continuous(s):
    a = []
    for i in s:
        if a[-1:] == [i]: continue
        a.append(i)
    return a
