# Introducion
- Ye notes un k lie perfect ha jo programming paradigm me reh chuke hain aur python ko explore krna chah rahe hain

- Is me mene Data types aur un k methods ki kuch examples show ki hain jis se apko har datatype ka work flow easily smjh ajyega  


Agar ap kisi bhi programming language se waqif ho aur sirf Python ke syntax explore karna chahte ho, to yeh file ap k liye perfect hai. Maine isme zyadatar **syntax** per focus kiya hai, taake ap bina kisi extra theory ke seedha Python likhna shuru kar sako. Har concept ko simple aur mazedar tareeke se explain kiya gaya hai, taake bore bhi na ho aur samajhna bhi easy rahe.

### 📌 **What’s in this file?**

✅ **Easy-to-understand syntax** – Har concept ko simple tareeke se likha gaya hai.  
✅ **Examples ke saath explanation** – Sirf theory nahi, balki har topic ka **practical** use bhi dikhaya gaya hai.    
✅ **Engaging style** – Aise likha gaya hai ke parhte waqt bore bhi nahi hoge!

---

### ❌ **What’s NOT in this file?**

🚫 **No lengthy programming exercises** – Sirf core syntax aur concepts hain, koi lambi coding problems nahi.  
🚫 **No unnecessary theory** – Har cheez **direct aur to-the-point** hai.  
🚫 **No hard and fast logic** – Yeh file sirf Python ka structure samajhne ke liye hai, complex algorithms nahi hain.  


# Data Types

## Numbers

```python
import random 
# import ka keyword use kr k ham libraries import krte hain jis me powerful methods hote hai jo k ham '.' laga kr access krte hain
random.random() # generate random number
random.randint(1,10) # generate random integer between 1 and 10
random.choice(list) #randomly choose one element from list (list is defined below)
random.shuffle(list) #randomly shuffle the elements in list (list is defined below)







0.3 + 0.3 + 0.3 -0.9  #ulta pulta (unexpected) result

#behtr tariqa niche wala ha niche dekho niche

from decimal import Decimal

Decimal('0.3') +Decimal('0.3')+Decimal('0.3')-Decimal('0.3')
#perfect output

```





## String



```python

len("Hello") #output:5 #length of string
"Hello".lower() #hello
"Hello".upper() #HELLO
"    Hello    ".strip() #Hello #remove extra spaces
"Hello World".replace("World" , "Saad") #"Hello Saad"


# string to list 


"Dhanya , Pudina , Adrak , Gobi ".split() 
#output: ['Dhanya', ',', 'Pudina', ',', 'Adrak', ',', 'Gobi']

#by default splited by <space>

#but we can mention like:
"Dhanya , Pudina , Adrak , Gobi ".split(" , ") 
#output:['Dhanya', 'Pudina', 'Adrak', 'Gobi ']



# list to string 
sabzi = "Dhanya , Pudina , Adrak , Gobi ".split(" , ") 
print(sabzi) #output:['Dhanya', 'Pudina', 'Adrak', 'Gobi ']
#ye split hgya ha ab dubara list banate hain


" ".join(sabzi) # bich me space k lie  
#output:Dhanya Pudina Adrak Gobi 

",".join(sabzi) # bich me , k lie  
#output:Dhanya,Pudina,Adrak,Gobi 



"Hello World".find("World") #output: 6  world starts from 6 position

"Hello World".find("Chachu") #output: -1  not found

"Hello World World World".count("World") #output:3


```

### Something Unique (Ise zaroor try krna)

``` python
my_class = "Sunday afternoon"
my_teacher = "Ali jawwad"

sentence = "Meri class {} wali ha aur muje {} prhate hain"
print(sentence) #output:Meri class {} wali ha aur muje {} prhate hain


proper_sentence = sentence.format(my_class,my_teacher)  

print(proper_sentence)#ouput:Meri class Sunday afternoon wali ha aur muje Ali jawwad prhate hain


# ye to apne codebase me apni class aur teacher k sath try krna banta h ;)
```

### Slicing to btai hi nahi
- slicing me kuch nahi ha ye self practice se ziada acha smjh ayega

```python

numbers = "0123456789"
print(numbers[:])
print(numbers[0:11])
print(numbers[2:6])
print(numbers[::2])
print(numbers[::-1])
print(numbers[-1:-5:-1])

#[1stpara:2nd Para:3rd Para] bs 3no me value change kro aur investigation study krte jao :)

```



## List


```python
#add in last of list
sabzi = ["Dhanya" , "Pudina" , "Adrak" , "Gobi"] 

# aloo nahi laye?....

sabzi.append("aloo")
print(sabzi)
#ouput: ["Dhanya" , "Pudina" , "Adrak" , "Gobi", "aloo"]

# Ye lo, le aaya aloo bhi!

# Mene to sirf pucha tha aloo nahi chayie


sabzi.pop() #ouput:Aloo
# pop last element ko remove kr k return kr deta ha


#dubara jao aur sabzi k saath fruits bhi le aao
fruits = ["apple","keenu","anaar"]

all_list = sabzi + fruits

print(all_list)


#insert at position
#adrak se pehle lehsan add krdete hain 
sabzi.insert(2,"Lehsan")
print(sabzi)
#ouput: ["Dhanya" , "Pudina" , "Lehsan" ,"Adrak" , "Gobi", "aloo"]





#python magic

squared_number = [x**2 for x in range(1,11)]
print(squared_number)
#run it yourself to see magic
# it has defined in loop topic

```




## Dictionaries


- if you are from *javascript* background so it is similar to **objects** in *javascript*

```python

sabzi_with_quantity = {
    "one" : "aloo",
    "five" : "Bengal",
    "three" : "Pudina",
    "two" : "dhanya",
}


print(sabzi_with_quantity.items())
#output:dict_items([('one', 'aloo'), ('five', 'Bengal'), ('three', 'Pudina'), ('two', 'dhanya')])

sabzi_with_quantity["five"] # Bengal
sabzi_with_quantity.get("five") # Bengal


# used for mostly in loops(!loops are defined next file)
# like:


for quantity in sabzi_with_quantity:
    print(quantity )

one 
five 
three 
two 

for sabzi in sabzi_with_quantity:
    print(sabzi , sabzi_with_quantity[sabzi])
#ouput:
"""
one aloo
five Bengal
three Pudina
two dhanya

"""

for quanitity,sabzi in sabzi_with_quantity.items():
    print(quanitity,sabzi)
#ouput:
"""
one aloo
five Bengal
three Pudina
two dhanya

"""




#dictionaries construct krne ka aik aur method bhi h
teachers = ["Sir Asharib", "Sir Hamza", "Sir Anas", "Sir Ali", "Sir Okasha""Sir Mubasir" ] 
teaching = "Acha prhate hain"

teacher_with_teaching = dict.fromkeys(teachers,teaching)

print(teacher_with_teaching)

#output:
# {'Sir Asharib': 'Acha prhate hain', 
# 'Sir Hamza': 'Acha prhate hain', 
# 'Sir Anas': 'Acha prhate hain', 
# 'Sir Ali': 'Acha prhate hain', 
# 'Sir OkashaSir Mubasir': 'Acha prhate hain'}








#now its time for python magic

squared_num = {x:x**2 for x in range(1,11)}
print(squared_num)
#run it yourself to see magic
# !Loops has discussed in loop section





```


## Tuples

- Tuple List hi hain yar bs immutable ha change nhi hoskti 

```python
sabzi = ("Dhanya" , "Paalak" , "Adrak" , "Gobi") #Tuple syntax


#wahi list ki trah

sabzi[0] # Dhanya
sabzi[1] # Paalak
sabzi[2] # Adrak
sabzi[3] # Gobi


#lekin:

#mene dhanya nhi pudina mangwaya tha

sabzi[0] = "Pudina" # error
# sorry jo agya us se kam chlao me koi list nhi jo change krlu


```


- bas yahi ha tuple me values overwrite nhi hoti 





## Sets

- Syntax curly braces {} wala ha 
- Is me **duplicate values nahi hoti**.
- **Unordered hota hai**, matlab jo order me daloge, zaroori nahi waisa hi mile.

```python
sabzi = {"Dhanya", "Pudina", "Adrak", "Gobi", "Adrak", "Pudina"}
print(sabzi)  # Output: {'Dhanya', 'Pudina', 'Adrak', 'Gobi'}
# duplicate values gayab! 

sabzi.add("Aloo")
print(sabzi)  # {'Dhanya', 'Pudina', 'Adrak', 'Gobi', 'Aloo'}
# new item add ho gaya! 

sabzi.remove("Dhanya")
print(sabzi)  # {'Pudina', 'Adrak', 'Gobi', 'Aloo'}



# han ye mathemetics wala set ha

sabzi = {"Dhanya", "Pudina", "Adrak"}
fruits = {"Apple", "Keenu", "Pudina"}

print(sabzi | fruits)  # Union - sab mil jaye! {'Dhanya', 'Pudina', 'Adrak', 'Apple', 'Keenu'}
print(sabzi & fruits)  # Intersection - jo dono me common hai! {'Pudina'}
print(sabzi - fruits)  # Difference - jo sirf sabzi me hai! {'Dhanya', 'Adrak'}



```

## Data Types End
- datatypes filhal k lie itna hi aage ap practice k sathsath sikh jaoge  
#### wo chiz jo sirf python me ha (jahan tak me dekh ska)
- **indentations:** python me scope define krne k lie curly braces ki need nnahi hoti ham simple <Tab> ya kuch <spaces> dete hain 
for example:
In **Javascript** we define our if statement like this:
```javascript
a = 5
b = 5
if(a==b){
    console.log("a is equal to b");    
}
```

but in python:

```python
a=5
b=5
if a == b:
    print("a is equal to b")

# we don't use curly braces for scope 
```


## Conditional Problems

- Ab programming to aati ha ham ko bilawaja condition k syntax me time waste ho behtr ha k direct 1 2 problems dekh lo
- Niche 2 problems k arrow pr click kr k expand kr lo 

<details>
<summary> 1. Grade Calculator
</summary>
Problem: Assign a letter grade based on a student's score: A (90-100), B (80-89), C (70-79), D (60-69), F (below 60).

### Solution
``` python
score = 185

if score >= 101:
    print("Please verify your grade again")
    exit()

if score >= 90:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
elif score >= 60:
    grade = "D"
else:
    grade = "F"

print("Grade: ", grade)
```

</details>




<details>
<summary>2. Leap Year Checker
</summary>
Problem: Determine if a year is a leap year. (Leap years are divisible by 4, but not by 100 unless also divisible by 400).

```python
year = 2023

if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):
    print( year, " is a leap year")
else:
    print(year, "is NOT a leap year")

```

</details>







## Loops

- Loops ka kaam simple hai: code ko repeat karna jab tak condition satisfy hoti rahe. Python me loops likhna easy hai,
- mene just chota sa code likha ha isko runnkrlo smjh ajyega(agar programming se aware ho to)

### For Loop
```python
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    print(num)

for num in range(1,6):
    print(num)

  
```

### While Loop
```python
x = 0
while x < 5:
    print(x)
    x += 1  # x ko 1 se increment kar rahe hain
```

## Python me switch nahi h kia???

- Q nhi bhai sab ha bs naming difference ha
- python me **switch** nahi **match** bolte hain 
### For Example
```python
x = 2
match x:
    case 1:
        print("One")
    case 2:
        print("Two")
    case _:
        print("Something else")

```



## Mutable and Immutable
Changeable or Inchangeable (respectively)
- ye theoritical topic ha jis me apko back of te stage sochna hota ha is lie meri recommendation ye ha k koi video dekh lo 

let's example integer is immutable(unchangable) so:
``` python
x = 10
y = x
print(x,y) #10 10
#let's change theh value
x = 15
print(x) # 15
print(y) # 10 not 15 

```



# In Last
Bas khtm hui apki core python😊
You are now ready to dive in deep
- Agar aapko programming ka basic idea hai, to ye file aapke liye ek shortcut hai. Lekin agar aap bilkul naye hain, to pehle **basic concepts** samajhna zaroori hai.

- Python seekhne ka sabse acha tareeqa **practice** hai. Jitna **explore** karoge, utna seekhne ko milega. **Happy Coding!** 



