# Domain modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## HTML Tables

what ?

HTML Tables are used to arrange data systematically so that the user can easily interpret it. With lots of data being available, the developers need to organize it in a manner so that it can be easily understood; tables facilitate this efficiently. They are widely used for research, data analysis, etc.

Why ?

- The schema of the databases is well defined with the help of tables.
- It helps in easy comparison of lots of data available.
- Tables help in the systematic presentation of information and content available.
- Tables consist of rows and columns and can contain text, images, links, other tables, etc.

How ?

The `<table>` element is used to create a table in HTML. Table header is defined by `<th>` and by default, the table headings are bold and centered. The `<tr>` tag is used for rows and `<td>` is used to define table data or cell.

### Javascript Functions

 what ?

 A function holds a set of actions that will run when we call that function. This helps us control the flow of our program and allows us to repeat a set of actions multiple times. Like variables, you are probably familiar with functions from math class. Functions in code are similar to those in class - they take some data and transform it in some way. Those transformations are really useful to us - they're the work that we want the computer to do.

why ?

- package code into blocks that we can reuse.
- prevent us from writing the same code over and over again.

how ?

**Declaration**
A function is a set of instructions that we write out once and reuse over and over. We call creating a new set of instructions declaring a function.

The syntax for writing JS functions is very specific. It looks like this:

        function name() {
                   // instructions here
                };
The instructions go inside the curly braces. Let’s add some instructions inside of a function in our my_script.js file and reload our html page to run the program.

        function goGetLunch() {
                    console.log("Close Computer");
                    console.log("Stand up");
                    console.log("Walk out the door")
                       };
**Calling a function**
We use a function with its name. The name for this is calling the function. In javascript, we write it like this:

                   goGetLunch();
