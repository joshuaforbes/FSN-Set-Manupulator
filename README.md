# Fuzzy Set Notation Set Manipulator

## What Does It Do?
This program implements 6 main functions that allow you to perform operations
on fuzzy sets in Fuzzy Set Notation. The operations are as follows:
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
First you need to clone the repo. Once you do that run the following command:
```
make
```
That will produce the program **checker1**.

## How Do I Use It?
Once you *make* the program you can run it using the following command:
```
./checker1
```
After you run the program it will halt for an input string. Once the input
string is entered, press enter, and the program will return the result.

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
