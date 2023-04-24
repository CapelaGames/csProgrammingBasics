# Commenting
Comments are sections of code that gets ignored by the computer. This is nice because we can write comments for others and ourself, describing what our code does.

Commenting is an important part of making your code easy to read, not just for others, but yourself in 3 months time, or 5 years time. You might have forgotten what your code does, but the comments will help you understand.

In C# there are multiple ways you might make comments.

## When should I comment code?




## Single line comments
To add a single line comment, just write //
This will turn everything to the right of // into a comment.

```
int x;
//This is a single line comment, you can write whatever you want here. By the way, this code just creates a variable "x" and stores the number 5 in it.
x = 5;
```

## Multi line comments
What if we want to make many lines comments, well we can write /* [Code goes here]  */
Now everything with in th /* and */ will be a comment. You can add /* and */ on different lines too.

```

/*
In this example, this line as well as the whole function below is now a comment and will be ignored by the computer.
int MyCode()
{
    int y = 7;
}
this line is also a comment.
*/
```

## Regions
This is a method of organising code that can work with comments to make your code neat. It sections off parts of your code, allowing you to minimise that part of your code, and keep your code organised. As the name suggests, if give your code regions, to help organise your code. 

To use it use "#region MyRegion" to start a region, MyRegion can be any name you like. Finally use #endregion to end a region. Give it a try to understand.

```
public class Health : MonoBehaviour
{
    #region Variables
    public int health = 5;  
    #endregion

    #region Functions
    private void Heal()
    {
        //code example here
    }
    #endregion
}

```