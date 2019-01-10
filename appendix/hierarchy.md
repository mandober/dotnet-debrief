# Hierarchy

* Tokens and symbols
  * Identifiers
    - Keywords
      - Reserved keywords
      - Contextual keywords
    - Names (identifiers as names)
      - name, `[_a-zA-Z][a-zA-Z_0-9]*`
      - keyword as name, `@keyword`
      - unicode identifier, `char \u0065 = 'e'`
  * Punctuation characters
    - block: braces
    - label: identifier followed by a colon, `label:`
  * Special characters
    - Verbatim identifier character, `@`
    - Interpolated string character, `$`
  * Comments
    - Syntax comments
      - single-line, `//`
      - multiline comments, `/* ... */`
    - Doc comments (also IDE tooltips)
      - single-line, `///`
      - multiline comments, `/** ... */`
  * Attributes, `[Test]`
  * Preprocessor directives, `#endregion`
  * Operators
  * Literals
    - Numeric
    - Char
    - String
  * Variables
    - global (static) variables
    - local variables
    - arguments
    - parameters
      - value parameter
      - reference parameter, `ref`
      - output parameter, `out`
      - variable (arity) parameter, `params`
  * Constants, `const int c = 3`
  * Flow
    - Loops
      - for
      - while
      - do...while
    - Conditionals
      - Null-conditional
  * Expressions
    - expression-bodied block, `... => expr;`
  * Statements
    - code block
    - labelled code block
    - statement block, `{}`
  * Values
    - value types, `int num = 42`
      - Boxing scalars, `var boxed = (object) num`
      - Unboxing scalars, `var num = (int) boxed`
    - reference types, `List<int> list = new List<int> { 1, 2, 3}`
      - pointer types (only in unsafe mode), `int* ip = &num`



* Class properties
  - class modifiers
  - class identifier (class name)

* Class memebers
  - attributes
  - fields
    - instance fields
    - static fields

* Methods
  - Main method
  - properties (getter/setters)
  - static methods
  - constructors
  - deconstructor (DCONS), `Deconstruct`
  - destructor (DTOR)
  - indexers
* Generics
  - generic type parameter
  - generic constraints


* Items
  - types
  - namespace, `namespace nsName`
  - using directive:
    - `using nsName`
    - `using ns = nsName`
    - `using static nsWithStaticClass`


  events
  indexers
  finalizers
  static

- types
- input type
- output/return type
- class
- namespace
- assembly
- events
- indexers
- finalizers


Language
- Environment
- Program Structure
- Basic Syntax
- Data Types
- Type Conversion
- Variables
- Constants
- Operators
- Decision Making
- Loops
- Encapsulation
- Methods
- Nullables
- Arrays
- Strings
- Structure
- Enums
- Classes
- Inheritance
- Polymorphism
- Operator Overloading
- Interfaces
- Namespaces
- Preprocessor Directives
- Regular Expressions
- Exception Handling
- File I/O
- Attributes
- Reflection
- Properties
- Indexers
- Delegates
- Events
- Collections
- Generics
- Anonymous Methods
- Unsafe Codes
- Multithreading


Anonymous Methods
Arrays
Attributes
Basic Syntax
Classes
Collections
Constants and Literals
Data Types
Decision Making
Delegates
Encapsulation
Enums
Environment
Events
Exception Handling
File I/O
Generics
Indexers
Inheritance
Interfaces
Loops
Methods
Multithreading
Namespaces
Nullables
Operator Overloading
Operators
Overview
Polymorphism
Preprocessor Directives
Program Structure
Properties
Reflection
Regular Expressions
Strings
Structures
Type Conversion
Unsafe Codes
Variables
