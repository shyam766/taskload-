ame=input('Enter your name\n')
gender=input('Enter Gender(Male or Female)\n')
print('\nHello ',name,'!!\nTo Calculate NASA TLX,you have to quantify your demanding level from 1 to 100(Multiple of 5). Where 1 is Extreme Low and 100 is Extreme High demanding')
def i1():
 global mds
 if mds<1 or mds>100 or mds%5!=0:
    print("Pls enter values between 1 to 100 and multiple of 5\n")
    mds=eval(input('HOW MENTALLY DEMANDING WAS THE TASK?\n'))
    i1()
 return(mds)
def i2():
 global pds  
 if pds<1 or pds>100 or (pds%5)!=0:
    print("Pls enter values between 1 to 100 and multiple of 5\n")
    pds=eval(input('HOW PHYSICALLY DEMANDING WAS THE TASK?\n'))
    i2()
 return(pds)
def i3():
 global tds  
 if tds<1 or tds>100 or (tds%5)!=0:
    print("Pls enter values between 1 to 100 and multiple of 5\n")
    tds=eval(input('How HURRIED OR RUSHED WAS THE PACE OF THE TASK?\n'))
    i3()
 return(tds)  
def i4():
 global ps  
 if ps<1 or ps>100 or (ps%5)!=0:
    print("Pls enter values between 1 to 100 and multiple of 5\n")
    ps=eval(input('HOW SUCCESSFUL WERE YOU IN COMPLETINING IT (1 BEING PERFECT AND 100 BEING FAILURE)\n'))
    i4()
 return(ps)  
def i5():
 global es  
 if es<1 or es>100 or (es%5)!=0:
    print("Pls enter values between 1 to 100 and multiple of 5\n")
    es=eval(input('HOW HARD DID YOU WORK'))
    i5()
 return(es)  
def i6():
 global fs  
 if fs<1 or fs>100 or (fs%5)!=0:
    print("Pls Enter Values Between 1 to 100 and multiple of 5\n")
    fs=eval(input('HOW FRUSTRATED WERE YOU?\n'))
    i6()
 return(fs)
mds=eval(input('HOW MENTALLY DEMANDING WAS THE TASK?\n'))
mds=i1()
pds=eval(input('HOW PHYSICALLY DEMANDING WAS THE TASK?\n'))
pds=i2()
tds=eval(input('HOW HURRIED OR RUSHED WAS THE PACE OF THE TASK\n'))
tds=i3()
ps=eval(input('HOW SUCCESSFUL WERE YOU IN COMPLETINING IT (1 BEING PERFECT AND 100 BEING FAILURE)\n'))
ps=i4()
es=eval(input('HOW HARD DID YOU WORK?\n'))
es=i5()
fs=eval(input('HOW FRUSTRATED WERE YOU?\n'))
fs=i6()                                    
print("\nMental Demand Raw Score:",mds)
print("Physical Demand Raw Score:",pds)
print("Temporal Demand Raw Score:",tds)
print("Performance Raw Score:",ps)
print("Effort Score:",es)
print("Frustration Score:",fs)
cmd,cpd,ctd,cp,ce,cf = 0,0,0,0,0,0
print("\nChoose the factor that represents the more important contributor of workload for the task\n")
a=5
while(a!=0  and a!=1):
                  print("Mental Demand (press 1) OR Physical Demand(press 0)?")
                  a=int(input())
                  if(a==1):
                           cmd=cmd+1
                  elif(a==0):
                            cpd=cpd+1
                  else:
                      print("Wrong Input")
a=5
while(a!=1 and a!=0):
                 print("Mental Demand (press 1) OR Temporal Demand(press 0)?")
                 a=int(input())
                 if(a==1):
                         cmd=cmd+1
                 elif(a==0):
                         ctd=ctd+1 
                 else:
                      print("Wrong Input")
a=5

while(a!=1 and a!=0):
    print("Mental Demand (press 1) OR Performance(press 0)?")
    a=int(input())
    if(a==1):
        cmd=cmd+1
    elif(a==0):
            cp=cp+1
    else:
            print("Wrong Input")
a=5
while(a!=1 and a!=0):
     print("Mental Demand (press 1) OR Effort(press 0)?")
     a=int(input())
     if(a==1):
         cmd=cmd+1
     elif(a==0):
         ce=ce+1
     else:
             print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Mental Demand (press 1) OR Frustration(press 0)?")
    a=int(input())
    if(a==1):
        cmd=cmd+1
    elif(a==0):
        cf=cf+1
    else:
            print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Physical Demand(press 1) OR Temporal Demand(press 0)?")
    a=int(input())
    if(a==1):
        cpd=cpd+1
    elif(a==0):
        ctd=ctd+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0): 
    print("Physical Demand(press 1) OR Performance(press 0)?")
    a=int(input())
    if(a==1):
        cpd=cpd+1
    elif(a==0):
        cp=cp+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Physical Demand(press 1) OR Effort(press 0)?")
    a=int(input())
    if(a==1):
        cpd=cpd+1
    elif(a==0):
        ce=ce+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Physical Demand(press 1) OR Frustration(press 0)?")
    a=int(input())
    if(a==1):
        cpd=cpd+1
    elif(a==0):
        cf=cf+1
    else:
            print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Temporal Demand(press 1) OR Performance(press 0)?")
    a=int(input())
    if(a==1):
        ctd=ctd+1
    elif(a==0):
        cp=cp+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Temporal Demand(press 1) OR Effort(press 0)?")
    a=int(input())
    if(a==1):
        ctd=ctd+1
    elif(a==0):
        ce=ce+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Temporal Demand(press 1) OR Frustration(press 0)?")
    a=int(input())
    if(a==1):
        ctd=ctd+1
    elif(a==0):
        cf=cf+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Performance(press 1) OR Effort(press 0)?")
    a=int(input())
    if(a==1):
        cp=cp+1
    elif(a==0):
        ce=ce+1
    else:
        print("Wrong Input")

a=5
while(a!=1 and a!=0):
    print("Performance(press 1) OR Frustration(press 0)?")
    a=int(input())
    if(a==1):
        cp=cp+1
    elif(a==0):
        cf=cf+1
    else:
        print("Wrong Input")
a=5
while(a!=1 and a!=0):
    print("Effort(press 1) OR Frustration(press 0)?")
    a=int(input())
    if(a==1):
        ce=ce+1
    elif(a==0):
        cf=cf+1
    else:
        print("Wrong Input")
#output
print("\n")
print("Name: ",name)
print("Gender:",gender)
wt=[mds*cmd,pds*cpd,tds*ctd,ps*cp,es*ce,fs*cf]
nestedList = [["Mental",mds,cmd,wt[0]],["Physical",pds,cpd,wt[1]],
               ["Temporal",tds,ctd,wt[2]],["Performance",ps,cp,wt[3]],
               ["Effort",es,ce,wt[4]],["Frustration",fs,cf,wt[5]]]
print(": TYPE OF DEMAND  :  SCORE   :  PRIORITY  :  FINAL SCORE :")
for item in nestedList:
    print(":",item[0]," "*(14-len(item[0])),": ",item[1]," "*(6-len(str(item[1]))),
          ": ",item[2]," "*(8-len(str(item[2]))),": ",item[3]," "*(10-len(str(item[3]))),":")
sum=0
for item in wt:
    sum=sum+item
nasaTLI=float(sum/15)
print(" ")
print("The NASA Task Load Index is: ",nasaTLI)
def ch():
    print('Enter the no of employees')
    n=int(input())
    a=list()
    for i in range(0,n):
        print('Enter the TLX Index for',i+1,' Employee')
        x=float(input())
        a.append(x)
    avg=(min(a)+max(a))/2

    c=0
    print("Average of best and worst NASA TLI:",avg)
    for i in range(0,n):
      if a[i]>avg:
        c=c+1
    if c<int(n/2):
       print("\nLess than 50% of Employees have high NASA TLI,so workforce is in good condition")
    else:
       print("\nMore than  50% of employees have high NASA TLI,so changes needed")

print("If you want to check if your workforce is in good condition,press 1,if no press any key")
inp=int(input())
if (inp==1):
  ch()
else:
  print('THANK YOU') 
