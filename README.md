 # ME 701 -- HW 3

Instructions:  Your solutions to the following should be contained in
one file named {\tt lastname\_firstname\_hw3.py} and uploaded to Canvas.


## Problem 1 -- Some Python `str` Basics


1. Let `a = "hello"` and `b = "world"`.  Use 
   `a` and `b` to produce `c = "hello world"`.
2. Figure out how to define `d = 'Hello World'` starting with `c`.
3. From `d`, define \texttt{e = ``Hello''} and  \texttt{f = ``World''}
   in a single line of code.
4. Let  `g = 123; h = 3.141592653589793; i = 6.022e23`.  Using those 
   values, produce `j = '123|3.1416| 6.02e+23'` in just one line.
5. Let `k = 5` (or some other integer).  Use that to produce 
   `l =  '0..1..2..3..4'` in just one line.

## Problem 2 -- A Python Oddity

Consider the following code and output
```
>>> a = [1, 2, 3]
>>> b = a
>>> a[0] = 99
>>> a
[99, 2, 3]
>>> b
[99, 2, 3]
```

In other words, a change in `a` leads to
a change in `b`.  This can confuse Python
newbies.

1. Explain, in your own words, why this happens.
2. Offer **two** ways by which one could produce a second list `b` with the same 
   `a`.  At least **one** of these should require no more than one 
   expression.  For reference, an expression is just a composition of 
   arithmetic or other operations, e.g., `sin(a**2)/4.0+1`.

## Problem 3 -- List Comprehension

List comprehension is a uniquely Pythonic way to construct lists
without using explicit loops.  Rewrite the following using list 
comprehension:

```
  # Part 3.1. Compute first 20 powers of 2
  i = 0
  powers = []
  while i < 20:
      p = 2 ** i
      powers.append(p)
      i = i + 1
```

```
  # Part 3.2. Generate all (x, y, z) coordinates from three lists
  xpoints = [1, 2, -1]
  ypoints = [8, 4, 3, 0]
  zpoints = [0, -1]
  points = []
  for x in xpoints:
      for y in ypoints:
	        for z in zpoints:
	            points.append((x, y, z))
```


