# Interview-Questions
I Would like to present a few coding interiew questions that varry in difficulty, 
starting with the easiest.




I will provide an additional more efficeint or difficult solution. 
Hope this will help you code better, and even help land that next job! 




Fizzbuzz:
The first coding problem is an easier one, 
and perhaps one of the most popular interview questions for junior/entry-level job.





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
    if i % 2 == 0:
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
