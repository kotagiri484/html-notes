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


------------------------HTML and GIT---------------------------------------------------------
<!-- --------------------------------------------------basic commands----------------------------------------------------------------= -->
<!-- if you want to create a empty file in ==> git bash here 
            we're using ==> touch filename  [it will create empty file]
               if you want to edit the empty file 
                                 we're using ==> cat > filname [it will edit file] after adding the text we're using [ctrl + d] to save the file
-->
<!--  -->

<!--  if you want to create a folder  ==> mkdir  -->

<!--if you want to change the directory ==> cd  -->

<!-- if you want to check the local files ==> ls -->

<!-- if you want to delete the file ==> rm filename -->

<!-- if you want to open VS Code ==> open terminal and ==> code . ==> then enter -->

<!-- what is GIT  ==> GIT is source code management tool [SCM]  -->

<!-- what is GIT hub ==> it's centralized repository [cloud]-->

<!-- once we install the git in our local , when ever we right click we can able to see git bash here, and git gui here  -->

<!-- git is runnning in our local  and we need to send our code to git hub -->

<!-- if we want to initialize git in our project  
     we are using 
                 ==> git init [note : single time only]
==
-->

<!-- if you want to configure your name and email 
we're using 
==> git config --global user.name "username"
==> git config --global user.email "user email"-->

<!--  if you want to check the config list 
        we're using
                   ==> git config --list
-->

<!--  if you want to use any repository code in your local we need to clone the repository
  
          by using ==> git clone " repo url"
-->

<!-- what atre the phases to send data to git hub? those are as follows  
                  ==> 1.working directory 
                  ==> 2. staging/index   
                  ==> 3. local repository  -->

<!-- if you want to check the status of the changed files we are using this command ==> git status -->

<!--  how you identify your changed files are availble in which pahse ?
    if you run git status command ==> 
    if the file shows red color it is in working directory,
    if the file is showing greeen color it's in staging/index, 
    if it's showing nothing to commit and working tree clean it's in local repository -->

    <!-- if you want to create a branch 
    
    we're using  ==> git branch branchNmae
    if you want to checkout to that branch 
    we're using ==> git checkout branchName
    if you want to create andf checkout at the same time 
    we're using  ==> git checkout -b branchName
    if you want to check the branch list
    we're using ==> git branch
     
    note : always create a branch from base branch , don't create new branch from another new branch and ,maintain proper naming convesion for branch name [like ticket id and description]
    -->

<!-- if you want to tranfer data from working directory to staging/index
 we're using 
==> git add fileName  ==> it will transfer onely the mentioned file into staging/index
==> git add .  ==> it will transfer all modified files to staging/index -->

<!-- if you want to hide the content after tranfer data from local repository to staging/index
we're using ==> git stash [it will hide the data]
if you want to retrive the data which you are hidden 
if you want to check the hidden list
we're using ==> git stash --list
we're using ==> git statsh apply (or) ==> git stash pop
-->

<!-- if you want to tranfer data from  staging/index to local repository
        we're using 
                  ==> git commit -m " commit message it's optional and understandable for every one"
                  
-->


<!--  if you want to transfer our local repository data to git hub repo 
we're using
   ==> git push command  , in fisrt push it's looking for origin branch at that time we can use git push --set-upstream origin/brach'
   
   ==> if you want to take the latest code from repo 
    
   ==> we're using ==> git pull 
   ==> recommended:  always take the latest pull before pushing your changes
-->

<!-- to fetch the info ==> git fetch --all -->

<!-- if you want to combine one branch in another branch 
 
we're using ==> git merge (or)  ==> git rebase
-->

<!-- if you want to combine multiple commits in single commits
 we are using 
 ===> git rebase -i head~no of commits we need to sqaush  [after running this command it will open vi editor]
  ==> if incase you are not selected proper commits count then you need to run git rebase --abort command [it will stop the rebase]
 ===> if you want to edit text in vi editor we are using [shift + i (or) i  ==> these are for insert the data or text]
 ===> we need to check the commits which commits need to sqaush change the text pick to squash or s 
 ===> after inseting the content and if you want to save the inserting content and quit the vi editor we're using [:wq!]
 ===> after that again it will open vi editor and we need to change the commit message , for inserting we are using [shift + i (or) i ]
 ==> after inserting the commit message we need to save and quit the vi editor  ==> [:wq!]
 ==> the we need to run ==> git push -f to push your commits to repository [this is not recommended]
--> 


<!-- IMP questions -->

<!-- what's the difference between git rebase and git merge  -->





