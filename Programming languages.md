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