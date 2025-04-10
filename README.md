# conditional-and-looping-statements
month_names=dict({1:'JANUARY',2:'FEBRUARY',3:'MARCH',4:'APRIL',5:'MAY',6:'JUNE',7:'JULY',8:'AUGUST',9:'SEPTEMBER',10:'OCTOBER',11:'NOVEMBER',12:'DECEMBER'})
name=input('Enter the month number between 1 and 12: ')
month_num=int(name)
if 1 <= month_num <= 12:
 "break"

month_names1 = month_names.get(month_num)
print(f'the month is' ,{month_names1})


age1 = input('enter your age: ')
age = int(age1)
if age <= 16:
    print('your ticket costs 3')

elif age >= 60:
    print('your ticket costs 2')

else:
    print('your ticket costs 6')




x=input('enter your weight in kg: ')
y=input('enter your height in m: ')
weight=float(x)
height=float(y)
BMI=weight/(height*height)
print('your BMI is',BMI)
if BMI < 18.5:
    print('you are underweight')
elif BMI >= 18.5 and BMI <= 24.9:
    print('you are normal')
elif BMI >= 25 and BMI <= 29.9:
    print('you are overweight')
elif BMI >= 30:
    print('you are obese')
else:
    print('invalid value')



x=int(input('enter number 1'))
y=int(input('enter number 2'))
z=int(input('enter number 3'))
if (x>y) and (x>z):
    a=x
elif (y>x) and (y>z):
    a=y
else:
    a=z

print('largest number is ',a)


num=int(input('Enter a number: '))
factorial = 1
for i in range(1,num+1):
    factorial = factorial * i
print('factorial of ',num, 'is',factorial)


num = int(input('Enter a number: '))
reversed_num = 0

while num != 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num //= 10

print("Reversed Number: " + str(reversed_num))


x=int(input('enter a number'))
print('multiples of ',x,'are')
for i in range(1,11):
    print(x*i,end=" ")



while True:
         x=input('enter a value (or done to quit): ')
         if x=='done':
             break
         else:
            print(x)



for i in range(1,21):
    if i%3==0 and i%5==0:
        print('FizzBuzz')
    elif i%3==0:
        print('Fizz')
    elif i%5==0:
        print('Buzz')

    else:
        print(i)




for i in range(5,0,-1):
    for j in range(i,0,-1):
        print(j,end=" ")
    print()
