# Week 2 :Evolution of programming languages

## PL/I
- First language designed for a broad spectrum of use cases
- Developed by IBM in 1963

### PL/I uses the best part of 
> Includes Algol 60's 
   > > block structure
   > > and recursion

> Fortran IV's
>> separate compilation with communication through global data

> COBOL's
>>data structures, 
>>input/output, 
>>report generating facilities

+ Huge language with a lot of features; first in having
  - Creating concurrently executing subprograms
  - Exception handling (23 different exceptions)
  - Efficient linking for nonrecursive subprograms
  - Pointers were included as a data type


``` pl
/* PL/I PROGRAM EXAMPLE
  INPUT: AN INTEGER, LISTLEN, WHERE LISTLEN IS LESS THAN
         100, FOLLOWED BY LISTLEN-INTEGER VALUES
  OUTPUT: THE NUMBER OF INPUT VALUES THAT ARE GREATER THAN
          THE AVERAGE OF ALL INPUT VALUES */
PLIEX: PROCEDURE OPTIONS (MAIN);
  DECLARE INTLIST (1:99) FIXED.
  DECLARE (LISTLEN, COUNTER, SUM, AVERAGE, RESULT) FIXED;
  SUM = 0;
  RESULT = 0;
  GET LIST (LISTLEN);
  IF (LISTLEN > 0) & (LISTLEN < 100) THEN
    DO;
/* READ INPUT DATA INTO AN ARRAY AND COMPUTE THE SUM */
    DO COUNTER = 1 TO LISTLEN;
      GET LIST (INTLIST (COUNTER));
      SUM = SUM + INTLIST (COUNTER);
    END;
```
---

## APL and SNOBOL

+ Both languages ar not base on any previous languages
+ they both have dynamic typing and storage allocation
+ APL
  - Designed around 1960 at ibm
  - **A** **P**rogramming **L**anguage
  - Hard to maintain
+ SNOBOL
  - Designed in the early 1960s for text processing
  - Powerful operations for string pattern matching

---

## Simula 67
+ Simula I was developed between 1962 and 1964 in Norway
  - Designed for simulations
  - Later extended to bvecome a general purpose language
+ Simula 67 presented/release in 1967
  - Extends Algol 60
  - Introduces coroutines
  - Introduces the class construct

---
## C
+ Developed at Bell Laboratories in 1972
+ Ancestors: CPL, BCPL, B, and Algol 68 
+ Designed as a language to implement UNIX
+ Fist official standard in 1989 (ANSI C); next in 1999 (C99)
+ Lack of complete type checking

``` C
/* C Example Program
Input: An integer, listlen, where listlen is less than
       100, followed by listlen-integer values
Output: The number of input values that are greater than
        the average of all input values */
int main (){
  int intlist[99], listlen, counter, sum, average, result;
  sum = 0;
  result = 0;
  scanf("%d", &listlen);
  if ((listlen > 0) && (listlen < 100)) {
/* Read input into an array and compute the sum */
    for (counter = 0; counter < listlen; counter++) {
      scanf("%d", &intlist[counter]);
      sum += intlist[counter];
    }
/* Compute the average */
    average = sum / listlen;
/* Count the input values that are > average */
    for (counter = 0; counter < listlen; counter++)
      if (intlist[counter] > average) result++;
/* Print result */
        printf("Number of values > average is:%d\n", result);
  }
  else 
    printf("Error-input list length is not legal\n");
}

```

--- 
## C++ 
+ Object-oriented version of C
+ Goals:
  - Add classes and inheritance
  - No performance penalty
+ Development steps
  - C with Classes (1983)
  - Extension with virtual methods (1984), first version called C++
  - First implementation in 1985 (Cfront)
  - Multiple inheritance, abstract classes (1989, C++ Release 2.0)
  - Templates, parametrized types, exception handling (1990, C++ Release 3.0)
  - Current C++ standardized in 1998, described in ISO

#### Features
> Supports procedural and object-orientated programming
Multiple inheritance
Operator overloading
Virtual methods
Class and method templates
Exception handling
+ Very popular language
+ Very large and complex
+ Inherits the insecurities of C, less safe than Ada or Java

---

## Additional notes:

> mentions ADA(American Army), 
> PROLOG(logic programming),
> Smalltalk (first object oriented language)

[Week 3](week3.md)