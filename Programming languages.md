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

08-25-2023
### Chapter 2 Evolution of the Major Programming Languages 

#### Computer Languages History

levenez.com

The history of a programming language 
![[Pasted image 20230824134455.png]]


#### UMBC CMSC 331
##### History of Programming languages 
**History**
- Tries to details the programming languages of history 
- from 1940s to early 2000s 
**Early History: First Programmers**
- Ada Lovelace - First programmer 
	- First lady programmer 
- Konrad Zuse and Plankalkul 
- 1940s: Von Neumann and Zuse 
	- Konrad Zuse (Plankalkul)


#### 1950
##### First Compiling system
- 1950-1953
- **Grace Hopper and her team at UNIVAC**
	- Started the name of Hex
	- Developed a "compilijng sytem"
	- Written in a type of psuedocode then expanded to machine code 

##### Progress in Generality 
- 1950

##### Speedcode system 
**Support for Floating point operations**
- **John Backus**
	- DNF 
	- Promoters of using a convention where we can define the grammar of a language 

##### First Real Compiler? 
- **Alick E. Glennie**
	- Mark I one of the first compilers 
	- Manchester (Europe)
- **Laning and Zierler**
	- MIT 
	- Developed an algebraic translation 

##### Fortran
- 1954
- **IBM 704**
	- Provide hardware for indexing and floating point instructions 
- **John Backus and group at IBM**
	- Provide efficiency of hand-coded programs
	- Implementation began in 1955
	- Released in 1957 as Fortran I 
	- Provide the first version of the compiler and d error checking

##### Artificial Intelligence 
**Mid 50s**
- Interest in AI emerged 
	- Natural language processing 
	- Human brin processes 
	- Mechanizing certain intelligent processes such as theorem proving 
		- Processing symbolic data in lists that could be easily manipulated

#####  AI and Fortran
- Mid 50s
- **IBM**
	- The forefront of microcomputers 
	- FLPL (Fortran List Processing Language)
		- Extension to the Fortran compiler
			- Used to construct a theorem prover for plane geometry 

##### First AI Programming Language 
**IPL - information processing language**
- 1956
- **Allen Newell, J.C. Shaw, Herbert Simon**
	- Published a description of one of the first AI Languages 
		- IPL-1
			- Information Processing Language 
##### Business Domain 
- 1957
- FLOW-MATIC
	- Business oriented language for the UNIVAC
		- Mathematical programs should be written in mathematical notation, data processing programs should be written in English statements (Grace Hopper 1953)
- **COBOL 60 (1959)**
	- Common Business Oriented Language 
		- Design Goals 
			- Use English 
			- Easy to use 
			- Not be overly restricted by problems 
		- Characteristics 
			- DEFINE verb for Macros 
			- Records 
			- Data Division and procedure division

##### Fortran Progresses 
- 1958
- **Fortran II compiler**
	- Bug fixes 
	- Independent compilation of subprograms 
		- Made lengthier programs possible 


##### LISP
**List Processing**
- 1959
- A functional language
- Dominated for a decade 
- Originally interpreted 
- Decedents 
	- Scheme 
	- COMMON LISP 
- Related Language - ML (Machine Language)
- **John McCarthy and Marvin Minsky**
	- Produced a system for list processing 
	- Promoted HCI and AI 
	- John McCarthy - The father of AI 

##### Expert System
- Try to imitate the human brain 
- Pickup points through questions and choices and finding a conclusion based on the answers given 
- Pattern of a tree
- When you look at the pattern itself it will have some Segway

#### 1960

#####  Progress of AI 
- 1960
- **Newwell and Tonge**
	- IPL-V
		- Demonstrated that list processing was feasible and useful
		- Actually an assembly language implemented in an interpreter with list processing instructions for the Johnniac machine 
		- Johnniac machine - Named after John Bakus 
		- More on list processing and not on scientific
- **ALGOL 60**
	- New additions 
		- Block structure concept 
		- Pass by value and pass by name 
		- Recursive procedures 
		- Stack-dynamic arrays 
	- Decedents 
		- PL/1, SIMULA 67, Pascal, Ada, C++ and Java

##### APL and SNOBOL
- 1960
- **APL**
	- Kenneth Iverson at IBM
	- Designed for describing  computer architecture 
- **SNOBOL**
	- Designed for text processing 
	- collection of powerful operations for string pattern matching 
- **Common features**