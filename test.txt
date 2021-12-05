#1000
import sys
input = sys.stdin.readline
print(sum(list(map(int,input().split()))))

#1001
import sys
input = sys.stdin.readline
list_input = list(map(int, input().split()))
print(list_input[0]-list_input[1])

#1002
import sys
T = int(input())
for _ in range (T):
    input = sys.stdin.readline
    x1, y1, r1, x2, y2, r2 = list(map(int, input().split()))
    dist = ((x1-x2)**2+(y1-y2)**2)
    if dist == 0 and r1==r2: print(-1)
    elif dist == (r1+r2)**2: print(1)
    elif dist > (r1+r2)**2 : print(0)
    elif dist == (r1-r2)**2 : print(1)
    elif dist < (r1-r2)**2: print(0)
    else: print(2)