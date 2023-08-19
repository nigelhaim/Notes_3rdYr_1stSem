Concepts of programming languages 
Robert Sebesta 

2023-08-12
### Motivations
Why studying programming languages 
- Increases our ability to express ideas
	- Increases capacity to use different constructs in writing programs
	- Enables us to have a bigger perspective 
- Enables to choose languages for projects 
- Makes learning new languages easier 
	- [TIOBE] Programming community
		- Organization having good assessment in the usage of programming languages 
- Better understanding of significance of implementation
	- Can help in bug fixing 
- Better use of languages that are already known 
- Overall advancement of computing 
	- Examples
		- ALGOL vs Fortran

Overall to have a better understanding and have a bigger perspective in learning different kinds of programming languages and when to use them. 

TIOBE INDEX
- Lists of the top 20 languages
- Not standard way of understanding 

**Programming languages**

No Electricity
- 1986
	- Low level programming languages 

Hard Core 
- 1950
	- Mark I/II
	- ABC
	- ENIAC
	- UNIVAC
- Mainframe -> Programming languages 
- Bits and bytes 
- High level programming language development 
	- Fortran
		- Formula Translator 
		- Made for Engineers 
	- COBOL
	- Advol

Spaghetti
- BASIC
	- Easy to use 
	- Beginner All-purpose Structure something something 
- Unstructured 
	- GOTO
Structured 
- Imperative 
- Not efficient 
- Hard coding 

OOP
- Easy application 
- Inheritance 

### Programming Domains
- Programs used in a wide variety off problem-solving domains
- The design and evaluation of a particular language is highly dependent on the domain in which it is to be used 
	- **Scientific** 
		- Fortran and AGOL 60
	- **Business Application**
		- COBOL, RPG
	- **Artificial intelligence** 
		- LSIP, Prolog, Scheme
	- **Systems programming** 
		- IBM's PLUS, Digital BLISS, UNIX
	- **Web Software** 
		- Java, PHP, JavaScript 

### Language Evaluation Criteria
- **Readability**
	- programs can be read and understood
	- can be interpreted
- **Writability**
	- language can be used to create programs in the program domain
	- what to write 
	- Differs according to the domain for which the language is designed 
	- Simplicity and orthogonality
		- Orthogonality - The set of constructs of a language 
- **Reliability**
	- conformance to specifications
	- Data types
- **Cost**
	- the total cost
	- Training programmers
	- Writing programs 
	- Compiling efficiency 
	- Executing efficiency
	- Language implementation system 
	- Reliability: poor reliability leads to high costs 
	- Maintaining programs
- **Other**
	- Portability - moved from one platform to another 
	- generality  - Wide range of applications 
	- well-defined - Precision of the language's official definition

![[Pasted image 20230817135027.png]]

2023-08-17

### Influences on Language design 
**Computer Architecture** - architectural model for procedural languages 
- von Neumann architecture 
**Programming methodologies** - New software development methodologies 
- OOD led to new programming paradigms

#### Von Neumann Architecture 
- **Fetch-execute-cycle**
```
	Initialize the program counter 
	 repeat forever
		fetch the instruction pointed by the counter 
		increment the counter 
		decode the instruction 
		execute the instruction 
		store the result 
	 end repeat
```
- ![[Pasted image 20230817141722.png]]
- **Von Neumann Bottleneck** - primary limiting factor in the speed of computer programming 

#### Computer Architecture Influence
- Von Neumann computer architecture 
- Imperative languages, most dominant, because of von Neumann computer s
	- Data and programs stored in memory 
	- Memory is separate form CPU 
	- Instructions and data are piped from memory to CPU 
	- Basis
		- Variables model memory cells
		- Assignment statements model piping 
		- Iteration is efficient

#### Programming methodologies Influence 
- **50s and early 60s**
	- Simple applications 
	- concerns were about machine efficiency 
- **Late 60s, early 70s**
	- Complex programming problems 
	- Reduced hardware cost 
	- Software devleopment increased costs 
		- More demand for programmers 
	- Structured programming movement led to Top-Down-Stepwise Refinement 
		- Readability, better control structures
- **Late 70s**
	- Shift from procedure-oriented to data-oriented design
		- Data abstraction to encapsulate processing with data
- **Middle 80s*
	- Object-oriented programming 
		- Data abstraction inherence and dynamic method binding (polymorphism)
- More recently procedure oritgneted programming applied to concurrency 

#### Other Influences on Language design 
- **Other considerations **
	- Concerns for commercial success
	- Implementation difficulties
		- Cobol 
	- Academic 
		- Fortran

#### Language Categories
**Imperative**
- Central features are variables, assignment statements, and iteration 
- Include languages that support object-oriented programming i
- include scripting and visual languages 
**Functional**
- Main means of making computations is by applying functions to given parameters
**Logic**
- Rule-based (rules are specified in no particular order)
- Returns true or false 

##### PROLOG
- y:-x "if x then y " - Rule based 

**Markup/Programming hybrid**
- Markup languages to extend to support some programming 
#### Language Design Trade-offs
**Reliability vs cost of execution** - 
**Readability vs writability** - 
**Writability (flexibility) vs reliability**

#### Layered View of Computer
- The operating system and language implementation are layered over machine interface of a computer
![[Pasted image 20230819180832.png]]

####  Methods of Implementation
- **Compilation**
	- Compiler - The programming language is developed 
	- Interpretation - source code is translated 
	- Hybrid interpretation - Compromise between compiler and interpreter
- **Pure Interpretation**
- **Hybrid Interpretation**
#### Compilation process phases
- Source code is translated into equivalent machine code as a unit and stored in to a file that has to be executed in separate step.
- **Lexical analysis**
	- extracts a sequence of tokens from source code 
	- the symbol table contains the definitions of the identifiers
- **Syntax analysis** 
	- Transforms tokens into parse trees which represent the syntactic structure of program.
- **Semantics analysis** 
	- Generate intermediate code
- **Code generation** 
	- Machine code is generated

#####  Backus-Naur Rules Form (BNF)
- Assignment statement - Composed of left hand side followed by a symbol followed by the right hand side 
- Left hand side - has an identifier
- Right hand side - has identifier followed an operand and another identifier

#### Pure Interpretation Process
- Pure Interpretation - source code is translated into machine code and executed immediatly 
- Advantage -run-time errors can refer to source level units such as array index out of bounds errors
- Disadvantage
	- 10 to 100 times slower execution time 
	- Often requires more space 
- Significant comeback with some Web scripting languages 
![[Pasted image 20230819183328.png]]

#### Hybrid Implementation Process
- A compromise between compilers and pure interpreters
- A high-level language program is translated into an intermediate language that allows easy interpretation
- Faster than pure interpretation since source language statements decode only once 


#### Additional compilation terminologies
**Linking and loading** - process of collection system program units and linking them to a user program 
**Load module** - the user and system code together
**Preprocessor** 
- Preprocessor macros Commonly used to specify that code from another file is to be included 
- A preprocessor processes a program immediately before the program is compiled to expand embedded preprocessor macros

#### Programming environments 
- Collection of tools used in software development 
- Simple - file system, text editor, compiler, interpreter or linker.
- Extensive - rich set of tools 
	- Borland Jbuilder
		- An integrated development environment for Java
	- Microsoft visual Studio.NET
		- A large, complex visual .....


### Chapter 2 hint 

#### Computter Lnauges History

levenez.com

The history of a programming language 