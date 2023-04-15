
# Week 1 : Introduction, Evolution of programming languages

## Language Evaluation Criteria:
1. Readablity 
2. Writability
3. Reliability 

## Readability
### Simplcity
- A language witha  larghe number of basic constructs is more difficult to learn
- Feature multiplicity
- Operator overloading
- Simplicity vs. high-level language

### Orthogonality
- Small number of primitive constructs can be combined in a small number of ways, each combination is legal and meaningful
- Independent of context

### Data types
- Adequate data types are available, e.g., Booleans
### Syntax Design
- Identifier forms, special words, form and meaning


## Writability

### Simplicity
- Misuse of unknown features
### Orthogonality
- Low orthogonality requires to memorize a lot of exceptions
- Errors can go undetected if nearly all combinations of primitives are legal
### Data types and Syntax design
- See Readability
### Support for abstraction
- Ability to define and use structures in ways that allow many details to be ignored
- Process abstraction: subprograms, polymorphism
- Data abstraction: interfaces, references, recursive data types
### Expressivity
- Powerful but convenient constructions


## Reliability

### Simplicity, Orthogonality, Data types, Syntax design, Support for abstraction and Expressivity
- See Readability and/or Writability
### Type checking
- Simple test for type errors
- Compile-time: more desirable, detect before run
- Errors at run-time: costly and errors might not be detected
### Exception handling
- Intercept run-time errors
### Aliasing
- Two or more distinct names accessing the same memory cell
Dangerous feature


[Week 2](week2.md)