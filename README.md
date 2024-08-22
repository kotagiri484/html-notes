javascript features- open source
                     cross platform
                     synchronous
                     single threaded
----------------------------------------------------------------------------------------
Scope -> lifetime visibility of an variable

javascript scopes- global scope
                   functional scope                                                               
                   block scope

global scope- variables declared globally(outside any function)have global scope.                      var can be hoisted
-> global variables can be accessed from anywhere in a javascript program
-> variables declared with var,let&const are quite similar when declared outside a block.

functional scope- 
-> javascript has function scope:each function creates new scope.
variables defined inside a function are not accessible(visible)from outside the function.
variable declared  with var,let & const are quiet similar when declared inside a function.
they all have function scope
-----------------------------------------------------------------------------------------


Hosting -> its javascript interpreter behaviour,it takes all the declaration to the top

----------------------------------------------------------------------------------------------

Temporial deadzone ->whenever we are declaring with let or const keywords, we cannot access before initialization,after initialization only we can access

-------------------------------------------------------------------------------------------------------

Global executaion context->
-----------------------------------------------------------------------------------------------------------


Shadowing- > Now, when a variable is declared in a certain scope having the same name defined on its outer scope and when we call the variable from the inner scope, the value assigned to    the variable in the inner scope is the value that will be stored in the variable in the memory space. This is known as Shadowing or Variable Shadowing.
------------------------------------------------------------------------------------------------------------------------------------------------------------
-------------
Block -> This scope restricts the variable that is declared inside a specific block, from access by the outside of the block.
example --> {
            
            }
-------------------------------------------------------------------------------------------------------------------------------------

Closure -> inner function can able to access the parent function local variables by itself but 
          vice versa is not possible is a called closure.
        ->function  bundle together with it's lexical environment.
-------------------------------------------------------------------------------------------------------------------------------------

Lexical environment-
Lexixal -> sequence
---------------------------------------------------------------------------------------------
Function ==> logical group of one or more expressions

Ways to write a function:

==> function declaration (can be hoisted)
==> function expression (can't hoisted)
==> arrow function (can't hoisted)
-----------------------------------------------------------------------------------------
shallow copy -> 
Deep copy ->
----------------------------------------------------------------------------------
Data types --> primitive(string,boolean,number) nd non-primitive(array,object)
----------------------------------------------------------------------------------
ECMA - european computers manufacturer association
 ->standard for javascript

-------------------------------------------------------------------------------------
                       Array Methods & Use Cases
 ------------------------------------------------------------------------------------
array methods and use cases
---------------------------------------------------------------------------------------
push ==> to add element in end of the array
---------------------------------------------------------------------------------------
pop  ==> to remove element from end of the array
---------------------------------------------------------------------------------------
 unshift  ==> to add element starting of the array
---------------------------------------------------------------------------------------
shift  ==> to remove element from starting of the array
---------------------------------------------------------------------------------------
slice  ==> it will select from one point to another point.  syntax ==> arrname.slice(startindex, endIndex)
---------------------------------------------------------------------------------------
 splice ==> by using splice we can able to add and remove elements from the array . syntax ==> arrname.splice(startindex,removeCount, items to add in the array)
---------------------------------------------------------------------------------------
 delete ==> to delete value from the array. syntax ==> delete indexof array   eg : delete arraName[index]
---------------------------------------------------------------------------------------
sort   ==> to sort the array
---------------------------------------------------------------------------------------
replace  ==> to repalce word with another word in string
---------------------------------------------------------------------------------------
trim   == > it will remove spaces from start and end of the string
---------------------------------------------------------------------------------------
 template literals  ==> it allows us to write string and expressions in the same line. denoted by (``)back ticks.  eg : let a=10; let str = ` hello world ${a}`

 let value = 100;

let str = " ${value} New Delhi, Saket \n F-11, Select CITYWALK \n District Centre, Saket\n New Delhi, Delhi, 110017\n000800 040 4503"
console.log(str)

let str1= ` ${value} New Delhi, Saket
F-11, Select CITYWALK
District Centre, Saket
New Delhi, Delhi, 110017
000800 040 4503`
---------------------------------------------------------------------------------------
 convert string into array  =>  by using split method , by using [...]
---------------------------------------------------------------------------------------
 split  ==> split the string into array 
---------------------------------------------------------------------------------------
 spread operator(...)   ==> it will expands the array
---------------------------------------------------------------------------------------
 reverse   => it will revrse the array of elements
---------------------------------------------------------------------------------------
 join   ==> it will join the array into string
---------------------------------------------------------------------------------------
 fill   ==> it will replace mentioned value from start index to end index
---------------------------------------------------------------------------------------
 concat ==> it will combine the values or arrays
---------------------------------------------------------------------------------------
let arr = [1,2,3]
let arr1 = [4,5,6]
let arr2= arr.concat(arr1)
console.log(arr2)