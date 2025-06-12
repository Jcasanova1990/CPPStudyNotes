iostream:
A C++ header file that allows input and output operations (e.g., cin, cout).

vector:
A dynamic array from the C++ Standard Template Library (STL) that can grow or shrink in size automatically. 
It stores elements in a contiguous block of memory and provides fast access by index.

namespace:
A way to group names (like functions and variables) to avoid naming conflicts.
std is the standard namespace in C++.

endl:
A special stream manipulator that inserts a newline and flushes the output buffer. used for immediate things i.e. text or healthbar or level.

\n:
A newline character that moves the cursor to the next line. It does not flush the buffer. used for continuous things like loops i.e doing damage 
repeating name and class taking damage and battle start.



**Example of rpg character class**

#include <iostream>
#include <string>

using namespace std;

class RPGCharacter {
private:
    string name;
    string charClass;
    int level;
    int health;

public:
    // Constructor
    RPGCharacter(const string& name, const string& charClass, int level, int health)
        : name(name), charClass(charClass), level(level), health(health) {}

    // Display character info
    void displayInfo() const {
        cout << "Character Info:" << endl;
        cout << "Name: " << name << "\n";
        cout << "Class: " << charClass << "\n";
        cout << "Level: " << level << endl;
        cout << "Health: " << health << endl;
    }

    // Simulate taking damage
    void takeDamage(int damage) {
        cout << name << " takes " << damage << " damage!\n";
        health -= damage;
        if (health < 0) health = 0;
        cout << "Remaining Health: " << health << endl;
    }
};

int main() {
    RPGCharacter hero("Arin", "Warrior", 5, 100);

    hero.displayInfo();
    cout << "\nBattle Begins!\n\n";

    hero.takeDamage(25);
    hero.takeDamage(50);

    return 0;
}



**Printing

file Output

For Linux both

use code runner or ctrl+shift+b = create .exe 

to run file in linux terminal run:
g++ filename.cpp -o rainbow

g++ = invokes gnu compiler
filename.cpp = file 
-0 = operator

then type ./rainbow to execute file in terminal
this will print text in terminal

for windows only ctrl+shift+b
then run ./rainbow.exe

for multi-line comments use /*multi example*/
for standard comments use //standard example

cout sends your output to console or terminal whatever is default


**Variables

Declaring = setting or declare the data typetype and name of the variable,
these two properties dont change.

Assigning = when setting the value of the variable, the variablecan change.

Accessing = when you retrieve the value of the variable by calling its name.


octal numbers = start with a 0 so the system converts any number with a Zero
to a decimal number.


**Data Types:Floating point numbers

Floats = are numbers with a decimal they can be positive or negative.

Double = because floats use 4 bytes it is ineffiecient to use, so we use
use double because it uses 8 bytes.

--also int has a whole number.

**Boolean

It is a declared variable that only take a true or false value.

Boolean values are case sensative and must be in all lowercase.

**Boolean Operators

== is equal checking
2= is assigning a value to the variable
2!= checks if values are not equal
!= is not equal to
boolAlpha checks Boolean for true or false
= assigns a value to a variable

**Strings

A collection of text numbers or symbols

i.e. 

#include <iostream>
using namespace std;

int main() {
    string words = "This is a string.";
    cout << words << endl;

    return 0;
}
    must be in lower case


**Declaring a Variable

string my_var, My_var, thisIsAwesome;

1.must start with an underscore or letter.
2.cannot use c++ keyword i.e. class.
3.c++ does not allow duplicate names for variables.
4.c++ does not allow spaces for variables.

**Iniatializing & Assigning

1.you can do this seperately or combine the same statement.
2.since the value stored in a variable can change, we call it assigning or reassigning.
3.cout accessesthe variable.

**Basic data types

1.Double
2.int
3.string
4.bool

