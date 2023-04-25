Part1                     
The code for StringServer:
![Image](code1.png)                           
                               
Two screenshots of using ```/add-message``` :                                 
![Image](screenshot-2.png)                                        

Method: handleRequest.                        
The relevant arguments are parameters and path.                       
```parameter[1]``` changed since it is related to the return output.

![Image](screenshot-1.png)                  
Method: handleRequest.                      
The relevant arguments are parameters and path.                              
```parameter[1]``` changed since it is related to the return output.

                                                   
Part2                      
A failure-inducing input for the buggy program:                    
```ArrayTests. java:1: error: package org- junit does not exist import static org.junit.Assert.*;
ArrayTests. java:2: error: package org- junit does not exist import org-junit.*;
MethodsTests. java:1: error: package org. junit does not exist import static org. junit.Assert.*;
MethodsTests. java:2: error: package org. junit does not exist import org-junit.*;
ArrayTests java:5: error: cannot find symbol
@Test
symbol:
class Test location: class ArrayTests
ArrayTests.java: 13: error: cannot find symbol
@Test
symbol:
class Test location: class ArrayTests
MethodsTests-java:5: error: cannot find symbol
@Test
symbol:
class Test location: class MethodsTests
MethodsTests. java: 10: error: cannot find symbol
@Test
symbol:
class Test location: class MethodsTests
MethodsTests. java: 15: error: cannot find symbol
@Test
symbol:
class Test location: class MethodsTests
ArrayTests. java:9: error: cannot find symbol assertArrayEquals(new int[I{ 3 }, input1) ;
symbol:
method assertArrayEquals (int [I , int [])
location: class ArrayTests
ArrayTests. java: 16: error: cannot find symbol
assertArrayEquals (new int []{ }, ArrayExamples. reversed (input1)) ;
symbol:
method assertArrayEquals (int [I, int [I)
location: class ArrayTests
MethodsTests. java: 8: error: cannot find symbol
assertEquals (EvensExample. sumEvenIndices (input1), 19) ;
symbol:
method assertEquals (int, int)
location: class MethodsTests
MethodsTests. java:13: error: cannot find symbol
assertEquals (EvensExample. sumEvenIndices ( input1), 52) ; symbol:
method assertEquals (int, int)
location: class MethodsTests
MethodsTests. java: 18: error: cannot find symbol
assertEquals (EvensExample. sumEvenIndices (input1), 24);
symbol:
method assertEquals (int, int)
location: class MethodsTests
14 errors
```                                   
This is the failure-inducing input for the buggy program, since MAC and Windows use different system, so different system have different associated code. Since I'm using mac and the command I used was for Windows, the compiler cannot recognize the two .jar files in the lib directory, which are ```lib/hamcrest-core-1.3.jar``` and ```lib/junit-4.13.2.jar;lib```. Hence, if there is any junit in the code, then the terminal will shows error.                                        
                                                         
Part3                      
In week2, I leanred how to build and run a server. In week3, I learned the difference code of Junit test for Mac users and Window users. Moreover, for the failure inducing input, we need to check it carefully on the for loop since it can be crashed even if there is a little mistake on the calculator. 
