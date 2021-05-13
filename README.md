# rev of fst and lst
n=int(input())
nn=0
temp=n
p=1
c=0
while n:
    r=n%10
    n=n//10
    c+=1
n=temp
k=c
c=c-1
n1=n%10
n2=n//pow(10,c)
print(c)
while n!=0 or c!=-1:
    r=n//pow(10,c)
    n=n%pow(10,c)
    if c==(k-1):
        r=n1
    else:
        if c==0:
            r=n2
    nn=nn*10+r
    c-=1
print(nn)        
