# nested-loops-pythonclass_count = 1

while(class_count <= 3):
    std_count = 1
    sec_avg = 0
    sec_sum = 0
    print
    while(std_count <= 5):
        print("Enter marks for Student-",std_count," of Section-",class_count," : ", end='')
        marks = int(input())
        sec_sum += marks
        std_count += 1
    sec_avg = sec_sum / 5
    print("Average Marks of Section-", class_count," : ", sec_avg)
    
    class_count += 1

  #2
repeat = 'y'

limit = 10
while(repeat == 'y' or repeat == 'Y'):
    count = 1
    num = int(input("Enter your Number : "))
    print("Table of ",num," : ")
    while count <= limit:
        print(num," X ", count, " = ", num*count)
        count += 1
        
    repeat = input("Do you want to Print Another Table (y/n) : ")
print("Thank You! ")


#3
outer = 1

print("Before Loop!")
while(outer <= 4):
    print("Inside Outer Loop!")
    inner = 1
    while(inner <= 3):
        print("Inside Inner Loop")
        inner += 1
    outer += 1

print("After All Loops")


#4
repeat = 'y'

while(repeat == 'y'):
    count = int(input("Enter Start of Table : "))
    limit = int(input("Enter Range of Table : "))

    num = int(input("Enter your Number : "))

    while(count <= limit):
        print(num," X ",count," = ", num*count)
        count += 1
    
    repeat = input("Do you want to Print Another Talble (y/n) ? ")


    #5
    r1 = int(input("Enter Start of Range : "))
r2 = int(input("Enter End   of Range : "))

print("Prime Numbers Between ",r1," and ",r2," : \n")
while(r1 < r2):
    
    prime = True
    d = 2
    while(d < r1):
        if(r1 % d == 0):
            prime = False
            break;
        d += 1

    if(prime):
        print(r1,"\t", end='')
    r1 += 1


    #6
    r1=int(input('enter the start of the range'))
r2=int(input('enter the end of the range'))
print('prime numbers between',r1,'and',r2,':/n')
while r1<r2:
    prime=True
    d=2
    while d<r1:
         if r1%d==0:
            prime=False
            break;
         d+=1
    if prime:
        print(r1,'/t',end='')
    r1+=1


    #7
    count = int(input("Enter Start of Table : "))
limit = int(input("Enter Range of Table : "))

num = int(input("Enter your Number : "))
count = 0
while(count <= limit):
    count += 1
    print("Count - ", count)
    if(count == 4):
        continue   
    print(num," X ",count," = ", num*count)
    
print("Count = ", count)
print("Outside of the Loop")

#8
N = int(input("How many Students in the Class : "))
Name = ' '
count = 1
while(count <= N):
    count += 1
    Name = input("What is Your Name : ")
    if(Name == 'HISHAM'):
        break
    Marks = int(input("Enter Yur Marks : "))
    City = input("Your City Please : ")
    
    print("Name  : ", Name)
    print("City  : ", City)
    print("Marks : ", Marks)


    #9
    num = int(input("Enter your Number : "))
d = 2
prime = True
while(d < num):
    if(num%d == 0):
        prime = False
        break;
    d += 1

if(prime):
    print(num," is a Prime Number.")
else:
    print(num," is not a Prime Number.")


#10
class_count = 1
while(class_count <= 3):
    std_count = 1
    class_sum = 0
    class_avg = 0
    while(std_count <= 5):
        print("Enter Marks of Student-",std_count," in Class-", class_count," : ", end='')
        marks = int(input())
        
        class_sum += marks
        std_count += 1
    class_avg = class_sum / 5
    print("Average Marks of Class-", class_count, " : ", class_avg)
    class_count += 1
print("Thank You For Using This App!")


#11
limit = 10
repeat = 'y'
while(repeat == 'y' or repeat == 'Y'):
    N = int(input("Enter your Number"))
    count = 1
    while count <= limit:
        print(N," X ", count, " = ", N*count)
        count += 1
    repeat = input("Do you want to Print another Table (y/n)?")
    
print("Thank You!")

#12
class_limit = 3
std_limit = 5
class_count = 1
while(class_count <= class_limit):
    std_count = 1
    class_sum = 0
    class_avg = 0
    while(std_count <= std_limit):
        print("Enter Marks of Student-",std_count," in Class-",class_count," : ")
        marks = int(input())
        class_sum += marks
        std_count += 1
    
    class_avg = class_sum / std_limit
    print("Average Marks of Class-",class_count," : ", class_avg)
    class_count += 1 

print("Thank You!")
