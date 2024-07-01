If we want to store 23 digit number we couldn't do it ,as we know in C++ the max number of digits a long long int can have is 20 
so to storing a number above 20 digits is not possible. But we cans tore them by changing each digit into a char of string 
And for more operations like adding two big/large number require addition from the last digit of the number, which can be done by strings if
we store the number in the string only in the reverse order. So when we have a new digit we can add it at the last char of the string.

The BigInt class provides a way to handle arbitrarily large integers in C++.

we can create these kings of strings by constructors
Constructors: 
1.BigInt(unsigned long long n = 0): Initializes the BigInt with an unsigned long long integer.
2.BigInt(const char *): Initializes the BigInt with a string literal.
3.BigInt(string &): Initializes the BigInt with a string.
4.BigInt(BigInt &): Copy constructor.

Helper Functions are also defined to know more info about the number :
(the keyword friend is used to grant a non-member function or another class access to the private and protected members of a class)
1. friend bool Null(const BigInt &): Checks if the BigInt is zero.
2. friend int Length(const BigInt &): Returns the number of digits in the BigInt.
3. friend void divide_by_2(BigInt &a): Divides the BigInt by 2.
4. int operator[](const int) const: Accesses a specific digit.

in Operator Overloading there r many functions included too like arithmetic and mathematical functions 
