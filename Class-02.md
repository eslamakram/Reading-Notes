# reading notes 201 class 02

## HTML

1.Headings and paragraphs

*HTML has six "levels" of headings:*
h1 is used for main headings
h2 is used for subheadings

**2.Bold, italic, emphasis**
   . Bold : By enclosing words in the tags b we can make characters appear bold and we can use tag strong
   . Italic : By enclosing words in the tags i we can make characters appear italic.
   . Emphasis : By enclosing words in the tags em we can make characters appear italic

**3. Structural and semantic markup**
     . Structural markup: the elements that you can use to describe both headings and paragraphs
     . Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something
                    you have written is a quotation (and who said it), the meaning of acronyms, and so on

## CSS

What CSS does :*
    CSS works as an invisible box around every HTML element.

Why CSS does? :*
    1. CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.
    2. can style certain elements such as lists, tables, and forms.

How CSS works? :*
    CSS works by associating rules with HTML elements. A CSS rule
    contains two parts: a selector and a declaration.

       selector
        p {
           font-family: Arial; // decrelation 
        }

 also; CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon.
 ![css selector](img/css%20slector.png)

There are two ways to do it :*
    1. internal : You can also include CSS rules within an HTML page by placing them inside a style element, which usually sits inside the head element of the page
    2. external : The link element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it  does not need a closing tag), and it lives inside the `<head>` element. It should use three attributes:
                              1. href : This specifies the path to the CSS file .
                              2. type :  The value should be text/css.
                              3. rel :  The value should be stylesheet

## JAVASCRIPT

1. **Basics of Instructions**
    A VARIABLE?
    A script will have to temporarily store the bits of information it needs to do its job. It can store data in it.
    firstly we should declare variables by **var** or **let**

    . when you use var , you can then change what is stored in the variable later in the same script

    DATA TYPES ?
    JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.

    ARRAYS?
    An array is a special type of variable. It doesn't just store one value; it stores a list of values.

    `colors = ['white', 'black', 'custom'];`

    Each item in an array is automatically given a number called an index. This can be used to access specific items in the array.

2. **Decisions**
     Decision making or flow control. JavaScript has built-in statements (keywords) called decision-making (flow control) structures. We will look at if and switch statements
    Using the results of evaluations, you can decide which path your script should go down.
    **if Statements**
Probably the most common flow control statement you will use will be the if statement. The if statement runs specified code if a conditional expression returns true.

The syntax for the if statement is

    if (conditional expression)
    {
    a statement;
    another statement;
    }

 **if...else Statements**
You can add an else statement to your if statement so you can specify one set of code to run if the conditional expression evaluates to true and another set of code to run if the conditional expression evaluates to false.

The syntax for the if...else statement is

      if (conditional expression)
     {
    a statement;
     another statement;
     }
      else
     {
    yet another statement;
    even another statement;
     }
  
  **Multiple if...else Statements**
If you have many choices of actions based on many possible values of an expression, you can use multiple if...else statements in sequence. (In the next section, we will see the switch statement, which is often a better way to go.)
    The syntax of a switch statement is like this:

    switch (expression)
      {
    case label1:
      statement;
      statement;
      break;

    case label2:
      statement;
      statement;
      break;

    case label3:
    case label4:
      statement;
      statement;
      break;

    default:
      statement;
      statement;
     }

   3.**Loops**
    The while or for statement is used for repeating a statement or code block as long as a given conditional expression evaluates to true.

The syntax of the while statement looks like this:

     while (conditional expression)
     {
    statement;
    statement;
        }

Please note these points about the above syntax:

. The statement begins with the while keyword.
. The conditional expression is contained in parentheses.
. The statement(s) that you want repeated are contained in curly braces.
. If the conditional expression is initially false, the loop never runs its contained statements.
. If the conditional expression initially evaluates to true, the loop runs until the conditional expression becomes false. Then the loop ends, and any statements following the loop are run.
