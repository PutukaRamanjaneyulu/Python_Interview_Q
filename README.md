
# Interview Important Questions (Basic Python)

This repository contains a Jupyter Notebook with essential Python interview questions and their solutions. These questions cover fundamental programming concepts, logic-building exercises, and common algorithmic challenges often encountered in coding interviews.

## 📌 Overview
This notebook is designed to help Python learners and job seekers practice important coding problems. The solutions provided are beginner-friendly and include explanations to enhance understanding.

## 📖 Table of Contents

### 🔢 Number-Based Problems
1. **Perfect Number Check** - Check if a number is a perfect number by summing its proper divisors.
2. **Factorial Calculation** - Calculate the factorial of a given number using iteration.
3. **Palindrome Check** - Check if a number remains the same when reversed.
4. **Armstrong Number Check** - Verify if a number is equal to the sum of its digits raised to the power of the number of digits.
5. **Strong Number Check** - Determine if a number is equal to the sum of the factorial of its digits.
6. **Fibonacci Series Generation** - Generate and print the Fibonacci series up to a given number.

### 🔠 String-Based Problems
7. **ASCII Value Processing** - Extract and sum even ASCII values of characters in a given string.
8. **Digit Extraction and Skipping** - Extract numbers from a string and process them according to specified conditions.
9. **Alphabet Frequency Count** - Count and display occurrences of each letter in a given string as key-value pairs.


   

## 📝 Code Solutions

### 1️⃣ Perfect Number Check
```python
# Question : 1
# we can take the One number sum of Divisible  of number equal to the number
n = int(input("Enter a number here: "))
c = 0
for i in range(1, n):
    if n % i == 0:
        c += i
if n == c:
    print(f'{n} is a perfect number')
else:
    print(f'{n} is not a perfect number')
```

### 2️⃣ Factorial Calculation
```python
#Question 2
# Factorial of the is Ex:5*4*3*2*1
n=int(input("Enter a number here :"))
c=1
for i in range(1,n+1):
  c=c*i
print("The factorial of the given number :",c)
```

### 3️⃣ Palindrome Check
```python
# Question : 3
# we can take the One number and reverse the  number equal to the  original number

n=int(input("Enter a number here : "))
temp=n
c=0
while n >0:
  res=n%10
  c=(c*10)+res
  n=n//10
  
if temp == c:
  print(f'{temp} : is a palindrome number')
else:
  print(f'{temp} : is not palindrome number')

# second Method

n = input("Enter a number: ")
if n == n[::-1]:
    print("Palindrome")
else:
    print("Not a palindrome")
```

### 4️⃣ Armstrong Number Check
```python
# Question : 4
# we can take the One number and cube the digits and sum of the digits  equal to the  original number

n=int(input("Enter a number here : "))
temp=n
c=0
while n >0:
  res=n%10
  c=c+(res*res*res)
  n=n//10
  
if temp == c:
  print(f'{temp} : is a amstrong  number')
else:
  print(f'{temp} : is not amstrong  number')

```

### 5️⃣ Strong Number Check
```python
# Question : 5 (Method 1) with using the loop
# If we take number the factorial of the individuals digits and sum of the Factorial is eual to the number

n=int(input("Enter a number here : "))
temp=n
c=0
while n >0:
  res=n%10
  f=1
  for i in range(1,res+1):
    f=f*i
  
  c=c+f
  n=n//10
  
if temp == c:
  print(f'{temp} : is a strong  number')
else:
  print(f'{temp} : is not strong  number')


# Question : 5 (Method 2) without using loop and using the Built in fumctions
# If we take number the factorial of the individuals digits and sum of the Factorial is eual to the number
import math
n=int(input("Enter a number here : "))
temp=n
c=0
while n >0:
  res=n%10
  f=math.factorial(res)
  
  c=c+f
  n=n//10
  
if temp == c:
  print(f'{temp} : is a strong  number')
else:
  print(f'{temp} : is not strong  number')

```

### 6️⃣ Fibonacci Series Generation
```python
# Question : 6 
# Fibonacci series means we need to add the present number and to privous number these series is called the fibonacci series

n=int(input("Enter a number here : "))
a=0
b=1
print(a)
print(b)

for i in range(n-2):
  c=a+b
  print(c)
  a=b
  b=c
```

### 7️⃣ ASCII Value Processing
```python
s = input("Enter a string: ")
print("Even ASCII values:", sum(ord(ch) for ch in s if ord(ch) % 2 == 0))
```

### 8️⃣ Digit Extraction and Skipping
```python
#Question: 7 (method : 1) With using Built in functions
#a="data scince"
a="data scince"
b=0
for i in a:
  if i.isalpha():

    c=ord(i)

    if c%2==0:
        b=b+int(c)
print("The sum of the ascii even  values : ",b)
```

### 9️⃣ Alphabet Frequency Count
```python
# Question :9
# we give the string of the variaable and count the alphats how many times in string and print the (key value pair)
a='Ramanjaneyulu'
c={}

for i in a:
  if i not in c:
    c[i]=1
  else:
    c[i]=c[i]+1
print(c)

```

## 💡 How to Contribute
We welcome contributions! To add more Python interview questions or improve existing solutions:

1. Fork the repository.
2. Create a new branch (`feature-new-question`).
3. Commit your changes.
4. Push the branch and create a pull request.

## 📜 License
This project is open-source and available under the MIT License.

---

💻 **Happy Coding!** 🚀

Visit My Linked in : [https://www.linkedin.com/in/putuka-ramanjaneyulu-2128r/](linkedin)
