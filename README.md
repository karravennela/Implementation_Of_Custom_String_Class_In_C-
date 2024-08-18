# Implementation_Of_Custom_STRING_Class_In_CPP
# Overview
This project "Implementation Of Custom STRING Class" is implemented to create our custom string class which will have the same functionality as the existing string class.
- The STRING class has the following basic functionalities: 
  + Constructor with no arguments
  + Parameterised Constructor with only one argument
  + Copy Constructor
  + Destructor
- Some more functionalities of STRING class are mentioned below in features...
  
# Main Menu
Created a executable file named "string" from different modules like main.cpp,memb_fn_defns.cpp,friend_fns.cpp....etc.., when executed will perform the main program accordingly.
# Features
As member functions:
1. Constructor with no arguments:
   -> This allocates the storage for the string object in the heap and assign the value as a NULL character.
2. Parameterised Constructor with only one argument :
   -> It accepts a pointer to a character or we can say if we pass an array of characters, accepts the pointer to the first character in the array then the constructor of the String class allocates the storage on the heap memory of the same size as of the passed array and copies the contents of the array to that allocated memory in heap. It copies the contents using the strcpy() function declared in cstring library. 
3. Copy Constructor:
   -> It is called when any object created of the same type from an already created object then it performs a deep copy. It allocates new space on the heap for the object that is to be created and copies the contents of the passed object(that is passed as a reference).
4. Assignment Operator Overload:
   -> '=' operator is overloaded as member function despite the availability of default assignment operator  overload is to avoid shallow copy.
5. '+'   Operator Overload:
   -> Plus operator is overloaded to perform concatination of two objects i.e strings and store into third object using strcpy() and strcat() functions.
6. '>'   Operator Overload:
7. '<'   Operator Overload:
8. '>='  Operator Overload:
9. '<='  Operator Overload:
10. '==' Operator Overload:
11. '!=' Operator Overload:
   -> Above mentioned operators are overloaded to compare two objects by using strcmp() function and returns true/false accordingly (bool datatype).
12. '[ ]' Operator Overload:
    -> Index operator is overloaded to return the address of object according to the integer argument passed.
As friend functions:
1. Extraction Operator Overload:
    -> '>>' is overloaded to store the input char by char into a temporary buffer file until enter key is pressed.
    -> The data of temporary buffer is copied to the object whose m/r is dynamically allocated according to the the string length. 
2. Insertion Operator Overload:
   -> '<<' is overloaded to write the string data of the object on to the console.
3. 

char * STRcpy(STRING &, STRING const &);
 
  +  char* STRncpy(STRING &, STRING const &, unsigned long);
  + int STRcmp(STRING const &, STRING const &);
  + int STRncmp(STRING const &, STRING const &, unsigned long);
  + char* STRcat(STRING &, STRING const &);
  + char* STRncat(STRING &, STRING const &, unsigned long);
  + void STRrev(STRING &);
  + void STRupper(STRING &);
  + void STRlower(STRING &);
  + char* STRchr(STRING const &, int);
  + char* STRrchr(STRING const &, int);
  + unsigned long int STRlen(STRING const &);
  + char* STRstr(STRING const &, STRING const &);
