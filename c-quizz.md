# C (Programming Language)

## Q1. Which Code sample will eventually cause the computer to run out of memory?

- a :

    ```c
    while(1)
    {
        char *smallString = (char *) malloc(10);
    }
    ```

- b :

    ```c
    long long number = 1;
        while(1)
        number *= 2;
    ```

- c :

    ```c
    while(1)
    {
        char hugeString[1000000L];
        memset(hugeString, 0, 1000000L);
    }
    ```

- d :

    ```c
    while(1)
    {
        long *bigArray = (long *) malloc(sizeof(long) * 1000);
        memset(bigArray, 1000000, 1000);
        free(bigArray);
    }
    ```

## Q2. What will this code print on the screen?

```c
int f1 (int a, int b)
{
    if (a > b)
    {
        printf("A is greater than B\n");
        return 1;
    }
    else
    {
        printf("B is greater than A");
        return 0;
    }
}

main()
{
    if (f1(20,10) || f1(10,20))
        printf("C is fun!\n");
}
```

- a :

```
A is greater then B
C is fun!
```

- b :

```
A is greater then B
B is greater then A
C is fun!
```

- c :

```
A is greater then B
B is greater then A
```

- d : Nothing is printed on Screen

## Q3. What is the name for calling a function inside the same function?

- a : recursion
- b : subfunction
- c : inner call
- d : infinite loop

## Q4. What does the declaration of variable c2 demonstrate?

```c
main(){
    char c1 ='a';
    char c2 = c1+10;
}
```

- a : character arithmetic
- b : undefined assignment
- c : type conversion
- d : invalid declaration

## Q5. What is this declaration an example of?

```c
struct s {
    int i;
    struct s *s1;
    struct s *s2;
};
```

- a : a node
- b : a linked list
- c : a stack
- d : a binary tree

## Q6. Header files are listed using the preprocessing directive #include, and can have one of the following formats: #include &lt;fileA&gt; or #include "fileB". What is the difference between these two formats?

- a : The preprocessor will try to locate fileA in same directory as the source file, and the fileB in a predetermined directory path.
- b : The preprocessor will try to locate fileA in the fixed system directory. It will try to locate fileB in the directory path designated by the -I option added to the command line while compiling the source code.
- c : The file using the fileA syntax must be system files, of unlimited number; fileB must be a user file at a maximun of one per source file.
- d : The preprocessor will try to locate fileA in a predetermined directory path. It will try to locate fileB in the same directory as the source file along with a custom directory path.

## Q7. Using a for loop, how could you write a C code to count down from 10 to 1 and display each number on its own line?

- a :

```c
for (int i = 0; i>=0, i--){
    printf("%d\n", i);
}//end of loop
```

- b :

```c
int i;
for (i=1; i<=10; i++){
    printf("%d", i);
}
```

- c :

```c
int i = 10;
while (i>0){
    printf("%d\n", i);
    i--;
}
```

- d :

```c
int i;
for (i= 10; i>0; i--){
    printf("%d\n", i);
}// end of loop
```

## Q8. What is not one of the reserved words in standard C?

- a : volatile
- b : typeof
- c : register
- d : typedef

## Q9. What does the program shown below return?

```c
int main(){
    int a=1, b=2, c=3, d=4;
    int x = a;
    if (a>b)
    if (b<c) x=b;
    else x=c;
    return(x);
}
```

- a : 1
- b : 3
- c : 2
- d : 0

## Q10. Using the Union declaration below, how many bytes of memory space will the data of this type occupy?

```c
union Cars {
    char make[20];
    char model[30];
    short year;
} car;
```

- a : 32
- b : 54
- c : 30
- d : 52

## Q11. In this code sample, what is not a problem for C compiler?

```c
main(){
    constant int PI = 3.14;
    printf("%f\n", pi);
}
```

- a : The value of PI needs to be set to 3.141593, not 3.14
- b : The declaration of PI needs to say const, not constant.
- c : The data type of PI needs to be float not int.
- d : The printf statement needs to use PI, not pi.

## Q12. Which is the smallest program to compile and run without errors?

- a : main()
- b : int main() {return 0;}
- c : main() { }
- d : main() { ; }

## Q13. What is optional in a function declaration?

- a : data type of parameters
- b : return type of function
- c : parameter names
- d : number of parameters

## Q14. C treats all devices, such as the display and the keyboard, as files. Which file opens automatically when a program executes?

- a : stdout
- b : stdio.h
- c : default.h
- d : string.h

## Q15. In which segment does dynamic memory allocation takes place?

- a : BSS Segment
- b : stack
- c : heap
- d : data segment

## Q16. Which function do you use to deallocate memory?

- a : dalloc()
- b : dealloc()
- c : release()
- d : free()

## Q17. In C language what are the basic building blocks that are constructed together to write a program?

- a : keywords
- b : identifiers
- c : tokens
- d : functions

## Q18. When is memory for a variable allocated?

- a : during the assigment of the variable
- b : during the initialization of the variable
- c : during the declaration of the variable
- d : during the definition of the variable

## Q19. C uses the call by value method to pass arguments to functions. How can you invoke the call by reference method?

- a : by using pointers
- b : by declaring functions separately from defining them
- c : by using recursive functions
- d : by using global variables

## Q20. A union allows you to store different `___` in the same `___`.

- a : Objects; Structure
- b : Variables; Declaration
- c : Data types; Memory space
- d : Arrays; Header file

## Q21. What is the output of this program?

```c
main() {
    char c1='a' , c2='A';
    int i=c2-c1;
    printf("%d", i);
}
```

- a : 32
- b : Runtime error
- c : -32
- d : 0

## Q22. What is the difference between scanf() and sscanf() functions?

- a : The scanf() function reads data formatted as a string; The sscanf() function reads string input from the screen.
- b : The scanf() function reads formatted data from the keyboard; The sscanf() function reads formatted input from a string.
- c : The scanf() function reads string data from the keyboard; The sscanf() function reads string data from a string.
- d : The scanf() function reads formatted data from a file; The sscanf() function reads input from a selected string

## Q23. What is not a valid command with this declaration?

```c
char *string[20] = { "one", "two", "three"};
```

- a : `printf("%c", string[1][2]);`
- b : `printf("%s", string[1][2]);`
- c : `printf("%s", string[1]);`
- d : `printf(string[1]);`

## Q24. What is the expression player->name equivalent to?

- a : `player.name`
- b : `(*player).name`
- c : `*player.name`
- d : `player.*name`

## Q25. Which program will compile and run without errors?

- a :

```c
main() {
    for(i=0; i<10; i++) ;
}
```

- b :

```c
main() {
int i=0;
    for(; i<10; i++) ;
}
```

- c :

```c
main() {
    int i;
    for(i=0; i<j; i++) ;
}
```

- d :

```c
main() {
int i;
    for (i= 10; i<10; i++)
}
```

## Q26. What does this function call return?

```c
1 main() { float x = f1(10, 5); }
2 float f1(int a, int b) { return (a/b); }
```

- a : 2
- b : 2.000000
- c : a runtime error
- d : a compiler error

## Q27. What does this program create?

```c
#include <stdio.h>
int main() {
    int *p = NULL;
    return 0;
}
```

- a : a runtime error
- b : a NULL pointer
- c : a compile error
- d : a void pointer

## Q28. What is an alternative way to write the expression (\*x).y?

- a : There is no equivalent.
- b : x->y
- c : \*x->y
- d : y->x

## Q29. Compile time errors are static errors that can be found where in the code?

- a : in declarations and definitions
- b : in functions and expressions
- c : in syntax and semantics
- d : in objects and statements

## Q30. File input and output (I/O) in C is heavily based on the way it is done `___`?

- a : in Unix
- b : in C++
- c : in C#
- d : in DOS

## Q31. What does the strcmp(str1, str2); function return?

- a : 0 if str1 and str2 are the same, a negative number if str1 is less than str2, a positive number if str1 is greater than str2
- b : true (1) if str1 and str2 are the same, false (0) if str1 and str2 are not the same
- c : true (1) if str1 and str2 are the same, NULL if str1 and str2 are not the same
- d : 0 if str1 and str2 are the same, a negative number if str2 is less than str1, a positive number if str2 is greater than str1

## Q32. What is the output of this program?

```c
int a=10, b=20;
int f1(a) { return(a*b); }
main() {
printf("%d", f1(5));
}
```

- a : 100
- b : 200
- c : 5
- d : 50

## Q33. Which is _not_ a correct way to declare a string variable?

- a : `char *string = "Hello World";`
- b : `char string = "Hello World";`
- c : `char string[20] = {'H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd'};`
- d : `char string[] = "Hello World";`

## Q34. Which choice is an include guard for the header file mylib.h?

- a :

```c
#ifdef MYLIB_H
#undef MYLIB_H

// mylib.h content

#endif /* MYLIB_H */
```

- b :

```c
#ifndef MYLIB_H
#define MYLIB_H

// mylib.h content

#endif /* MYLIB_H */
```

- c :

```c
#define MYLIB_H
#include "mylib.h"

#undef MYLIB_H
```

- d :

```c
#ifdef MYLIB_H
#define MYLIB_H

// mylib.h content

#endif /* MYLIB_H */
```

## Q35. How many times does the code inside the while loop get executed in this program?

```c
main(){
 int x=1;
 while(x++<100){
    x*=x;
    if(x<10) continue;
    if(x>50) break;
 }
}
```

- a : 100
- b : 3
- c : 5
- d : 50

## Q36. File input and output (I/O) in C is done through what?

- a : syntax-driven components
- b : native interfaces
- c : system objects
- d : function calls

## Q37. Directives are translated by the?

- a : Pre-processor
- b : Compiler
- c : Linker
- d : Editor

## Q38. The main loop structures in C programming are the for loop, the while loop, and which other loop?

- a : do...while
- b : for...in
- c : repeat...until
- d : do...until

## Q39. By default, C Functions are what type of functions?

- a : global
- b : static
- c : library
- d : system

## Q40. You have written a function that you want to include as a member of structure a. How is such as structure member defiened?

- a :

```c
struct a {
    void *f1;
};
```

- b :

```c
struct a {
    void (*f1)();
};
```

- c :

```c
struct a {
    *(void *f1)();
};
```

- d :

```c
struct a {
    void *f1();
};
```

## Q41. A Stack data structure allows all data operations at one end only, making it what kind of an implementation?

- a : FIFO
- b : LIFO
- c : LILO
- d : LOLI

## Q42. What does this program display?

```c
main(){
    char *p = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
    int i;
    for (i=0;i<5;i++) *p++; *p++;
    printf("%c",*p++);
}
```

- a : K
- b : M
- c : H
- d : G

## Q43. Describe the relationship between lvalue and rvalue.

- a : An lvalue may appear only on the left-hand side of an assignment; an rvalue may appear only on the right-hand side.
- b : An lvalue may appear only on the left-hand side of an assignment; an rvalue may appear on either the left-hand or right-hand side.
- c : An lvalue and an rvalue may appear on either left-hand or right-hand side of an assignment.
- d : An lvalue may appear on the left-hand or right-hand side of an assignment; an rvalue may appear only on the right-hand side.

## Q44. Which operator is used to access the address of a variable?

- a : `%`
- b : `**`
- c : `*`
- d : `&`

## Q45. Which add function properly returns the updated value of result?

- a :

```c
void add (int a, int b, int *result)
{
    *result = a+b;
}

main()
{
    int a = 10;
    int b = 20;
    int result = 0;

    add(a,b,&result);
}
```

- b :

```c
void add (int a, int b, int result)
{
    result = a+b;
}

main()
{
    int a = 10;
    int b = 20;
    int result = 0;

    add(a,b,result);
}
```

- c :

```c
void add (int a, int b, int *result)
{
    result = a+b;
}

main()
{
    int a = 10;
    int b = 20;
    int result = 0;

    add(a,b,result);
}
```

- d :

```c
void add (int *a, int *b, int *result)
{
    result = a+b;
}

main()
{
    int a = 10;
    int b = 20;
    int result = 0;

    add(*a,*b,*result);
}
```

## Q46. Consider the number of the Fibonacci series below 100: 0,1,1,2,3,5,8,13,21,34,55,89. Which piece of code outputs the sequence?

- a :

```c
void fibonacci(int a, int b)
{
    int c = a+b;

    if(a>100)
       return;

    printf("%d", a);

    fibonacci(a,b);
}

int main()
{
    fibonacci(0,1);
}
```

- b :

```c
void fibonacci(int a, int b)
{
    int c = a+b;

    if(a>100)
       return;

    printf("%d", b);

    fibonacci(a,c);
}

int main()
{
    fibonacci(0,1);
}
```

- c :

```c
void fibonacci(int a, int b)
{
    int c = a+b;

    if(a>100)
       return;

    printf("%d", a);

    fibonacci(b,c);
}

int main()
{
    fibonacci(0,1);
}
```

- d :

```c
void fibonacci(int a, int b)
{
    int c = a+b;

    if(a>100)
       return;

    printf("%d", c);

    fibonacci(b,c);
}

int main()
{
    fibonacci(0,1);
}
```

## Q47. Which is _not_ a storage class specifier?

- a : `intern`
- b : `extern`
- c : `register`
- d : `static`

## Q48. Which line of code, after execution, results in `i` having the value of 1?

- a : `for(i=1; i<=1; i++);`
- b : `for(i=1; i=10; i++);`
- c : `for(i=1; i==10; i++);`
- d : `for(i=10; i>=1; i--);`

## Q49. What is the value of variable c at the end of this program?

```
1 main() {
2   int a, b, c;
3   a=10; b=50;
4   c=a * b % a;
5 }
```

- a : 50
- b : 5
- c : 0
- d : 500

## Q50. What is _not_ one of the basic data types in C

- a : long double
- b : unsigned char
- c : array
- d : float

## Q51. What is the member access operator for a structure?

- a : ,
- b : []
- c : .
- d :

## Q52. What standard data type provides the smallest storage size and can be used in computations?

- a : char
- b : float
- c : int
- d : short

## Q53. what does the ctype tolower() function do?

- a : It returns TRUE for lowercase letters of the alphabet.
- b : It ensures that text output uses only ASCII values (0 through 127).
- c : It returns FALSE for lowercase letters of the alphabet.
- d : It converts an uppercase letter of the alphabet to lowercase.

## Q54. Void pointer _vptr_ is assigned the address of float variable _g_. What is a valid way to dereference _vptr_ to assign its pointed value to a float variable named _f_ later in the program?

```c
float g;
void *vptr=&g;
```

- a : `f=(float *)vptr;`
- b : `f=*(float *)vptr;`
- c : `f=*(float)vptr;`
- d : `f=(float)*vptr;`

## Q55. The dynamic memory allocation functions are defined in which system header file ?

- a : stdio.h
- b : stdlib.h
- c : limits.h
- d : stddef.h

## Q56. A function is a set of **\_**.

- a : declarations
- b : statements
- c : variables
- d : objects

## Q57. How are static functions different from global functions?

- a : Static functions must be declared in advance of being defined.
- b : Static functions must be declared is a separate header file.
- c : Static functions always return the same value.
- d : Static functions can be accessed only in the file where they are declared.

## Q58. Which code example creates the string "Hello Mars" in storage buffer `hello`.

- a :

```c
    char hello[25];
    strcpy(hello, "Hello ");
    strcpy(hello, "Mars");
```

- b :

```c
    char hello[25];
    char *p;
    strcpy(hello, "Hello World");
    p = hello;
    p +=6;
    strcpy(p, "Mars");
```

- c :

```c
    char *hello;
    strcpy(hello, "Hello World");
    hello+=6;
    strcpy(hello, "Mars");
```

- d :

```c
    char hello[25];
    strcpy(hello, "Hello World");
    strcpy(*hello[6], "Mars");
```

## Q59. If you use the fopen() function with the "a" mode, what happens if the named file doesn't exist?

- a : The file is created and opened for reading.
- b : The file is created and opened for writing.
- c : The fopen() function returns a NULL indicating that the operation has failed.
- d : The file is created and opened for both writing and reading

## Q60. What does this function return?

```c
int fl(int a, int b) { return(a>b?a:b); }
```

- a : compiler error
- b : the smaller value of the two passed parameters
- c : runtime error
- d : the greater value of the two passed parameters
