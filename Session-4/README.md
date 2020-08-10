# session4-Anil Bhatt
session3-Anil Bhatt created by GitHub Classroom

# Floats: Coercing to Integers
- Different way to configure the data loss like Truncation, floor, ceiling, round
- Truncation --> remove the floating part and returns the integer
- Floor --> Largest integer less than or equal to the number
- Ceiling --> Smallest integer greater than or equal to number

# Floats: Rounding
- Rouding is the Built-in function in python
  
# Decimals
- Refer Pep 327
- Decimal “is based on a floating-point model which was designed with people in mind, and necessarily has a paramount guiding principle – computers must provide an arithmetic that works in the same way as the arithmetic that people learn at school.” – excerpt from the decimal arithmetic specification.

# Decimals: Constructors and Contexts
- In accordance with the standard, the decimal module provides two ready to use standard contexts, BasicContext and ExtendedContext. 
- The former is especially useful for debugging because many of the traps are enabled:
  
ctx=decimal.getcontext() --> this is global contexts

ctx.prec

ctx.rouding --> different way of rounding can be seen here

- The Decimal class is in the module decimal as below

from decimal import Decimal

- Type of decimals

  - integes  --> a = Decimal(10)
  - string   --> a = Decimal('10')
  - tuple    --> a = Decimal((1,(3,1,4,1,5),-1)
	
# Context Precision and the Constructors
Context precision affects mathematical operations  but context precision does not affect the constructor.

# Decimals: Math Operations
Some arithmetic operators dont work the same as float or integers

# Decimals: Performance Considerations

There are some drawbacks to the Decimal class vs the float class.

Those are:
1. Not as easy to code: construction vis strings or tuples
2. Not all mathematical function that exist int he math module have a Decimal counterpart
3. More memory overhead
4. Performance: much slower than float

# Complex Numbers
- Complex numbers are represented as k+3j where k is real part and j is imaginary part.
- These are stored as float & hence must be very careful while testing
- Arimaetic Operations supported --> (+,-,/,*,**)
- Real and complex numbers can be mixed
- // and % operators dont support complex numbers
- == and != operator are supported
- comparision operators are not supported
- Functions in the 'math' module will not work hence we have to use 'cmath' module
- Some instance properites and methods are:
1. .real 				    --> returns the real part
2. .imag 				    --> returns the imaginary part
3. .conjugate()			--> returns the complex conjugate

# Booleans

- Python has a concrete bool class that is used to represent boolean values.
- bool is subclass of the int class and it inherits all the properites of int class
- True is 1 and False is 0

# Booleans: Precedence and Short-Circuiting
- The boolean Operator: not and, or
- Operator precidence: BODMAS

# Final output

