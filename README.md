# EPAI
EPAI Github repo

# Numeric Types
## Notes
Please refer https://nbviewer.jupyter.org/github/anilbhatt1/EPAI_1_Phase1/blob/main/S4_Numeric_Types_II/S4_Notes.ipynb. Notebook Covers following topics:
- isclose() both based on rel_tol and abs_tol
- trunc()
- floor()
- ceil()
- round()
- Decimals
  - getcontext
  - Context manager 'decimal.localcontext()' and setting localcontexts to override 'rounding', 'prec' etc using it.
  - Getting size using sys.getsizeof()
  - Why we should use floats whenever possible instead of Decimal. Use Decimal only if extra precision is required
- Complex Numbers
  - real & imag
  - cmath (Substitute of math for complex numbers)
- Booleans
  - display using format with required decimal places
  - Fact : True is 1, false is 0
  - 5 Cool booelan tricks with examples
  - Familiarize strings
  - How OR evaluates a condition
  - How AND evaluates a condition
  - Using 'in' to evaluate conditions

## Assignment

- Assignment is as below.

![Assignment](https://github.com/anilbhatt1/EPAI/blob/master/Session-4/Assignment.jpg)


## Assignment Solution

- Following functions were written to enable the Qualean Class.

- **init**
  - This function accepts the user input which must be one among [-1, 0, 1].
  - This input is passed to **transform** function which will return a value that will be stored in self.q.
  - If user input is not the desired one, an exception is raised.
- **transform**
  - Used in tandom with **init** function.
  - Accepts user input from init function, generates a random value between -1 and 1.
  - Multiplies this random value with user input, rounds it to 10 decimal places and returns back value to init.
  - This value is stored as self.q in init.
- **str**
  - Overridden innate str function to return user input value *Qualean Number :{int(self.user_input)}* eg: Qualean Number :1
  - Prior to customization, str was returning memory location of object
  - Gets invoked when print() or str() is called. 
- **repr**
  - Overridden innate repr function to return user input value.
  - Initially it was displaying the location of the object.
  - Gets invoked when we try to display variable name eg: x
- **add**
