# Syntax

Syntax are the rules of the a programming language, you must follow the Syntax of C# or your code won't run. You can think of it as C#'s grammar, its the rules on how to structure lines of code.

The following is Unity3D's default script.

```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class NewBehaviourScript : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}

```
I will break down some basic syntax shown above.

## Case Sensitive
First thing of note is that C# is CaSe SeNsItiVe. "John" would not be the same person as "john" in the C# world.

## Statements
Statements are composed of [Variables](https://github.com/CapelaGames/csProgrammingBasics/blob/main/variables.md) and [Expressions](https://github.com/CapelaGames/csProgrammingBasics/blob/main/expressions.md) and for a line of code that preforms an action. 

For example
> float totalPrice = subTotal + salesTax;

Notice that Statements end in a semicolon ";". Forgetting the semicolon at the end of Statements is a very common mistake.

## Comments
Writing notes within your code is a good way of remembering what your code does. These notes are called comments. It also helps communicate with other developers to make debugging and upgrading code easier.

Everything on a line after a // is ignored by the compiler

```
//Sales tax must be added to the subtotal.
float totalPrice = subTotal + salesTax;
```
You can also create a multi line comment with /* and */

```
/*
   This is a multi-
   line comment
   isn't that wild?
*/

## Blocks
Not understanding blocks of code is a common mistake amongst beginners. We use curly brackets to indicate a block of code { }. Usually blocks start with a declaration, followed by it's contents within the curly brackets. Make sure to pay attention to where the { } starts and ends blocks of code. Keeping your code indented well will improve readability of blocks of code.

```
using System; // notice the line ends in a semicolon

namespace Basics
{ // an open brace indicating the start of a block
    class Program
    {
    	int y = 0;
        void Function()
	{
	    int x = 1 + 1;
	}

	void Function2()
	{
	    if(y==0)
	    {
	       y = 322;
	    }
	}
    }
} // a close brace indicating the end of a block
```


## Keywords
Certain words are reserved for C#'s use, they carry certin meaning. You cannot use these key words to name things (like classes or variables)

### Using
You might notice that the first three lines of code start with "using". These are allowing us access to code written somewhere else. For example if I write

> using UnityEngine;

I can now access code created by Unity that is related to the UnityEngine

### Class
Classes in programming are a way of structuring code into logical groups. They also function like blueprints.
```
class TestClass
{
    // Methods, variables (properties, fields), events, delegates, etc go here
}

```
