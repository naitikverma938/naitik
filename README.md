## C (Programming Language)

#### Q1. Which Code sample will eventually cause the computer to run out of memory?

- [x] :

```c
while(1)
{
    char *smallString = (char *) malloc(10);
}
```

- [ ] :

```c
long long number = 1;
    while(1)
    number *= 2;
```

- [ ] :

```c
while(1)
{
    char hugeString[1000000L];
    memset(hugeString, 0, 1000000L);
}
```

- [ ] :

```c
while(1)
{
    long *bigArray = (long *) malloc(sizeof(long) * 1000);
    memset(bigArray, 1000000, 1000);

    (bigArray);
}
```

#### Q2. What will this code print on the screen?

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

- [x] :

```
A is greater then B
C is fun!
```

- [ ] :

```
A is greater then B
B is greater then A
C is fun!
```

- [ ] :

```
A is greater then B
B is greater then A
```

- [ ] Nothing is printed on Screen

#### Q3. What is the name for calling a function inside the same function?

- [x] recursion
- [ ] subfunction
- [ ] inner call
- [ ] infinite loop

[Reference](https://www.cprogramming.com/tutorial/c/lesson16.html)

#### Q4. What does the declaration of variable c2 demonstrate?

```c
main(){
    char c1 ='a';
    char c2 = c1+10;
}
```

- [x] character arithmetic
- [ ] undefined assignment
- [ ] type conversion
- [ ] invalid declaration

[Reference](https://tutorialspoint.dev/language/c/character-arithmetic-c-c)

#### Q5. What is this declaration an example of?

```c
struct s {
    int i;
    struct s *s1;
    struct s *s2;
};
```

- [x] a node
- [ ] a linked list
- [ ] a stack
- [ ] a binary tree

#### Q6. Header files are listed using the preprocessing directive #include, and can have one of the following formats: #include &lt;fileA&gt; or #include "fileB". What is the difference between these two formats?

- [ ] The preprocessor will try to locate fileA in same directory as the source file, and the fileB in a predetermined directory path.
- [ ] The preprocessor will try to locate fileA in the fixed system directory. It will try to locate fileB in the directory path designated by the -I option added to the command line while compiling the source code.
- [ ] The file using the fileA syntax must be system files, of unlimited number; fileB must be a user file at a maximun of one per source file.
- [x] The preprocessor will try to locate fileA in a predetermined directory path. It will try to locate fileB in the same directory as the source file along with a custom directory path.

[Reference](https://www.geeksforgeeks.org/difference-between-include-and-include-in-c-c-with-examples/#:~:text=The%20difference%20between%20the%20two,be%20included%20in%20the%20code.&text=%23include%20is%20for%20pre%2Ddefined%20header%20files.)

#### Q7. Using a for loop, how could you write a C code to count down from 10 to 1 and display each number on its own line?

- [ ] :

```c
for (int i = 0; i>=0, i--){
    printf("%d\n", i);
}//end of loop
```

- [ ] :

```c
int i;
for (i=1; i<=10; i++){
    printf("%d", i);
}
```

- [ ] :

```c
int i = 10;
while (i>0){
    printf("%d\n", i);
    i--;
}
```

- [x] :

```c
int i;
for (i= 10; i>0; i--){
    printf("%d\n", i);
}// end of loop
```

#### Q8. What is not one of the reserved words in standard C?

- [ ] volatile
- [x] typeof
- [ ] register
- [ ] typedef

[Reference](https://www.ibm.com/docs/en/adfz/developer-for-zos/14.2.0?topic=programs-c-reserved-keywords)

#### Q9. What does the program shown below return?

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

- [x] 1
- [ ] 3
- [ ] 2
- [ ] 0

#### Q10. Using the Union declaration below, how many bytes of memory space will the data of this type occupy?

```c
union Cars {
    char make[20];
    char model[30];
    short year;
} car;
```

- [ ] 32
- [ ] 54
- [x] 30
- [ ] 52

#### Q11. In this code sample, what is not a problem for C compiler?

```c
main(){
    constant int PI = 3.14;
    printf("%f\n", pi);
}
```

- [x] The value of PI needs to be set to 3.141593, not 3.14
- [ ] The declaration of PI needs to say const, not constant.
- [ ] The data type of PI needs to be float not int.
- [ ] The printf statement needs to use PI, not pi.

#### Q12. Which is the smallest program to compile and run without errors?

- [ ] main()
- [x] int main() {return 0;}
- [ ] main() { }
- [ ] main() { ; }

[Reference](https://www.beningo.com/150-the-wolrds-shortest-c-program/)

#### Q13. What is optional in a function declaration?

- [ ] data type of parameters
- [ ] return type of function
- [x] parameter names
- [ ] number of parameters

[Reference](https://www.cprogramming.com/tutorial/c/lesson4.html)

#### Q14. C treats all devices, such as the display and the keyboard, as files. Which file opens automatically when a program executes?

- [x] stdout
- [ ] stdio.h
- [ ] default.h
- [ ] string.h

#### Q15. In which segment does dynamic memory allocation takes place?

- [ ] BSS Segment
- [ ] stack
- [x] heap
- [ ] data segment

[Reference](http://www.it.uc3m.es/pbasanta/asng/course_notes/dynamic_memory_heap_en.html#:~:text=The%20dynamic%20memory%20that%20is,reads%20a%20set%20of%20words.)

#### Q16. Which function do you use to deallocate memory?

- [ ] dalloc()
- [ ] dealloc()
- [ ] release()
- [x] free()

[Reference](https://devdocs.io/c/memory/free)

[Reference](https://www.tutorialspoint.com/c_standard_library/c_function_free.htm)

#### Q17. In C language what are the basic building blocks that are constructed together to write a program?

- [ ] keywords
- [ ] identifiers
- [x] tokens
- [ ] functions

[Reference](https://fresh2refresh.com/c-programming/c-tokens-identifiers-keywords/#:~:text=C%20tokens%20are%20the%20basic,are%20known%20as%20C%20tokens.)

#### Q18. When is memory for a variable allocated?

- [ ] during the assigment of the variable
- [ ] during the initialization of the variable
- [x] during the declaration of the variable
- [ ] during the definition of the variable

[Reference](https://www.codingame.com/playgrounds/14589/how-to-play-with-pointers-in-c/dynamic-memory-allocation#:~:text=When%20a%20variable%20is%20declared,allocation%20or%20dynamic%20memory%20allocation.)

#### Q19. C uses the call by value method to pass arguments to functions. How can you invoke the call by reference method?

- [x] by using pointers
- [ ] by declaring functions separately from defining them
- [ ] by using recursive functions
- [ ] by using global variables

[Reference](https://www.javatpoint.com/call-by-value-and-call-by-reference-in-c)

#### Q20. A union allows you to store different `___` in the same `___`.

- [ ] Objects; Structure
- [ ] Variables; Declaration
- [x] Data types; Memory space
- [ ] Arrays; Header file

#### Q21. What is the output of this program?

```c
main() {
    char c1='a' , c2='A';
    int i=c2-c1;
    printf("%d", i);
}
```

- [ ] 32
- [ ] Runtime error
- [x] -32
- [ ] 0

#### Q22. What is the difference between scanf() and sscanf() functions?

- [ ] The scanf() function reads data formatted as a string; The sscanf() function reads string input from the screen.
- [x] The scanf() function reads formatted data from the keyboard; The sscanf() function reads formatted input from a string.
- [ ] The scanf() function reads string data from the keyboard; The sscanf() function reads string data from a string.
- [ ] The scanf() function reads formatted data from a file; The sscanf() function reads input from a selected string

#### Q23. What is not a valid command with this declaration?

```c
char *string[20] = { "one", "two", "three"};
```

- [ ] `printf("%c", string[1][2]);`
- [x] `printf("%s", string[1][2]);`
- [ ] `printf("%s", string[1]);`
- [ ] `printf(string[1]);`

#### Q24. What is the expression player->name equivalent to?

- [ ] `player.name`
- [x] `(*player).name`