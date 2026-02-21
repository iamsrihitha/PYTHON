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