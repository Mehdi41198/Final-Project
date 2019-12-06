# Final-Project
CSC 101 Final Project
#First part Matrix Calculator
print("WELCOME TO THE MATRIX CALCULATOR !!")

print("This Matrix calculator will allow you to input your values in three by three dimension matrices (x,y) the calculator will first show the addition of theses two matrices, then their difference, and their product")

n = 3

print("For your first matrix (x) please input your variables from a to i")


a=int(input("a: "))
b=int(input("b: "))
c=int(input("c: "))
d=int(input("d: "))
e=int(input("e: "))
f=int(input("f: "))
g=int(input("g: "))
h=int(input("h: "))
i=int(input("i: "))

print("Now you can input your values for the Y Matrix")

j=int(input('j: '))
k=int(input('k: '))
l=int(input('l: '))
m=int(input('m: '))
o=int(input('o: '))
p=int(input('p: '))
q=int(input('q: '))
s=int(input('s: '))
t=int(input('t: '))



X = [[a,b,c],
    [d ,e,f],
    [g ,h,i]]

Y = [[j,k,l],
    [m,o,p],
    [q,s,t]]

result = [[0,0,0],[0,0,0],[0,0,0]]
         
for i in range(len(X)):
   for j in range(len(X[0])):
       result[i][j] = X[i][j] + Y[i][j]

print("Addition: ")
for r in result:
   print(r)



for i in range(len(X)):
   for j in range(len(X[0])):
       result[i][j] = X[i][j] - Y[i][j]

print("Substraction: ")
for r in result:
   print(r)


for i in range(len(X)):
   for j in range(len(X[0])):
       result[i][j] = sum((X[i][v]*Y[v][j] for v in range(n)))

print("Multiplication: ")
for r in result:
   print(r)
