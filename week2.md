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
