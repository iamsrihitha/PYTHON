# this is fibonaci series
def fib(n):
    if n==0:
        return 0
    elif n==1:
        return 1
    else:
        return fib(n-1)+fib(n-2)
n=int(input())
for i in range(n):
    print(fib(i))

'''
input:5
output:0
1
1
2
3
'''



# sum of fibonacci series 
def fibonacci(n):
    if n == 0:
        return 0
    if n==1:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)
n=int(input())
sums=0
for i in range(n):
    sums+=fibonacci(i)
print(sums)

'''
input: 5
output:7
'''


# three digit number divisible by 9
n=int(input())
if 100<= n <= 999:
    if n%9==0:
        print("divisible by 9")
    else:
        print("not")
else:
    print("it is not a three digit number")

# smallest and largest number and their difference
n=int(input())
arr=list(map(int,input().split()))
smallest=arr[0]
largest=arr[0]
for i in arr:
    if smallest>i:
        smallest=i
    if largest<i:
        largest=i
print(smallest)
print(largest)
print("The maximum difference is",largest-smallest)