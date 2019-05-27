# Looping

## Print Multiplication Table for a Number

```python
val = input("Enter the number: ")
for i in range(1, 11):
    print(val + " x " + str(i) + " = " + str(int(i)*int(val)))
```

## Finding Factors of a Number

```python
num=int(input("Enter A Number: "))

print("Factors of " + str(num) + " are: ")

for i in range(1,num+1):
    if num%i==0:
       print(i)
```

## Checking for Perfect Number

```python
num=int(input("Enter A Number: "))

s = 0
for i in range(1,num+1):
    if num%i==0:
       s = s + i

if(s == 2*num):
    print("The number is a perfect number")
else:
    print("The number is not a perfect number")
```

## Checking for Prime Number

```python
n = 0

for i in range(2, num):
    if i%num == 0:
        n += 1

if n == 0:
    print(n, " is a prime number")
else:
    print(n, " is not a prime number")
```

## Checking for Palindrome Number

```python
n = int(input("Enter Number: "))
num = n
r = 0
while n != 0:
    digit = n % 10
    r = (r * 10) + digit
    n = n//10

if(num == r):
    print("The humber is a palindrome")
else:
    print("The number is not a palindrome")
```

## Checking for Armstrong Number

```python
num = int(input("Enter a number: "))
sum = 0
n = num

while n > 0:
   digit = n % 10
   sum += digit ** 3
   n //= 10
if num == sum:
   print(num,"is an Armstrong number")
else:
   print(num,"is not an Armstrong number")
```

## Fibonacci sequence upto n terms

```python
nterms = int(input("How many terms? "))

n1 = 0
n2 = 1
count = 0

if nterms == 1:
   print("Fibonacci sequence upto",nterms,":")
   print(n1)
else:
   print("Fibonacci sequence upto",nterms,":")
   while count < nterms:
       print(n1,end=', ')
       nth = n1 + n2
       n1 = n2
       n2 = nth
       count += 1
```

# Menu Driven Program

## Print Factors & Check Even or Odd

### Without Loop

```python
print("1 - Print Factor")
print("2 - Check Even or Odd")
choice = int(input("Enter your choice - "))
if choice == 1:
    n = int(input("Enter Number: "))
    for i in range (1, n +1):
        if n%i==0:
            print(i)
elif choice == 2:
    n = int(input("Enter Number: "))
    if n % 2 == 0:
        print("Even")
    else:
        print("Odd")
else:
    print("Invalid Choice")
```

### With Loop

```python
while True:
    print("1 - Print Factor")
    print("2 - Check Even or Odd")
    print("0 - Exit")
    choice = int(input("Enter your choice : "))
    if choice == 0:
        break
    elif choice == 1:
        n = int(input("Enter Number: "))
        for i in range (1, n +1):
            if n % i==0:
                print(i)
    elif choice == 2:
        n = int(input("Enter Number: "))
        if n % 2 == 0:
            print("Even")
        else:
            print("Odd")
    else:
        print("Invalid Choice")

``
