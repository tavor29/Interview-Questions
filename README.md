# Interview-Questions
I Would like to present a few coding interiew questions that varry in difficulty, 
starting with the easiest.




I will provide an additional more efficeint or difficult solution. 
Hope this will help you code better, and even help land that next job! 




# Fizzbuzz:
The task is to code the game Fizzbuzz, using Python.

The rules of the game are:

Count from 1 to 100, while each time an int divides by 3 without a reaminder, return the word "Fizz" instead.

If n/5 without a remainder, it should return "buzz" instead.

If both are possible for n, return "Fizzbuzz".

Here are the best ways to complete the solution in my opinion:
The first coding problem is an easier one, 
and perhaps one of the most popular interview questions for junior/entry-level jobs.





# **First solution: The most primitive**


    for i in range(0,100):
    i += 1
    
      if i%3 == 0 and i%5 == 0:
          print("fizzbuzz")
      elif i%3 == 0:
          print("Fizz")
      elif i%5 ==0:
          print("Buzz")
      else:
          print(i)







# Improved:

    for i in range(1,100):
      a = ""
     if i % 3 == 0:
        a = a + "fizz"
     if i % 5 == 0:
        a = a+ "buzz"
     if a == "":
        a = i
     print a
  
  
  
  
  
  
  
  
 # Advanced: The one liner
 
    print("\n".join([("Fizz"*(not i%3)+"Buzz"*(not i%5)+str(i)*(i%3!=0 and i%5!=0)) for i in range(1,100)]))
    
    
    
    
    
    
    
 # The last improvment:
 
     print("\n".join(["Fizz"*(i%3==0)+"Buzz"*(i%5==0) or str(i) for i in range(100)]))
     
     
     
 # The correct output:
  
1
2
Fizz
4
Buzz
Fizz
7
8
Fizz
Buzz
11
Fizz
13
14
FizzBuzz
16
17
Fizz
19
Buzz
Fizz
22
23
Fizz
Buzz
26
Fizz
28
29
FizzBuzz
31
32
Fizz
34
Buzz
Fizz
37
38
Fizz
Buzz
41
Fizz
43
44
FizzBuzz
46
47
Fizz
49
Buzz
Fizz
52
53
Fizz
Buzz
56
Fizz
58
59
FizzBuzz
61
62
Fizz
64
Buzz
Fizz
67
68
Fizz
Buzz
71
Fizz
73
74
FizzBuzz
76
77
Fizz
79
Buzz
Fizz
82
83
Fizz
Buzz
86
Fizz
88
89
FizzBuzz
91
92
Fizz
94
Buzz
Fizz
97
98
Fizz


