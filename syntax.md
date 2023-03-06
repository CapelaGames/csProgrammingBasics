# Syntax

Syntax are the rules of the a programming language, you must follow the Syntax of C# or your code won't run. Functions a bit like grammar does for the english language, its the rules on how to structure a sentence (or lines of code).

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

## Keywords
Certain words are reserved for C#'s use, they carry certin meaning. You cannot use these key words to name things (like classes or variables)

### Using
You might notice that the first three lines of code start with "using". These are allowing us access to code written somewhere else. For example if I write

> using UnityEngine;

I can now access code created by Unity that is related to the UnityEngine

### Class
Classes in programming are a way of structuring code into logical groups
