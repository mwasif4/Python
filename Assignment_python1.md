Write code to check a String is palindrome or not
def palind_check(x):
    a = x.replace(' ','').lower()
    if a == a[::-1]:
        return True
    else:
        return False
palind_check('A Santa dog lived as a devil God at NASA')
True
palind_check('Nittin')
True


Write a method which will remove any given character from a String?
a = 'this is a %sentence'
def remove_character(x,index):
    return x.replace(x[index],'')
remove_character(a,10)
'this is a sentence'


In an list 1-100 numbers are stored, one number is missing how do you find it?
a = list(range(101))
a.pop(75)
sum(range(101)) - sum(a)
75


In an list 1-100 exactly one number is duplicate how do you find it?
y = list(range(101))
y.append(35)
sum(y) - sum (range(101))
35


Given two list, 1,2,3,4,5 and 2,3,1,0,5 find which number is not present in the second list?
a = [1,2,3,4,5]
b = [2,3,1,0,5]
list(set(a) - set(b)) # Difference a- b will return the value only in a and b -a will return the value only present in b
""" OR"""

for i in a:
    if i not in b:
        print (i)
4


How do you find second highest number in an integer array?
z = list(range(20))
sorted(set(z),reverse = True)[1]

""" OR """
z.sort(reverse = True)
z[1]
18


How to swap two numbers without using temp variable?
a = 24
b = 64
a,b = b,a 
print (a,b)
64 24
