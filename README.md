# Basic-calc2.py
print("Enter the expression:")
var = input()
res=0
res1=0
res2=0
A=str(var)
if "+" in A:
    for x in range(len(A)):
        if A[x]=="+":
            a=x
    i=0
    while i<a:
        res=res+int(A[i])*(10**(a-(i+1)))
        i=i+1
    i=0
    while i<len(A)-a-1:
        res=res+int(A[a+i+1])*(10**(len(A)-a-i-2))
        i=i+1
    print(res)   
if "-" in A:
    for x in range(len(A)):
        if A[x]=="-":
            a=x
    i=0
    while i<a:
        res1=res1+int(A[i])*(10**(a-(i+1)))
        i=i+1
    i=0
    while i<len(A)-a-1:
        res2=res2+int(A[a+i+1])*(10**(len(A)-a-i-2))
        i=i+1
    print(res1-res2)   
if "*" in A:
    for x in range(len(A)):
        if A[x]=="*":
            a=x
    i=0
    while i<a:
        res1=res1+int(A[i])*(10**(a-(i+1)))
        i=i+1
    i=0
    while i<len(A)-a-1:
        res2=res2+int(A[a+i+1])*(10**(len(A)-a-i-2))
        i=i+1
    print(res1*res2)             
if "/" in A:
    for x in range(len(A)):
        if A[x]=="/":
            a=x
    i=0
    while i<a:
        res1=res1+int(A[i])*(10**(a-(i+1)))
        i=i+1
    i=0
    while i<len(A)-a-1:
        res2=res2+int(A[a+i+1])*(10**(len(A)-a-i-2))
        i=i+1
    print(res1/res2)             
if "^" in A:
    for x in range(len(A)):
        if A[x]=="^":
            a=x
    i=0
    while i<a:
        res1=res1+int(A[i])*(10**(a-(i+1)))
        i=i+1
    i=0
    while i<len(A)-a-1:
        res2=res2+int(A[a+i+1])*(10**(len(A)-a-i-2))
        i=i+1
    print(pow(res1,res2))             
             
    
