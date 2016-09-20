### Prime Finder


## To Run
Clone or download the CS511 repository and change your working directory to 'Assn1'

# Compile Everything
```sh
$ javac *.java
```
# Run
```sh
$ java AssignmentOne
```

## Synopsis

Implement a class AssignmentOne that includes a method

public List<Integer> lprimes(List<Integer[]> intervals)

that given a list of arrays of integers of size 2 [[g1,d1],...,[gk,dk]] such that the list [g1,d1,...,gk,dk] is increasing and
each number is greater or equal to 2, creates k threads where each thread i computes the list of primes in the interval [gi,di+1) (notice the interval is semi-open). 

For example, given the list of arrays
lprimes([[1,101],[101,201],[201,301],[301,401],[401,501]])
it will spawn 5 processes. Process 2 will, for example, compute all the primes between 101 and 200, namely
[101,103,107,109,113,127,131,137,139,149,151,157,163,167, 173,179,181,191,193,197,199]

The result of the whole process would be the list
[2,3,5,7,11,13,17,19,23,29,31,37,41,43,47,53,59,61,67,71,73,79,83,89,97,101, 103,107,109,113,127,131,137,139,149,151,157,163,167,173,179,181,191,193,197, 199,211,223,227,229,233,239,241,251,257,263,269,271,277,281,283,293,307,311, 313,317,331,337,347,349,353,359,367,373,379,383,389,397,401,409,419,421,431, 433,439,443,449,457,461,463,467,479,487,491,499]
