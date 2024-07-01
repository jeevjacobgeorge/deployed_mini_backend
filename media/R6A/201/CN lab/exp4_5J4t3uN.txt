# #question no: 3
# print(round(12.57))
# print(5/2)
# print(int(6.5))

# #question no: 4

# s = "Computer" 
# print(s[::2])
# print(s[::-1])
# print(s[:])




# # # Python program to find gcd using inbuilt function using math library
# # import math
 
# # #Driver code
# # if __name__ == '__main__':
# #   a = 10
# #   b = 5
# #   gcd_result = math.gcd(a, b) # inbuilt function gcd() using math library
 
# #   print("The gcd of a and b is", gcd_result)
  
# def gcd(a,b):
#     if(b==0):
#         return a
#     else:
#         return gcd(b,a%b)
# a=int(input("Enter first number:"))
# b=int(input("Enter second number:"))
# GCD=gcd(a,b)
# print("GCD is: ")
# print(GCD)


# import numpy as np
# arr1 = np.arange(6).reshape((3, 2))
# arr2 = np.arange(6).reshape((3,2))
# arr3 = arr1 + arr2[0].reshape((1, 2))
# print(arr3)


# import turtle as t

# window = t.Screen()
# ptr =  t.Turtle()
# t.setheading(0)

# window.mainloop()

# def generate_primes(start, end):
#     primes = []

#     for num in range(start, end + 1):
#         if num > 1:
#             is_prime = True
#             for i in range(2, int(num**0.5) + 1):
#                 if num % i == 0:
#                     is_prime = False
#                     break
#             if is_prime:
#                 primes.append(num)

#     return primes

# # Input the range
# start = int(input("Enter the start of the range: "))
# end = int(input("Enter the end of the range: "))

# # Generate and print prime numbers within the range
# print(f"Prime numbers between {start} and {end}:")
# print(generate_primes(start, end))



# data = "Python rules!"
# print(data.split())
# print(data.upper())
# print(data.find("rules"))
# print(data.replace("!", "?"))
# Open the file for input



file =  open("trial.txt", 'r')
        # Read the contents of the file
content = file.read()
        
        # Split the content into words
words = content.split()
print(words)
        # Count the number of four-letter words
# sum = 0
# for word in words: 
#     if len(word) == 4:
#         sum += 1 
four_letter_words = sum(1 for word in words if len(word) == 4)
        
        # Print the number of four-letter words
print("Number of four-letter words in the file:", four_letter_words)

