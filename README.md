# MoonMathManual
This repo contains my learning and work on the Moon Math Manual for ZK-SNARKS.


Integers :
    Integers are also known as Whole numbers, these are the numbers that can be written without fractional part
    Examples of the numbers that are not integers are : 2/3, 1.2 and -1280.006

    We use the symbol "Z" as a short for the set of all integers.

    Integers vs Whole Numbers:
        Integers include both negative and positive numbers including zero that are not decimals and fractional numbers
        Whole Numbers are just a set of non-negative numbers inluding zero that are not decimals and fractional numbers
    
    Z = {...,-3,-2,-1,0,1,2,3,....}

Absolute Value : Absolute value of an integer is always a non-negative number. It's denoted by |x| where x is eitehr +ve or -ve. and always yields a +ve value of x 
    Eg: |4| = 4
        |-4| = 4

We use the symbol N for the set of all +ve integers, they are usually called Natural Numbers.
Natural numbers don't have a zero.
We use N0 for the set of all non-negative integers. This means N does not contain 0 and N0 contains a 0.
    N := {1,2,3}
    N0 := {0,1,2,3}

Rational Numbers : Rational numbers are alwasy represented as a set of fractions n/m.
                    Where n is in the set of integers Z and m is in the set of natural numbers N.
                    There must be no other fraction n'/m' and natural number K which is in set N with k!= 1

The sets N, Z, Q have a notion of addition and multiplication defined on them.

`**************************************************************************************************************`

Another set of numbers that we are interested in is the set of `Prime Numbers`.
A prime number is a natural number with p >= 2 that is only divisible by itself and 1.
Prime Numbers are Natural numbers, that are greater than or equal to 2 and they are divisible by itself and 1.

Apart from Number 2 all other Primes are called odd primes. 

P is used to represent prime numbers, P3 for set of all add primes

The set of Prime Numbers P is an infinite set, and it can be ordered according to the size.
There is no largest prime number, no matter how large a prime number is there will always be a larger prime number.

Fundamental thoerem of arithmetic says every natural number greater than 1 can be uniquely expressed as a product of prime numbers. In other words prime numbers are the basic building blocks of all natural numbers.

this representation n = p1 * p2 * p3 is called prime factorization.

Prime numbers are the building blocks of number system. Prime numbers are like atoms of the number system.
Just like every molecule is made up of atoms, every natural number greater than 1 can be built by multiplying together prime numbers in some combination.

eg 6 = 2 * 3  = Both 2 and 3 are prime numbers
12 = 2^2 * 3 = Both  and three are prime numbers
30 = 2 * 3 * 5 = All 2,3,5 are prime numbers.
This kind of representation is called a prime factorization.

Uniqueness of Factorization:
The prime factorization of a number is unique. For any given natural numbers n, there is only one way to write n
as a product of primes, upto the order of the factors.
eg : 30 can be represented in prime facrotization as 2 * 3 * 5 - No other combination of primes can produce 30 (Ignoring the oder of the multiplication which doesn't matter).

This uniqueness is a crucial feature of the fundamental theorem of arithmetic.

Examples : n = 60 => Prime factorization of 60 is 2 * 2 * 3 * 5 = 2^2 * 3 * 5 - here p1 =2 p2 =3 p3 = 5, e1=2,e2=1, e3=1

Computation of the factorization of an integer  is expensive, becasue we have to divide , repeat themselves. From this an imporant question arises, How fast can we compute factorization of a natural number.
This question is the famous integer factorization problem and as far  as we know there is currently no known method that can factor integers much faster than the naive approach of just dividint he given number by all prime numbers in ascending order.

but, computing the product of given set of prime number is fast: you just multiply factors
This simple observation implies that the two processes,
Prime number multiplication on the one side and its inverse procee, "Natural Number factorization" have very different computational costs.
This factorization problem is therefore an example of a so-called one-way function:
an invertible function that is easy to compute in one direction, but hard to compute in the other 
direction.


Euclidean Division :

Euclidean division referes to the process of dividing two integers to obtain a quotient and a remainder.
It is based on the principle that for any two integers a and b(Where b != 0) there exists unique integers q and r -- Quotient and remainder respectively such that:
    a = bq + r -- a divident, b is divisor, q is quotient, r is remainder.
    where 0 <= r <|b|

Given integers a and b the divison process results in a = br + q


Applications of Euclidean division:
    1. Greatest Common Divisor: The Euclidean algorithm, based on repeated Euclidean division is a method to compute the GCD of two numbers.
    2. Modulo Operation: The remainder r in Euclidean division is ued in modular arithmetic
     (a mod b = r).

     a div b := m a mod b := r
     We can say an integer a is divisible by another integer b if a mod b = 0 holds true.

In a nutshell Euclidean division is the process of dividing one integer by another in a way that produces a quotient and a non-negative remainder,
The latter of which is smaller than the absolute value of the divisor.




