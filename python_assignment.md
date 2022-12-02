Program to merge to dictionaries:

Input : [('for', 24), ('Geeks', 8), ('Geeks', 30)] 
#Output : [('Geeks', 8), ('for', 24), ('Geeks', 30)]
dict1={1:'p',2:'v'}
dict2={3:'n',4:'m'}
dict1.update(dict2)
print(dict1)

#Write a Python program to extract unquire dictionary values.
dict={1:'p',2:'v',3:'n',4:'m',3:'n',4:'m'}
#for k,v in dict:


Program to print factorial of a number
#print("enter no.",)
def factorial(num):
    fact=1
    for i in range(1,num+1):
        fact=fact*i
        return fact
print(factorial(5))        

Write a Python Program to calculate the natural logarithm of any number?    
import math

try:
    num = int(input("Enter the number: "))
except Exception as e:
    print(e)
else:
    print(math.log(num))    


Write a Python Program for cube sum of first n natural numbers?
def cubN(n):
    return sum(range(n+1))**3
print(cubN(3))

Write a Python Program to check if given array is Monotonic?
l=[67,55,44,33,78,2]
def monotonic(l):
    flag=True
    if l[0]>l[len(l)-1]:
        for i in range(1,len(l)):
            if l[i-1]<l[i]:
                flag= False
    else:
        for i in range(1,len(l)):
            if l[i-1]>l[i]:
                flag= False

    return flag    
s=monotonic(l)
if s==True:
    print("array is monotonic")
else:
    print("Array is not monotonic")    

#Program to add to matrices
mat1 = [[1,2,3],
        [6, -4, -9],
        [3,6,9]]

mat2 = [[6,9,3],
        [1,-1,1],
        [0, 9, 11]]
result=[]        
for i in range(len(mat1)):
    row=[]
    for j in range(len(mat1)):
        row.append(mat1[i][j]+mat2[i][j])  
    result.append(row)    
print(result)

Program to multiply two matrices
result=[]
for i in range(len(mat1)) :
    row =[]
    sum =0
    for j in range(len(mat2)) :
        row=sum+mat1[i][j]*mat2[i][j]
    result    


#transpose of a matrice

X = [[12,7],
    [4 ,5],
    [3 ,8]]

result = [[0,0,0],
         [0,0,0]]

# iterating through rows
for i in range(len(X)):
   # iterating through columns
   for j in range(len(X[0])):
        result[j][i] = X[i][j]

for r in result:
    print(r)  

#Write a Python Program to Sort Words in Alphabetic Order?
try:

    sen=input('Enter sentence here:')
    words=[word.lower() for word in sen.split(" ")]
    words.sort()
    print("words after sorting:")
    for word in words:
        print(word,end=" ")
except Exception as e:
    print(e)

## 5. Write a Python Program to Remove Punctuation From a String?
punctuations = '''!()-[]{};:'"\,<>./?@#$%^&*_~'''

string = input("Enter the string: ")

outputString = ""

for char in string:
    if char not in punctuations:
        outputString += char
        
print(outputString)

print("just for commit")
print("commit 2")

print("commit 3")
print("commit 4")