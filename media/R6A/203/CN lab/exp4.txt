import math
num = int(input("Enter the number: "))
count = math.floor(math.log10(num) + 1)
print(count)
sum = 0
n1 = num
while num > 0:
    d = num % 10
    sum = sum + d**count
    num = num // 10
print(sum)
print(n1)
if n1 == sum:
    print("armstrong")
else:
    print(" not armstrong")
