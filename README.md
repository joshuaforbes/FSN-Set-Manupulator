# Fuzzy Set Notation Set Manipulator

## What Does It Do?
This program implements 6 main functions that allow you to perform operations
on fuzzy sets in Fuzzy Set Notation. The parameter interface for these function
is curried. The operations are as follows:
- **set_intersect**: This function takes in two sets and returns a set that contains
the point-by-point maximum between both sets.
- **listMaxTuples**: This function takes in a set and returns the tuple with the
largest membership function. If the set has multiple tuples with the same max
value, the first occurrence will be returned.
- **listMaxTupleValue**: This function takes in a set and returns the membership 
function of the tuple that would be returned by listMaxTuples.
- **truncateConsequentMu**: This function takes in a set and a membership function
and returns the set with all membership functions greater than the given value
truncated at the given value.
- **listMaxTuplesAll**: This function takes in a set and returns a list of all 
tuples in the set with the same maximum value. This function will behave as
listMaxTuples if the set only has one max tuple.
- **mom**: This function takes in a list of truncated maximum values, 
preferentially the product of truncateConsequentMu and listMaxTuplesAll, and,
returns the mean of the maximum values of the tuples (ie, the integer value).


## Warning!
The code presented here does not handle exceptional cases such as:
- Conflicting Domains
- Improper Syntax
- Improper Values

You are responsible for checking these conditions before the sets are passed to
the functions.

## What Do I Need?
This version was developed using:
- Ocaml 4.02.3

## How Do I Get It?
First you need to clone the repo. Once you do that start Ocaml like so:
```
ocaml
```
That will start the ocaml interpreter. Then you load the file like so:
```
# #use "sde2.caml";;
```
This should give you signatures for the six functions discussed above. This
means that the file was imported properly and that everything is good to go.

## What About These Other Functions That Come Up?
They are merely helper functions written to help implement the six discussed
above. Ignore them or feel free to use them as you see fit.

## How Do I Use It?
Just call the functions by name in the interpreter.

## License Information
This software is licensed under the GNU GPL V3.0. The actual license can be
found in the file named LICENSE and online [HERE](https://www.gnu.org/licenses/gpl.html). 
The software is copyrighted by the owner of the repo and the statement of 
copyright is provided here as well.
> Copyright (C) 2017 Joshua Forbes

## Academic Misconduct Disclaimer
As of the date of this writing the code contained in this repo completes an
assignment given as part of the **CPSC/ECE 3520** class taught at Clemson 
University by [Dr. Robert J. Schalkoff](http://www.clemson.edu/cecas/departments/ece/faculty_staff/faculty/rschalkoff.html).
Viewing or copying this code or repo while currently enrolled in this course is
a violation of Clemson University's [Academic Integrity Policy](http://www.clemson.edu/studentaffairs/student-handbook/universitypolicies/academic_integrity.html).
If you choose to do so, you are doing so without the knowledge of the owner of
this repo and at your own risk. If you choose to do so you are doing so alone of 
your own accord and the owner of this repo carries no responsibility for your 
actions. You have been warned.
