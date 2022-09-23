# Technical Documentation Page

> `Certification Project`
> ## Technical Documentation Page
> - This is one of the required projects to earn your certification.
> - For this project, you will build a technical documentation page to serve as instruction or reference for a topic.

> ### **Instructions**
> **Build a Technical Documentation Page** <br>
> <br>
> **Objective:** Build an app that is functionally similar to [Technical Documentation Page](https://technical-documentation-page.freecodecamp.rocks) <br>
> <br>
> **User Stories:**
> 1. You can see a `main` element with a corresponding `id="main-doc"`, which contains the page's main content (technical documentation)
> 2. Within the `#main-doc` element, you can see several `section` elements, each with a class of `main-section`. There should be a minimum of five
> 3. The first element within each `.main-section` should be a `header` element, which contains text that describes the topic of that section
> 4. Each `section` element with the class of `main-section` should also have an `id` that corresponds with the text of each `header` contained within it. Any spaces should be replaced with underscores (e.g. The section that contains the header "JavaScript and Java" should have a corresponding `id="JavaScript_and_Java"`)
> 5. The `.main-section` elements should contain at least ten `p` elements total (not each)
> 6. The `.main-section` elements should contain at least five `code` elements total (not each)
> 7. The `.main-section` elements should contain at least five `li` items total (not each)
> 8. You can see a `nav` element with a corresponding `id="navbar"`
> 9. The navbar element should contain one `header` element which contains text that describes the topic of the technical documentation
> 10. Additionally, the navbar should contain link (`a`) elements with the class of `nav-link`. There should be one for every element with the class `main-section`
> 11. The `header` element in the `#navbar` must come before any link (`a`) elements in the navbar
> 12. Each element with the class of `nav-link` should contain text that corresponds to the `header` text within each `section` (e.g. if you have a "Hello world" section/header, your navbar should have an element which contains the text "Hello world")
> 13. When you click on a navbar element, the page should navigate to the corresponding section of the `#main-doc` element (e.g. If you click on a `.nav-link` element that contains the text "Hello world", the page navigates to a `section` element with that id, and contains the corresponding header)
> 14. On regular sized devices (laptops, desktops), the element with `id="navbar"` should be shown on the left side of the screen and should always be visible to the user
> 15. Your technical documentation should use at least one media query <br>

> Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding! <br>

> **Note:** Be sure to add ```<link rel="stylesheet" href="styles.css">``` in your HTML to link your stylesheet and apply your CSS <br>

---

> ## **Solutions** <br>
> **Follow Step by Step** <br><br>

> **Step 1** <br>
You can see a `main` element with a corresponding `id="main-doc"`, which contains the page's main content (technical documentation)

```html
#index.html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>

    <main id="main-doc">
    </main>

  </body>
</html>
```
```css
#styles.css
html,
body {
  min-width: 290px;
  color: #4d4e53;
  background-color: #ffffff;
  font-family: 'Open Sans', Arial, sans-serif;
  line-height: 1.5;
}
```
> **Step 2** <br>
Within the `#main-doc` element, you can see several `section` elements, each with a class of `main-section`. There should be a minimum of five

```html
#index.html
    <main id="main-doc">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
      <section class="main-section">
    </main>
```
```css
#styles.css
#main-doc {
  position: absolute;
  margin-left: 310px;
  padding: 20px;
  margin-bottom: 110px;
}
```
> **Step 3** <br>
The first element within each `.main-section` should be a `header` element, which contains text that describes the topic of that section

```html
#index.html
    <main id="main-doc">
      <section class="main-section">
        <header>Introduction</header>
      <section class="main-section">
        <header>What you should already know</header>
      <section class="main-section">
        <header>JavaScript and Java</header>
      <section class="main-section">
        <header>Hello world</header>
      <section class="main-section">
        <header>Variables</header>
      <section class="main-section">
        <header>Declaring variables</header>
      <section class="main-section">
        <header>Variable scope</header>
      <section class="main-section">
        <header>Global variables</header>
      <section class="main-section">
        <header>Constants</header>
      <section class="main-section">
        <header>Data types</header>
      <section class="main-section">
        <header>if...else statement</header>
      <section class="main-section">
        <header>while statement</header>
      <section class="main-section">
        <header>Function declarations</header>
      <section class="main-section">
    </main>
```
```css
#styles.css
header {
  color: black;
  margin: 10px;
  text-align: center;
  font-size: 1.8em;
  font-weight: thin;
}

#main-doc header {
  text-align: left;
  margin: 0px;
}
```
> **Step 4** <br>
Each `section` element with the class of `main-section` should also have an `id` that corresponds with the text of each `header` contained within it. Any spaces should be replaced with underscores (e.g. The section that contains the header "JavaScript and Java" should have a corresponding `id="JavaScript_and_Java"`)

```html
#index.html
    <main id="main-doc">
      <section class="main-section" id="Introduction">
        <header>Introduction</header>
      <section class="main-section" id="What_you_should_already_know">
        <header>What you should already know</header>
      <section class="main-section" id="JavaScript_and_Java">
        <header>JavaScript and Java</header>
      <section class="main-section" id="Hello_world">
        <header>Hello world</header>
      <section class="main-section" id="Variables">
        <header>Variables</header>
      <section class="main-section" id="Declaring_variables">
        <header>Declaring variables</header>
      <section class="main-section" id="Variable_scope">
        <header>Variable scope</header>
      <section class="main-section" id="Global_variables">
        <header>Global variables</header>
      <section class="main-section" id="Constants">
        <header>Constants</header>
      <section class="main-section" id="Data_types">
        <header>Data types</header>
      <section class="main-section" id="if...else_statement">
        <header>if...else statement</header>
      <section class="main-section" id="while_statement">
        <header>while statement</header>
      <section class="main-section" id="Function_declarations">
        <header>Function declarations</header>
      <section class="main-section" id="Reference">
    </main>
```
> **Step 5** <br>
The `.main-section` elements should contain at least ten `p` elements total (not each)

```html
#index.html
      <section class="main-section" id="Introduction">
        <header>Introduction</header>
        <article>
          <p>
            JavaScript is a cross-platform, object-oriented scripting language.
            It is a small and lightweight language. Inside a host environment
            (for example, a web browser), JavaScript can be connected to the
            objects of its environment to provide programmatic control over
            them.
          </p>
          <p>
            JavaScript contains a standard library of objects, such as Array,
            Date, and Math, and a core set of language elements such as
            operators, control structures, and statements. Core JavaScript can
            be extended for a variety of purposes by supplementing it with
            additional objects; for example:
          </p>
        </article>
      </section>
      <section class="main-section" id="What_you_should_already_know">
        <header>What you should already know</header>
        <article>
          <p>This guide assumes you have the following basic background:
          </p>
        </article>
      </section>
      <section class="main-section" id="JavaScript_and_Java">
        <header>JavaScript and Java</header>
        <article>
          <p>
            JavaScript and Java are similar in some ways but fundamentally
            different in some others. The JavaScript language resembles Java but
            does not have Java's static typing and strong type checking.
            JavaScript follows most Java expression syntax, naming conventions
            and basic control-flow constructs which was the reason why it was
            renamed from LiveScript to JavaScript.
          </p>
          <p>
            In contrast to Java's compile-time system of classes built by
            declarations, JavaScript supports a runtime system based on a small
            number of data types representing numeric, Boolean, and string
            values. JavaScript has a prototype-based object model instead of the
            more common class-based object model. The prototype-based model
            provides dynamic inheritance; that is, what is inherited can vary
            for individual objects. JavaScript also supports functions without
            any special declarative requirements. Functions can be properties of
            objects, executing as loosely typed methods.
          </p>
          <p>
            JavaScript is a very free-form language compared to Java. You do not
            have to declare all variables, classes, and methods. You do not have
            to be concerned with whether methods are public, private, or
            protected, and you do not have to implement interfaces. Variables,
            parameters, and function return types are not explicitly typed.
          </p>
        </article>
      </section>
      <section class="main-section" id="Hello_world">
        <header>Hello world</header>
        <article>
          To get started with writing JavaScript, open the Scratchpad and write
          your first "Hello world" JavaScript code:
          Select the code in the pad and hit Ctrl+R to watch it unfold in your
          browser!
        </article>
      </section>
      <section class="main-section" id="Variables">
        <header>Variables</header>
        <p>
          You use variables as symbolic names for values in your application.
          The names of variables, called identifiers, conform to certain rules.
        </p>
        <p>
          A JavaScript identifier must start with a letter, underscore (_), or
          dollar sign ($); subsequent characters can also be digits (0-9).
          Because JavaScript is case sensitive, letters include the characters
          "A" through "Z" (uppercase) and the characters "a" through "z"
          (lowercase).
        </p>
        <p>
          You can use ISO 8859-1 or Unicode letters such as å and ü in
          identifiers. You can also use the Unicode escape sequences as
          characters in identifiers. Some examples of legal names are
          Number_hits, temp99, and _name.
        </p>
      </section>
      <section class="main-section" id="Declaring_variables">
        <header>Declaring variables</header>
        <article>
          You can declare a variable in three ways:
        </article>
      </section>
      <section class="main-section" id="Variable_scope">
        <header>Variable scope</header>
        <article>
          <p>
            When you declare a variable outside of any function, it is called a
            global variable, because it is available to any other code in the
            current document. When you declare a variable within a function, it
            is called a local variable, because it is available only within that
            function.
          </p>
          <p>
            JavaScript before ECMAScript 2015 does not have block statement
            scope; rather, a variable declared within a block is local to the
            function (or global scope) that the block resides within. For
            example the following code will log 5, because the scope of x is the
            function (or global context) within which x is declared, not the
            block, which in this case is an if statement.
          </p>
          <p>
            This behavior changes, when using the let declaration introduced in
            ECMAScript 2015.
          </p>
        </article>
      </section>
      <section class="main-section" id="Global_variables">
        <header>Global variables</header>
        <article>
          <p>
            Global variables are in fact properties of the global object. In web
            pages the global object is window, so you can set and access global
            variables using the window.variable syntax.
          </p>
          <p>
            Consequently, you can access global variables declared in one window
            or frame from another window or frame by specifying the window or
            frame name. For example, if a variable called phoneNumber is
            declared in a document, you can refer to this variable from an
            iframe as parent.phoneNumber.
          </p>
        </article>
      </section>
      <section class="main-section" id="Constants">
        <header>Constants</header>
        <article>
          <p>
            You can create a read-only, named constant with the const keyword.
            The syntax of a constant identifier is the same as for a variable
            identifier: it must start with a letter, underscore or dollar sign
            and can contain alphabetic, numeric, or underscore characters.
          </p>
          <p>
            A constant cannot change value through assignment or be re-declared
            while the script is running. It has to be initialized to a value.
          </p>
          <p>
            The scope rules for constants are the same as those for let block
            scope variables. If the const keyword is omitted, the identifier is
            assumed to represent a variable.
          </p>
          <p>
            You cannot declare a constant with the same name as a function or
            variable in the same scope. For example:
          </p>
        </article>
      </section>
      <section class="main-section" id="Data_types">
        <header>Data types</header>
        <article>
          <p>The latest ECMAScript standard defines seven data types:</p>
          Although these data types are a relatively small amount, they enable
          you to perform useful functions with your applications. Objects and
          functions are the other fundamental elements in the language. You can
          think of objects as named containers for values, and functions as
          procedures that your application can perform.
        </article>
      </section>
      <section class="main-section" id="if...else_statement">
        <header>if...else statement</header>
        <article>
          Use the if statement to execute a statement if a logical condition is
          true. Use the optional else clause to execute a statement if the
          condition is false. An if statement looks as follows:
          <p>
            You may also compound the statements using else if to have multiple
            conditions tested in sequence, as follows:
          </p>
        </article>
      </section>
      <section class="main-section" id="while_statement">
        <header>while statement</header>
        <article>
          A while statement executes its statements as long as a specified
          condition evaluates to true. A while statement looks as follows:
          If the condition becomes
          false, statement within the loop stops executing and control passes to
          the statement following the loop.
          <p>
            The condition test occurs before statement in the loop is executed.
            If the condition returns true, statement is executed and the
            condition is tested again. If the condition returns false, execution
            stops and control is passed to the statement following while.
          </p>
          <p>
            To execute multiple statements, use a block statement ({ ... }) to
            group those statements.
          </p>
          <p>
            The following while loop iterates as long as n is less than three:
          </p>
          <p>
            With each iteration, the loop increments n and adds that value to x.
            Therefore, x and n take on the following values:
          </p>
          <p>
            After completing the third pass, the condition n &lt; 3 is no longer
            true, so the loop terminates.
          </p>
        </article>
      </section>
      <section class="main-section" id="Function_declarations">
        <header>Function declarations</header>
        <article>
          A function definition (also called a function declaration, or function
          statement) consists of the function keyword, followed by:
          <p>
            For example, the following code defines a simple function named
            square:
          </p>
          <p>
            The function square takes one argument, called number. The function
            consists of one statement that says to return the argument of the
            function (that is, number) multiplied by itself. The return
            statement specifies the value returned by the function.
          </p>
          <p>
            Primitive parameters (such as a number) are passed to functions by
            value; the value is passed to the function, but if the function
            changes the value of the parameter, this change is not reflected
            globally or in the calling function.
          </p>
        </article>
      </section>
      <section class="main-section" id="Reference">
        <header>Reference</header>
        <article>
        </article>
      </section>
```
```css
#styles.css
#main-doc {
  position: absolute;
  margin-left: 310px;
  padding: 20px;
  margin-bottom: 110px;
}

section article {
  color: #4d4e53;
  margin: 15px;
  font-size: 0.96em;
}
```
> **Step 6** <br>
The `.main-section` elements should contain at least five `code` elements total (not each)

```html
#index.html
      <section class="main-section" id="Introduction">
        <header>Introduction</header>
        <article>
          <p>
            JavaScript is a cross-platform, object-oriented scripting language.
            It is a small and lightweight language. Inside a host environment
            (for example, a web browser), JavaScript can be connected to the
            objects of its environment to provide programmatic control over
            them.
          </p>
          <p>
            JavaScript contains a standard library of objects, such as Array,
            Date, and Math, and a core set of language elements such as
            operators, control structures, and statements. Core JavaScript can
            be extended for a variety of purposes by supplementing it with
            additional objects; for example:
          </p>
        </article>
      </section>
      <section class="main-section" id="What_you_should_already_know">
        <header>What you should already know</header>
        <article>
          <p>This guide assumes you have the following basic background:
          </p>
        </article>
      </section>
      <section class="main-section" id="JavaScript_and_Java">
        <header>JavaScript and Java</header>
        <article>
          <p>
            JavaScript and Java are similar in some ways but fundamentally
            different in some others. The JavaScript language resembles Java but
            does not have Java's static typing and strong type checking.
            JavaScript follows most Java expression syntax, naming conventions
            and basic control-flow constructs which was the reason why it was
            renamed from LiveScript to JavaScript.
          </p>
          <p>
            In contrast to Java's compile-time system of classes built by
            declarations, JavaScript supports a runtime system based on a small
            number of data types representing numeric, Boolean, and string
            values. JavaScript has a prototype-based object model instead of the
            more common class-based object model. The prototype-based model
            provides dynamic inheritance; that is, what is inherited can vary
            for individual objects. JavaScript also supports functions without
            any special declarative requirements. Functions can be properties of
            objects, executing as loosely typed methods.
          </p>
          <p>
            JavaScript is a very free-form language compared to Java. You do not
            have to declare all variables, classes, and methods. You do not have
            to be concerned with whether methods are public, private, or
            protected, and you do not have to implement interfaces. Variables,
            parameters, and function return types are not explicitly typed.
          </p>
        </article>
      </section>
      <section class="main-section" id="Hello_world">
        <header>Hello world</header>
        <article>
          To get started with writing JavaScript, open the Scratchpad and write
          your first "Hello world" JavaScript code:
          <code>
            function greetMe(yourName) { alert("Hello " + yourName); }
            greetMe("World");
          </code>
          Select the code in the pad and hit Ctrl+R to watch it unfold in your
          browser!
        </article>
      </section>
      <section class="main-section" id="Variables">
        <header>Variables</header>
        <p>
          You use variables as symbolic names for values in your application.
          The names of variables, called identifiers, conform to certain rules.
        </p>
        <p>
          A JavaScript identifier must start with a letter, underscore (_), or
          dollar sign ($); subsequent characters can also be digits (0-9).
          Because JavaScript is case sensitive, letters include the characters
          "A" through "Z" (uppercase) and the characters "a" through "z"
          (lowercase).
        </p>
        <p>
          You can use ISO 8859-1 or Unicode letters such as å and ü in
          identifiers. You can also use the Unicode escape sequences as
          characters in identifiers. Some examples of legal names are
          Number_hits, temp99, and _name.
        </p>
      </section>
      <section class="main-section" id="Declaring_variables">
        <header>Declaring variables</header>
        <article>
          You can declare a variable in three ways:
          <p>
            With the keyword var. For example, <code>var x = 42.</code> This
            syntax can be used to declare both local and global variables.
          </p>
          <p>
            By simply assigning it a value. For example,
            <code>x = 42.</code> This always declares a global variable. It
            generates a strict JavaScript warning. You shouldn't use this
            variant.
          </p>
          <p>
            With the keyword let. For example,<code> let y = 13.</code> This
            syntax can be used to declare a block scope local variable. See
            Variable scope below.
          </p>
        </article>
      </section>
      <section class="main-section" id="Variable_scope">
        <header>Variable scope</header>
        <article>
          <p>
            When you declare a variable outside of any function, it is called a
            global variable, because it is available to any other code in the
            current document. When you declare a variable within a function, it
            is called a local variable, because it is available only within that
            function.
          </p>
          <p>
            JavaScript before ECMAScript 2015 does not have block statement
            scope; rather, a variable declared within a block is local to the
            function (or global scope) that the block resides within. For
            example the following code will log 5, because the scope of x is the
            function (or global context) within which x is declared, not the
            block, which in this case is an if statement.
          </p>
          <code>if (true) { var x = 5; } console.log(x); // 5</code>
          <p>
            This behavior changes, when using the let declaration introduced in
            ECMAScript 2015.
          </p>
          <code>
            if (true) { let y = 5; } console.log(y); // ReferenceError: y is
            not defined
          </code>
        </article>
      </section>
      <section class="main-section" id="Global_variables">
        <header>Global variables</header>
        <article>
          <p>
            Global variables are in fact properties of the global object. In web
            pages the global object is window, so you can set and access global
            variables using the window.variable syntax.
          </p>
          <p>
            Consequently, you can access global variables declared in one window
            or frame from another window or frame by specifying the window or
            frame name. For example, if a variable called phoneNumber is
            declared in a document, you can refer to this variable from an
            iframe as parent.phoneNumber.
          </p>
        </article>
      </section>
      <section class="main-section" id="Constants">
        <header>Constants</header>
        <article>
          <p>
            You can create a read-only, named constant with the const keyword.
            The syntax of a constant identifier is the same as for a variable
            identifier: it must start with a letter, underscore or dollar sign
            and can contain alphabetic, numeric, or underscore characters.
          </p>
          <code>const PI = 3.14;</code>
          <p>
            A constant cannot change value through assignment or be re-declared
            while the script is running. It has to be initialized to a value.
          </p>
          <p>
            The scope rules for constants are the same as those for let block
            scope variables. If the const keyword is omitted, the identifier is
            assumed to represent a variable.
          </p>
          <p>
            You cannot declare a constant with the same name as a function or
            variable in the same scope. For example:
          </p>
          <code>// THIS WILL CAUSE AN ERROR function f() {}; const f = 5; // THIS
            WILL CAUSE AN ERROR ALSO function f() { const g = 5; var g;
            //statements }
          </code>
          However, object attributes are not protected, so the following
          statement is executed without problems.
          <code>const MY_OBJECT = {"key": "value"}; MY_OBJECT.key =
            "otherValue";
          </code>
        </article>
      </section>
      <section class="main-section" id="Data_types">
        <header>Data types</header>
        <article>
          <p>The latest ECMAScript standard defines seven data types:</p>
          Although these data types are a relatively small amount, they enable
          you to perform useful functions with your applications. Objects and
          functions are the other fundamental elements in the language. You can
          think of objects as named containers for values, and functions as
          procedures that your application can perform.
        </article>
      </section>
      <section class="main-section" id="if...else_statement">
        <header>if...else statement</header>
        <article>
          Use the if statement to execute a statement if a logical condition is
          true. Use the optional else clause to execute a statement if the
          condition is false. An if statement looks as follows:
          <code>
            if (condition) { statement_1; } else { statement_2; }
          </code>
          condition can be any expression that evaluates to true or false. See
          Boolean for an explanation of what evaluates to true and false. If
          condition evaluates to true, statement_1 is executed; otherwise,
          statement_2 is executed. statement_1 and statement_2 can be any
          statement, including further nested if statements.
          <p>
            You may also compound the statements using else if to have multiple
            conditions tested in sequence, as follows:
          </p>
          <code>
            if (condition_1) { statement_1; } else if (condition_2) {
            statement_2; } else if (condition_n) { statement_n; } else {
            statement_last; }
          </code>
          In the case of multiple conditions only the first logical condition
          which evaluates to true will be executed. To execute multiple
          statements, group them within a block statement ({ ... }) . In
          general, it's good practice to always use block statements, especially
          when nesting if statements:
          <code>
            if (condition) { statement_1_runs_if_condition_is_true;
            statement_2_runs_if_condition_is_true; } else {
            statement_3_runs_if_condition_is_false;
            statement_4_runs_if_condition_is_false; }
          </code>
          It is advisable to not use simple assignments in a conditional
          expression, because the assignment can be confused with equality when
          glancing over the code. For example, do not use the following code:
          <code>if (x = y) { /* statements here */ }</code> If you need to use
          an assignment in a conditional expression, a common practice is to put
          additional parentheses around the assignment. For example:
          <code>if ((x = y)) { /* statements here */ }</code>
        </article>
      </section>
      <section class="main-section" id="while_statement">
        <header>while statement</header>
        <article>
          A while statement executes its statements as long as a specified
          condition evaluates to true. A while statement looks as follows:
          <code>while (condition) statement</code> 
          If the condition becomes
          false, statement within the loop stops executing and control passes to
          the statement following the loop.
          <p>
            The condition test occurs before statement in the loop is executed.
            If the condition returns true, statement is executed and the
            condition is tested again. If the condition returns false, execution
            stops and control is passed to the statement following while.
          </p>
          <p>
            To execute multiple statements, use a block statement ({ ... }) to
            group those statements.
          </p>
          Example:
          <p>
            The following while loop iterates as long as n is less than three:
          </p>
          <code>
            var n = 0; var x = 0; while (n &lt; 3) { n++; x += n; }
          </code>
          <p>
            With each iteration, the loop increments n and adds that value to x.
            Therefore, x and n take on the following values:
          </p>
          <p>
            After completing the third pass, the condition n &lt; 3 is no longer
            true, so the loop terminates.
          </p>
        </article>
      </section>
      <section class="main-section" id="Function_declarations">
        <header>Function declarations</header>
        <article>
          A function definition (also called a function declaration, or function
          statement) consists of the function keyword, followed by:
          <p>
            For example, the following code defines a simple function named
            square:
          </p>
          <code>function square(number) { return number * number; }</code>
          <p>
            The function square takes one argument, called number. The function
            consists of one statement that says to return the argument of the
            function (that is, number) multiplied by itself. The return
            statement specifies the value returned by the function.
          </p>
          <code>return number * number;</code>
          <p>
            Primitive parameters (such as a number) are passed to functions by
            value; the value is passed to the function, but if the function
            changes the value of the parameter, this change is not reflected
            globally or in the calling function.
          </p>
        </article>
      </section>
      <section class="main-section" id="Reference">
        <header>Reference</header>
        <article>
        </article>
      </section>
```
```css
#styles.css
code {
  display: block;
  text-align: left;
  white-space: pre-line;
  position: relative;
  word-break: normal;
  word-wrap: normal;
  line-height: 2;
  background-color: #f7f7f7;
  padding: 15px;
  margin: 10px;
  border-radius: 5px;
}
```
> **Step 7** <br>
The `.main-section` elements should contain at least five `li` items total (not each)

```html
#index.html
      <section class="main-section" id="Introduction">
        <header>Introduction</header>
        <article>
          <p>
            JavaScript is a cross-platform, object-oriented scripting language.
            It is a small and lightweight language. Inside a host environment
            (for example, a web browser), JavaScript can be connected to the
            objects of its environment to provide programmatic control over
            them.
          </p>

          <p>
            JavaScript contains a standard library of objects, such as Array,
            Date, and Math, and a core set of language elements such as
            operators, control structures, and statements. Core JavaScript can
            be extended for a variety of purposes by supplementing it with
            additional objects; for example:
          </p>
          <ul>
            <li>
              Client-side JavaScript extends the core language by supplying
              objects to control a browser and its Document Object Model (DOM).
              For example, client-side extensions allow an application to place
              elements on an HTML form and respond to user events such as mouse
              clicks, form input, and page navigation.
            </li>
            <li>
              Server-side JavaScript extends the core language by supplying
              objects relevant to running JavaScript on a server. For example,
              server-side extensions allow an application to communicate with a
              database, provide continuity of information from one invocation to
              another of the application, or perform file manipulations on a
              server.
            </li>
          </ul>
        </article>
      </section>
      <section class="main-section" id="What_you_should_already_know">
        <header>What you should already know</header>
        <article>
          <p>This guide assumes you have the following basic background:</p>

          <ul>
            <li>
              A general understanding of the Internet and the World Wide Web
              (WWW).
            </li>
            <li>Good working knowledge of HyperText Markup Language (HTML).</li>
            <li>
              Some programming experience. If you are new to programming, try
              one of the tutorials linked on the main page about JavaScript.
            </li>
          </ul>
        </article>
      </section>
      <section class="main-section" id="JavaScript_and_Java">
        <header>JavaScript and Java</header>
        <article>
          <p>
            JavaScript and Java are similar in some ways but fundamentally
            different in some others. The JavaScript language resembles Java but
            does not have Java's static typing and strong type checking.
            JavaScript follows most Java expression syntax, naming conventions
            and basic control-flow constructs which was the reason why it was
            renamed from LiveScript to JavaScript.
          </p>

          <p>
            In contrast to Java's compile-time system of classes built by
            declarations, JavaScript supports a runtime system based on a small
            number of data types representing numeric, Boolean, and string
            values. JavaScript has a prototype-based object model instead of the
            more common class-based object model. The prototype-based model
            provides dynamic inheritance; that is, what is inherited can vary
            for individual objects. JavaScript also supports functions without
            any special declarative requirements. Functions can be properties of
            objects, executing as loosely typed methods.
          </p>
          <p>
            JavaScript is a very free-form language compared to Java. You do not
            have to declare all variables, classes, and methods. You do not have
            to be concerned with whether methods are public, private, or
            protected, and you do not have to implement interfaces. Variables,
            parameters, and function return types are not explicitly typed.
          </p>
        </article>
      </section>
      <section class="main-section" id="Hello_world">
        <header>Hello world</header>
        <article>
          To get started with writing JavaScript, open the Scratchpad and write
          your first "Hello world" JavaScript code:
          <code
            >function greetMe(yourName) { alert("Hello " + yourName); }
            greetMe("World");
          </code>

          Select the code in the pad and hit Ctrl+R to watch it unfold in your
          browser!
        </article>
      </section>
      <section class="main-section" id="Variables">
        <header>Variables</header>
        <p>
          You use variables as symbolic names for values in your application.
          The names of variables, called identifiers, conform to certain rules.
        </p>
        <p>
          A JavaScript identifier must start with a letter, underscore (_), or
          dollar sign ($); subsequent characters can also be digits (0-9).
          Because JavaScript is case sensitive, letters include the characters
          "A" through "Z" (uppercase) and the characters "a" through "z"
          (lowercase).
        </p>
        <p>
          You can use ISO 8859-1 or Unicode letters such as å and ü in
          identifiers. You can also use the Unicode escape sequences as
          characters in identifiers. Some examples of legal names are
          Number_hits, temp99, and _name.
        </p>
      </section>
      <section class="main-section" id="Declaring_variables">
        <header>Declaring variables</header>
        <article>
          You can declare a variable in three ways:
          <p>
            With the keyword var. For example, <code>var x = 42.</code> This
            syntax can be used to declare both local and global variables.
          </p>
          <p>
            By simply assigning it a value. For example,
            <code>x = 42.</code> This always declares a global variable. It
            generates a strict JavaScript warning. You shouldn't use this
            variant.
          </p>
          <p>
            With the keyword let. For example,<code> let y = 13.</code> This
            syntax can be used to declare a block scope local variable. See
            Variable scope below.
          </p>
        </article>
      </section>
      <section class="main-section" id="Variable_scope">
        <header>Variable scope</header>
        <article>
          <p>
            When you declare a variable outside of any function, it is called a
            global variable, because it is available to any other code in the
            current document. When you declare a variable within a function, it
            is called a local variable, because it is available only within that
            function.
          </p>

          <p>
            JavaScript before ECMAScript 2015 does not have block statement
            scope; rather, a variable declared within a block is local to the
            function (or global scope) that the block resides within. For
            example the following code will log 5, because the scope of x is the
            function (or global context) within which x is declared, not the
            block, which in this case is an if statement.
          </p>
          <code>if (true) { var x = 5; } console.log(x); // 5</code>
          <p>
            This behavior changes, when using the let declaration introduced in
            ECMAScript 2015.
          </p>

          <code
            >if (true) { let y = 5; } console.log(y); // ReferenceError: y is
            not defined</code
          >
        </article>
      </section>
      <section class="main-section" id="Global_variables">
        <header>Global variables</header>
        <article>
          <p>
            Global variables are in fact properties of the global object. In web
            pages the global object is window, so you can set and access global
            variables using the window.variable syntax.
          </p>

          <p>
            Consequently, you can access global variables declared in one window
            or frame from another window or frame by specifying the window or
            frame name. For example, if a variable called phoneNumber is
            declared in a document, you can refer to this variable from an
            iframe as parent.phoneNumber.
          </p>
        </article>
      </section>
      <section class="main-section" id="Constants">
        <header>Constants</header>
        <article>
          <p>
            You can create a read-only, named constant with the const keyword.
            The syntax of a constant identifier is the same as for a variable
            identifier: it must start with a letter, underscore or dollar sign
            and can contain alphabetic, numeric, or underscore characters.
          </p>

          <code>const PI = 3.14;</code>
          <p>
            A constant cannot change value through assignment or be re-declared
            while the script is running. It has to be initialized to a value.
          </p>

          <p>
            The scope rules for constants are the same as those for let block
            scope variables. If the const keyword is omitted, the identifier is
            assumed to represent a variable.
          </p>

          <p>
            You cannot declare a constant with the same name as a function or
            variable in the same scope. For example:
          </p>

          <code
            >// THIS WILL CAUSE AN ERROR function f() {}; const f = 5; // THIS
            WILL CAUSE AN ERROR ALSO function f() { const g = 5; var g;
            //statements }</code
          >
          However, object attributes are not protected, so the following
          statement is executed without problems.
          <code
            >const MY_OBJECT = {"key": "value"}; MY_OBJECT.key =
            "otherValue";</code
          >
        </article>
      </section>
      <section class="main-section" id="Data_types">
        <header>Data types</header>
        <article>
          <p>The latest ECMAScript standard defines seven data types:</p>
          <ul>
            <li>
              <p>Six data types that are primitives:</p>
              <ul>
                <li>Boolean. true and false.</li>
                <li>
                  null. A special keyword denoting a null value. Because
                  JavaScript is case-sensitive, null is not the same as Null,
                  NULL, or any other variant.
                </li>
                <li>
                  undefined. A top-level property whose value is undefined.
                </li>
                <li>Number. 42 or 3.14159.</li>
                <li>String. "Howdy"</li>
                <li>
                  Symbol (new in ECMAScript 2015). A data type whose instances
                  are unique and immutable.
                </li>
              </ul>
            </li>

            <li>and Object</li>
          </ul>
          Although these data types are a relatively small amount, they enable
          you to perform useful functions with your applications. Objects and
          functions are the other fundamental elements in the language. You can
          think of objects as named containers for values, and functions as
          procedures that your application can perform.
        </article>
      </section>
      <section class="main-section" id="if...else_statement">
        <header>if...else statement</header>
        <article>
          Use the if statement to execute a statement if a logical condition is
          true. Use the optional else clause to execute a statement if the
          condition is false. An if statement looks as follows:

          <code>if (condition) { statement_1; } else { statement_2; }</code>
          condition can be any expression that evaluates to true or false. See
          Boolean for an explanation of what evaluates to true and false. If
          condition evaluates to true, statement_1 is executed; otherwise,
          statement_2 is executed. statement_1 and statement_2 can be any
          statement, including further nested if statements.
          <p>
            You may also compound the statements using else if to have multiple
            conditions tested in sequence, as follows:
          </p>
          <code
            >if (condition_1) { statement_1; } else if (condition_2) {
            statement_2; } else if (condition_n) { statement_n; } else {
            statement_last; }
          </code>
          In the case of multiple conditions only the first logical condition
          which evaluates to true will be executed. To execute multiple
          statements, group them within a block statement ({ ... }) . In
          general, it's good practice to always use block statements, especially
          when nesting if statements:

          <code
            >if (condition) { statement_1_runs_if_condition_is_true;
            statement_2_runs_if_condition_is_true; } else {
            statement_3_runs_if_condition_is_false;
            statement_4_runs_if_condition_is_false; }</code
          >
          It is advisable to not use simple assignments in a conditional
          expression, because the assignment can be confused with equality when
          glancing over the code. For example, do not use the following code:
          <code>if (x = y) { /* statements here */ }</code> If you need to use
          an assignment in a conditional expression, a common practice is to put
          additional parentheses around the assignment. For example:

          <code>if ((x = y)) { /* statements here */ }</code>
        </article>
      </section>
      <section class="main-section" id="while_statement">
        <header>while statement</header>
        <article>
          A while statement executes its statements as long as a specified
          condition evaluates to true. A while statement looks as follows:

          <code>while (condition) statement</code> If the condition becomes
          false, statement within the loop stops executing and control passes to
          the statement following the loop.

          <p>
            The condition test occurs before statement in the loop is executed.
            If the condition returns true, statement is executed and the
            condition is tested again. If the condition returns false, execution
            stops and control is passed to the statement following while.
          </p>

          <p>
            To execute multiple statements, use a block statement ({ ... }) to
            group those statements.
          </p>

          Example:

          <p>
            The following while loop iterates as long as n is less than three:
          </p>

          <code>var n = 0; var x = 0; while (n &lt; 3) { n++; x += n; }</code>
          <p>
            With each iteration, the loop increments n and adds that value to x.
            Therefore, x and n take on the following values:
          </p>

          <ul>
            <li>After the first pass: n = 1 and x = 1</li>
            <li>After the second pass: n = 2 and x = 3</li>
            <li>After the third pass: n = 3 and x = 6</li>
          </ul>
          <p>
            After completing the third pass, the condition n &lt; 3 is no longer
            true, so the loop terminates.
          </p>
        </article>
      </section>
      <section class="main-section" id="Function_declarations">
        <header>Function declarations</header>
        <article>
          A function definition (also called a function declaration, or function
          statement) consists of the function keyword, followed by:

          <ul>
            <li>The name of the function.</li>
            <li>
              A list of arguments to the function, enclosed in parentheses and
              separated by commas.
            </li>
            <li>
              The JavaScript statements that define the function, enclosed in
              curly brackets, { }.
            </li>
          </ul>
          <p>
            For example, the following code defines a simple function named
            square:
          </p>

          <code>function square(number) { return number * number; }</code>
          <p>
            The function square takes one argument, called number. The function
            consists of one statement that says to return the argument of the
            function (that is, number) multiplied by itself. The return
            statement specifies the value returned by the function.
          </p>
          <code>return number * number;</code>
          <p>
            Primitive parameters (such as a number) are passed to functions by
            value; the value is passed to the function, but if the function
            changes the value of the parameter, this change is not reflected
            globally or in the calling function.
          </p>
        </article>
      </section>
      <section class="main-section" id="Reference">
        <header>Reference</header>
        <article>
          <ul>
            <li>
              All the documentation in this page is taken from
              <a
                href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide"
                target="_blank"
                >MDN</a
              >
            </li>
          </ul>
        </article>
      </section>
```
```css
#styles.css
section li {
  margin: 15px 0px 0px 20px;
}
```
> **Step 8** <br>
You can see a `nav` element with a corresponding `id="navbar"`

```html
#index.html
    <nav id="navbar">
    </nav>
```
```css
#styles.css
#navbar {
  position: fixed;
  min-width: 290px;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 100%;
  border-right: solid;
  border-color: rgba(0, 22, 22, 0.4);
}
```
> **Step 9** <br>
The navbar element should contain one `header` element which contains text that describes the topic of the technical documentation

```html
#index.html
    <nav id="navbar">
      <header>JS Documentation</header>
      <ul>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </nav>
```
```css
#styles.css
header {
  color: black;
  margin: 10px;
  text-align: center;
  font-size: 1.8em;
  font-weight: thin;
}
```
> **Step 10** <br>
Additionally, the navbar should contain link (`a`) elements with the class of `nav-link`. There should be one for every element with the class `main-section`

```html
#index.html
    <nav id="navbar">
      <header>JS Documentation</header>
      <ul>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
          <a class="nav-link"></a>
        </li>
        <li>
          <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
          <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
          <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
          <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
        <li>
          <a class="nav-link"></a>
        </li>
        <li>
            <a class="nav-link"></a>
        </li>
      </ul>
    </nav>
```
```css
#styles.css
#navbar ul {
  height: 88%;
  padding: 0;
  overflow-y: auto;
  overflow-x: hidden;
}

#navbar li {
  color: #4d4e53;
  border-top: 1px solid;
  list-style: none;
  position: relative;
  width: 100%;
}
```
> **Step 11** <br>
The `header` element in the `#navbar` must come before any link (`a`) elements in the navbar

```html
#index.html
    <nav id="navbar">
      <header>JS Documentation</header>
      <ul>
        <li><a class="nav-link" href="#Introduction"></a></li>
        <li>
          <a class="nav-link" href="#What_you_should_already_know"
            ></a
          >
        </li>
        <li>
          <a class="nav-link" href="#JavaScript_and_Java"
            ></a
          >
        </li>
        <li><a class="nav-link" href="#Hello_world"></a></li>
        <li><a class="nav-link" href="#Variables"></a></li>
        <li>
          <a class="nav-link" href="#Declaring_variables"
            ></a
          >
        </li>
        <li><a class="nav-link" href="#Variable_scope"></a></li>
        <li>
          <a class="nav-link" href="#Global_variables"></a>
        </li>
        <li><a class="nav-link" href="#Constants"></a></li>
        <li><a class="nav-link" href="#Data_types"></a></li>
        <li>
          <a class="nav-link" href="#if...else_statement"
            ></a
          >
        </li>
        <li><a class="nav-link" href="#while_statement">while statement</a></li>
        <li>
          <a class="nav-link" href="#Function_declarations"
            ></a
          >
        </li>
        <li><a class="nav-link" href="#Reference"></a></li>
      </ul>
    </nav>
```
```css
#styles.css
#navbar a {
  display: block;
  padding: 10px 30px;
  color: #4d4e53;
  text-decoration: none;
  cursor: pointer;
}
```
> **Step 12** <br>
Each element with the class of `nav-link` should contain text that corresponds to the `header` text within each `section` (e.g. if you have a "Hello world" section/header, your navbar should have an element which contains the text "Hello world")

```html
#index.html
    <nav id="navbar">
      <header>JS Documentation</header>
      <ul>
        <li><a class="nav-link" href="#Introduction">Introduction</a></li>
        <li>
          <a class="nav-link" href="#What_you_should_already_know"
            >What you should already know</a
          >
        </li>
        <li>
          <a class="nav-link" href="#JavaScript_and_Java"
            >JavaScript and Java</a
          >
        </li>
        <li><a class="nav-link" href="#Hello_world">Hello world</a></li>
        <li><a class="nav-link" href="#Variables">Variables</a></li>
        <li>
          <a class="nav-link" href="#Declaring_variables"
            >Declaring variables</a
          >
        </li>
        <li><a class="nav-link" href="#Variable_scope">Variable scope</a></li>
        <li>
          <a class="nav-link" href="#Global_variables">Global variables</a>
        </li>
        <li><a class="nav-link" href="#Constants">Constants</a></li>
        <li><a class="nav-link" href="#Data_types">Data types</a></li>
        <li>
          <a class="nav-link" href="#if...else_statement"
            >if...else statement</a
          >
        </li>
        <li><a class="nav-link" href="#while_statement">while statement</a></li>
        <li>
          <a class="nav-link" href="#Function_declarations"
            >Function declarations</a
          >
        </li>
        <li><a class="nav-link" href="#Reference">Reference</a></li>
      </ul>
    </nav>
```
> **Step 13** <br>
When you click on a navbar element, the page should navigate to the corresponding section of the `#main-doc` element (e.g. If you click on a `.nav-link` element that contains the text "Hello world", the page navigates to a `section` element with that id, and contains the corresponding header)

```html
#index.html
    <nav id="navbar">
      <header>JS Documentation</header>
      <ul>
        <li><a class="nav-link" href="#Introduction">Introduction</a></li>
        <li>
          <a class="nav-link" href="#What_you_should_already_know"
            >What you should already know</a
          >
        </li>
        <li>
          <a class="nav-link" href="#JavaScript_and_Java"
            >JavaScript and Java</a
          >
        </li>
        <li><a class="nav-link" href="#Hello_world">Hello world</a></li>
        <li><a class="nav-link" href="#Variables">Variables</a></li>
        <li>
          <a class="nav-link" href="#Declaring_variables"
            >Declaring variables</a
          >
        </li>
        <li><a class="nav-link" href="#Variable_scope">Variable scope</a></li>
        <li>
          <a class="nav-link" href="#Global_variables">Global variables</a>
        </li>
        <li><a class="nav-link" href="#Constants">Constants</a></li>
        <li><a class="nav-link" href="#Data_types">Data types</a></li>
        <li>
          <a class="nav-link" href="#if...else_statement"
            >if...else statement</a
          >
        </li>
        <li><a class="nav-link" href="#while_statement">while statement</a></li>
        <li>
          <a class="nav-link" href="#Function_declarations"
            >Function declarations</a
          >
        </li>
        <li><a class="nav-link" href="#Reference">Reference</a></li>
      </ul>
    </nav>
    <main id="main-doc">
      <section class="main-section" id="Introduction">
        <header>Introduction</header>
        <article>
          <p>
            JavaScript is a cross-platform, object-oriented scripting language.
            It is a small and lightweight language. Inside a host environment
            (for example, a web browser), JavaScript can be connected to the
            objects of its environment to provide programmatic control over
            them.
          </p>

          <p>
            JavaScript contains a standard library of objects, such as Array,
            Date, and Math, and a core set of language elements such as
            operators, control structures, and statements. Core JavaScript can
            be extended for a variety of purposes by supplementing it with
            additional objects; for example:
          </p>
          <ul>
            <li>
              Client-side JavaScript extends the core language by supplying
              objects to control a browser and its Document Object Model (DOM).
              For example, client-side extensions allow an application to place
              elements on an HTML form and respond to user events such as mouse
              clicks, form input, and page navigation.
            </li>
            <li>
              Server-side JavaScript extends the core language by supplying
              objects relevant to running JavaScript on a server. For example,
              server-side extensions allow an application to communicate with a
              database, provide continuity of information from one invocation to
              another of the application, or perform file manipulations on a
              server.
            </li>
          </ul>
        </article>
      </section>
    </main>

    <!---->
```
> **Note:** Respectively, the others must contain a `.nav-link` element with their own headers. The page goes to a `section` element with that id and contains the corresponding header) <br>
> **Note:** It's all written as a whole at the bottom of the last step **(Step 15)** so that there isn't too much code duplication.
> **Step 14** <br>
On regular sized devices (laptops, desktops), the element with `id="navbar"` should be shown on the left side of the screen and should always be visible to the user

```css
#styles.css
#navbar {
  position: fixed;
  min-width: 290px;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 100%;
  border-right: solid;
  border-color: rgba(0, 22, 22, 0.4);
}
```
> **Step 15** <br>
Your technical documentation should use at least one media query

```css
#styles.css
@media only screen and (max-width: 815px) {
  /* For mobile phones: */
  #navbar ul {
    border: 1px solid;
    height: 207px;
  }

  #navbar {
    background-color: white;
    position: absolute;
    top: 0;
    padding: 0;
    margin: 0;
    width: 100%;
    max-height: 275px;
    border: none;
    z-index: 1;
    border-bottom: 2px solid;
  }

  #main-doc {
    position: relative;
    margin-left: 0px;
    margin-top: 270px;
  }
}

@media only screen and (max-width: 400px) {
  #main-doc {
    margin-left: -10px;
  }

  code {
    margin-left: -20px;
    width: 100%;
    padding: 15px;
    padding-left: 10px;
    padding-right: 45px;
    min-width: 233px;
  }
}
```

> **Note:** Be sure to add ```<link rel="stylesheet" href="styles.css">``` in your HTML to link your stylesheet and apply your CSS <br>
> <br>

```html
#index.html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <nav id="navbar">
      <header>JS Documentation</header>
      <ul>
        <li><a class="nav-link" href="#Introduction">Introduction</a></li>
        <li>
          <a class="nav-link" href="#What_you_should_already_know"
            >What you should already know</a
          >
        </li>
        <li>
          <a class="nav-link" href="#JavaScript_and_Java"
            >JavaScript and Java</a
          >
        </li>
        <li><a class="nav-link" href="#Hello_world">Hello world</a></li>
        <li><a class="nav-link" href="#Variables">Variables</a></li>
        <li>
          <a class="nav-link" href="#Declaring_variables"
            >Declaring variables</a
          >
        </li>
        <li><a class="nav-link" href="#Variable_scope">Variable scope</a></li>
        <li>
          <a class="nav-link" href="#Global_variables">Global variables</a>
        </li>
        <li><a class="nav-link" href="#Constants">Constants</a></li>
        <li><a class="nav-link" href="#Data_types">Data types</a></li>
        <li>
          <a class="nav-link" href="#if...else_statement"
            >if...else statement</a
          >
        </li>
        <li><a class="nav-link" href="#while_statement">while statement</a></li>
        <li>
          <a class="nav-link" href="#Function_declarations"
            >Function declarations</a
          >
        </li>
        <li><a class="nav-link" href="#Reference">Reference</a></li>
      </ul>
    </nav>
    <main id="main-doc">
      <section class="main-section" id="Introduction">
        <header>Introduction</header>
        <article>
          <p>
            JavaScript is a cross-platform, object-oriented scripting language.
            It is a small and lightweight language. Inside a host environment
            (for example, a web browser), JavaScript can be connected to the
            objects of its environment to provide programmatic control over
            them.
          </p>

          <p>
            JavaScript contains a standard library of objects, such as Array,
            Date, and Math, and a core set of language elements such as
            operators, control structures, and statements. Core JavaScript can
            be extended for a variety of purposes by supplementing it with
            additional objects; for example:
          </p>
          <ul>
            <li>
              Client-side JavaScript extends the core language by supplying
              objects to control a browser and its Document Object Model (DOM).
              For example, client-side extensions allow an application to place
              elements on an HTML form and respond to user events such as mouse
              clicks, form input, and page navigation.
            </li>
            <li>
              Server-side JavaScript extends the core language by supplying
              objects relevant to running JavaScript on a server. For example,
              server-side extensions allow an application to communicate with a
              database, provide continuity of information from one invocation to
              another of the application, or perform file manipulations on a
              server.
            </li>
          </ul>
        </article>
      </section>
      <section class="main-section" id="What_you_should_already_know">
        <header>What you should already know</header>
        <article>
          <p>This guide assumes you have the following basic background:</p>

          <ul>
            <li>
              A general understanding of the Internet and the World Wide Web
              (WWW).
            </li>
            <li>Good working knowledge of HyperText Markup Language (HTML).</li>
            <li>
              Some programming experience. If you are new to programming, try
              one of the tutorials linked on the main page about JavaScript.
            </li>
          </ul>
        </article>
      </section>
      <section class="main-section" id="JavaScript_and_Java">
        <header>JavaScript and Java</header>
        <article>
          <p>
            JavaScript and Java are similar in some ways but fundamentally
            different in some others. The JavaScript language resembles Java but
            does not have Java's static typing and strong type checking.
            JavaScript follows most Java expression syntax, naming conventions
            and basic control-flow constructs which was the reason why it was
            renamed from LiveScript to JavaScript.
          </p>

          <p>
            In contrast to Java's compile-time system of classes built by
            declarations, JavaScript supports a runtime system based on a small
            number of data types representing numeric, Boolean, and string
            values. JavaScript has a prototype-based object model instead of the
            more common class-based object model. The prototype-based model
            provides dynamic inheritance; that is, what is inherited can vary
            for individual objects. JavaScript also supports functions without
            any special declarative requirements. Functions can be properties of
            objects, executing as loosely typed methods.
          </p>
          <p>
            JavaScript is a very free-form language compared to Java. You do not
            have to declare all variables, classes, and methods. You do not have
            to be concerned with whether methods are public, private, or
            protected, and you do not have to implement interfaces. Variables,
            parameters, and function return types are not explicitly typed.
          </p>
        </article>
      </section>
      <section class="main-section" id="Hello_world">
        <header>Hello world</header>
        <article>
          To get started with writing JavaScript, open the Scratchpad and write
          your first "Hello world" JavaScript code:
          <code
            >function greetMe(yourName) { alert("Hello " + yourName); }
            greetMe("World");
          </code>

          Select the code in the pad and hit Ctrl+R to watch it unfold in your
          browser!
        </article>
      </section>
      <section class="main-section" id="Variables">
        <header>Variables</header>
        <p>
          You use variables as symbolic names for values in your application.
          The names of variables, called identifiers, conform to certain rules.
        </p>
        <p>
          A JavaScript identifier must start with a letter, underscore (_), or
          dollar sign ($); subsequent characters can also be digits (0-9).
          Because JavaScript is case sensitive, letters include the characters
          "A" through "Z" (uppercase) and the characters "a" through "z"
          (lowercase).
        </p>
        <p>
          You can use ISO 8859-1 or Unicode letters such as å and ü in
          identifiers. You can also use the Unicode escape sequences as
          characters in identifiers. Some examples of legal names are
          Number_hits, temp99, and _name.
        </p>
      </section>
      <section class="main-section" id="Declaring_variables">
        <header>Declaring variables</header>
        <article>
          You can declare a variable in three ways:
          <p>
            With the keyword var. For example, <code>var x = 42.</code> This
            syntax can be used to declare both local and global variables.
          </p>
          <p>
            By simply assigning it a value. For example,
            <code>x = 42.</code> This always declares a global variable. It
            generates a strict JavaScript warning. You shouldn't use this
            variant.
          </p>
          <p>
            With the keyword let. For example,<code> let y = 13.</code> This
            syntax can be used to declare a block scope local variable. See
            Variable scope below.
          </p>
        </article>
      </section>
      <section class="main-section" id="Variable_scope">
        <header>Variable scope</header>
        <article>
          <p>
            When you declare a variable outside of any function, it is called a
            global variable, because it is available to any other code in the
            current document. When you declare a variable within a function, it
            is called a local variable, because it is available only within that
            function.
          </p>

          <p>
            JavaScript before ECMAScript 2015 does not have block statement
            scope; rather, a variable declared within a block is local to the
            function (or global scope) that the block resides within. For
            example the following code will log 5, because the scope of x is the
            function (or global context) within which x is declared, not the
            block, which in this case is an if statement.
          </p>
          <code>if (true) { var x = 5; } console.log(x); // 5</code>
          <p>
            This behavior changes, when using the let declaration introduced in
            ECMAScript 2015.
          </p>

          <code
            >if (true) { let y = 5; } console.log(y); // ReferenceError: y is
            not defined</code
          >
        </article>
      </section>
      <section class="main-section" id="Global_variables">
        <header>Global variables</header>
        <article>
          <p>
            Global variables are in fact properties of the global object. In web
            pages the global object is window, so you can set and access global
            variables using the window.variable syntax.
          </p>

          <p>
            Consequently, you can access global variables declared in one window
            or frame from another window or frame by specifying the window or
            frame name. For example, if a variable called phoneNumber is
            declared in a document, you can refer to this variable from an
            iframe as parent.phoneNumber.
          </p>
        </article>
      </section>
      <section class="main-section" id="Constants">
        <header>Constants</header>
        <article>
          <p>
            You can create a read-only, named constant with the const keyword.
            The syntax of a constant identifier is the same as for a variable
            identifier: it must start with a letter, underscore or dollar sign
            and can contain alphabetic, numeric, or underscore characters.
          </p>

          <code>const PI = 3.14;</code>
          <p>
            A constant cannot change value through assignment or be re-declared
            while the script is running. It has to be initialized to a value.
          </p>

          <p>
            The scope rules for constants are the same as those for let block
            scope variables. If the const keyword is omitted, the identifier is
            assumed to represent a variable.
          </p>

          <p>
            You cannot declare a constant with the same name as a function or
            variable in the same scope. For example:
          </p>

          <code
            >// THIS WILL CAUSE AN ERROR function f() {}; const f = 5; // THIS
            WILL CAUSE AN ERROR ALSO function f() { const g = 5; var g;
            //statements }</code
          >
          However, object attributes are not protected, so the following
          statement is executed without problems.
          <code
            >const MY_OBJECT = {"key": "value"}; MY_OBJECT.key =
            "otherValue";</code
          >
        </article>
      </section>
      <section class="main-section" id="Data_types">
        <header>Data types</header>
        <article>
          <p>The latest ECMAScript standard defines seven data types:</p>
          <ul>
            <li>
              <p>Six data types that are primitives:</p>
              <ul>
                <li>Boolean. true and false.</li>
                <li>
                  null. A special keyword denoting a null value. Because
                  JavaScript is case-sensitive, null is not the same as Null,
                  NULL, or any other variant.
                </li>
                <li>
                  undefined. A top-level property whose value is undefined.
                </li>
                <li>Number. 42 or 3.14159.</li>
                <li>String. "Howdy"</li>
                <li>
                  Symbol (new in ECMAScript 2015). A data type whose instances
                  are unique and immutable.
                </li>
              </ul>
            </li>

            <li>and Object</li>
          </ul>
          Although these data types are a relatively small amount, they enable
          you to perform useful functions with your applications. Objects and
          functions are the other fundamental elements in the language. You can
          think of objects as named containers for values, and functions as
          procedures that your application can perform.
        </article>
      </section>
      <section class="main-section" id="if...else_statement">
        <header>if...else statement</header>
        <article>
          Use the if statement to execute a statement if a logical condition is
          true. Use the optional else clause to execute a statement if the
          condition is false. An if statement looks as follows:

          <code>if (condition) { statement_1; } else { statement_2; }</code>
          condition can be any expression that evaluates to true or false. See
          Boolean for an explanation of what evaluates to true and false. If
          condition evaluates to true, statement_1 is executed; otherwise,
          statement_2 is executed. statement_1 and statement_2 can be any
          statement, including further nested if statements.
          <p>
            You may also compound the statements using else if to have multiple
            conditions tested in sequence, as follows:
          </p>
          <code
            >if (condition_1) { statement_1; } else if (condition_2) {
            statement_2; } else if (condition_n) { statement_n; } else {
            statement_last; }
          </code>
          In the case of multiple conditions only the first logical condition
          which evaluates to true will be executed. To execute multiple
          statements, group them within a block statement ({ ... }) . In
          general, it's good practice to always use block statements, especially
          when nesting if statements:

          <code
            >if (condition) { statement_1_runs_if_condition_is_true;
            statement_2_runs_if_condition_is_true; } else {
            statement_3_runs_if_condition_is_false;
            statement_4_runs_if_condition_is_false; }</code
          >
          It is advisable to not use simple assignments in a conditional
          expression, because the assignment can be confused with equality when
          glancing over the code. For example, do not use the following code:
          <code>if (x = y) { /* statements here */ }</code> If you need to use
          an assignment in a conditional expression, a common practice is to put
          additional parentheses around the assignment. For example:

          <code>if ((x = y)) { /* statements here */ }</code>
        </article>
      </section>
      <section class="main-section" id="while_statement">
        <header>while statement</header>
        <article>
          A while statement executes its statements as long as a specified
          condition evaluates to true. A while statement looks as follows:

          <code>while (condition) statement</code> If the condition becomes
          false, statement within the loop stops executing and control passes to
          the statement following the loop.

          <p>
            The condition test occurs before statement in the loop is executed.
            If the condition returns true, statement is executed and the
            condition is tested again. If the condition returns false, execution
            stops and control is passed to the statement following while.
          </p>

          <p>
            To execute multiple statements, use a block statement ({ ... }) to
            group those statements.
          </p>

          Example:

          <p>
            The following while loop iterates as long as n is less than three:
          </p>

          <code>var n = 0; var x = 0; while (n &lt; 3) { n++; x += n; }</code>
          <p>
            With each iteration, the loop increments n and adds that value to x.
            Therefore, x and n take on the following values:
          </p>

          <ul>
            <li>After the first pass: n = 1 and x = 1</li>
            <li>After the second pass: n = 2 and x = 3</li>
            <li>After the third pass: n = 3 and x = 6</li>
          </ul>
          <p>
            After completing the third pass, the condition n &lt; 3 is no longer
            true, so the loop terminates.
          </p>
        </article>
      </section>
      <section class="main-section" id="Function_declarations">
        <header>Function declarations</header>
        <article>
          A function definition (also called a function declaration, or function
          statement) consists of the function keyword, followed by:

          <ul>
            <li>The name of the function.</li>
            <li>
              A list of arguments to the function, enclosed in parentheses and
              separated by commas.
            </li>
            <li>
              The JavaScript statements that define the function, enclosed in
              curly brackets, { }.
            </li>
          </ul>
          <p>
            For example, the following code defines a simple function named
            square:
          </p>

          <code>function square(number) { return number * number; }</code>
          <p>
            The function square takes one argument, called number. The function
            consists of one statement that says to return the argument of the
            function (that is, number) multiplied by itself. The return
            statement specifies the value returned by the function.
          </p>
          <code>return number * number;</code>
          <p>
            Primitive parameters (such as a number) are passed to functions by
            value; the value is passed to the function, but if the function
            changes the value of the parameter, this change is not reflected
            globally or in the calling function.
          </p>
        </article>
      </section>
      <section class="main-section" id="Reference">
        <header>Reference</header>
        <article>
          <ul>
            <li>
              All the documentation in this page is taken from
              <a
                href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide"
                target="_blank"
                >MDN</a
              >
            </li>
          </ul>
        </article>
      </section>
    </main>
  </body>
</html>
```
```css
#styles.css
html,
body {
  min-width: 290px;
  color: #4d4e53;
  background-color: #ffffff;
  font-family: 'Open Sans', Arial, sans-serif;
  line-height: 1.5;
}

#navbar {
  position: fixed;
  min-width: 290px;
  top: 0px;
  left: 0px;
  width: 300px;
  height: 100%;
  border-right: solid;
  border-color: rgba(0, 22, 22, 0.4);
}

header {
  color: black;
  margin: 10px;
  text-align: center;
  font-size: 1.8em;
  font-weight: thin;
}

#main-doc header {
  text-align: left;
  margin: 0px;
}

#navbar ul {
  height: 88%;
  padding: 0;
  overflow-y: auto;
  overflow-x: hidden;
}

#navbar li {
  color: #4d4e53;
  border-top: 1px solid;
  list-style: none;
  position: relative;
  width: 100%;
}

#navbar a {
  display: block;
  padding: 10px 30px;
  color: #4d4e53;
  text-decoration: none;
  cursor: pointer;
}

#main-doc {
  position: absolute;
  margin-left: 310px;
  padding: 20px;
  margin-bottom: 110px;
}

section article {
  color: #4d4e53;
  margin: 15px;
  font-size: 0.96em;
}

section li {
  margin: 15px 0px 0px 20px;
}

code {
  display: block;
  text-align: left;
  white-space: pre-line;
  position: relative;
  word-break: normal;
  word-wrap: normal;
  line-height: 2;
  background-color: #f7f7f7;
  padding: 15px;
  margin: 10px;
  border-radius: 5px;
}

@media only screen and (max-width: 815px) {
  /* For mobile phones: */
  #navbar ul {
    border: 1px solid;
    height: 207px;
  }

  #navbar {
    background-color: white;
    position: absolute;
    top: 0;
    padding: 0;
    margin: 0;
    width: 100%;
    max-height: 275px;
    border: none;
    z-index: 1;
    border-bottom: 2px solid;
  }

  #main-doc {
    position: relative;
    margin-left: 0px;
    margin-top: 270px;
  }
}

@media only screen and (max-width: 400px) {
  #main-doc {
    margin-left: -10px;
  }

  code {
    margin-left: -20px;
    width: 100%;
    padding: 15px;
    padding-left: 10px;
    padding-right: 45px;
    min-width: 233px;
  }
}
```