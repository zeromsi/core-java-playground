# core-java-playground

# Language Fundamentals
## Topics 
- Identifiers
- Reserved words
- Data types
- Literals
- Arrays
- Types and variables
- var-arg methods 
- main method
- Command line args
- Java coding standards


### Identifiers:
 A Name is concerned as identifier in java program. It can be a name of a class, method , variable or label name.
 ``` Note: ``` Predefined class name like ```String``` are also identifier. 
 For example,
 ```xml
String x=10;
```
Here theres's two identifiers, ```String``` and ```x```.


Roles for defining Java identifier,

1. Only allowed characters in java identifiers are,
- A-Z
- a-z
- 0-9
- _
-$
If we use any other chars, we'll get compile time ```error```

2. Identifiers can not start with digit

```total123``` is valid but ```123Total``` is not valid.

3. Java identifiers are case sensative as java is a case sensative programming language.

4. There's no length limit for java identifiers

5. We can't use reserved words as identifiers.
For example,

``` int if=12;``` is not valid as ```if ``` is a reserved word. It'll through compile time error.
6. Predefined class name and interface name can be use as identifiers but it is not recommended.

For example,

``` int Runnable=5;```
It's not gonna through any error or exception.
 

### Reserved words

In java theres only ```53``` reserved words. Reserved words are there to represent meaning of functionality.

From these ```53``` there's ```50``` ```keywords``` and ```3``` ```Literals```.  

What is a ```Keyword```?
If the ```reserved``` words represents any functionality, then it's a ```keyword```.
From these ```50``` ```keywords``` ```48``` are ```used keyword```.
List of ```unused keyword```
- goto
- const

List of ```used keywords```
- abstract	
- assert	
- boolean
- break
- byte
- case
- catch
- char
- class
- continue
- default
- do	
- double
- else
- enum
- extends
- final
- finally
- float
- for
- if
- implements
- import
- instanceof
- int
- interface
- long
- native
- new
- package
- private
- protected
- public
- return
- short
- static
- strictfp
- super
- switch
- synchronized
- this
- throw
- throws
- transient
- try
- void
- volatile
- while

What is a ```literal```?
If the ```reserved``` words represents any value, then it's a ```literal```
List of ```reserved literals```
- true
- false
- null

### Data types
Theres 8 data type,
- byte
- short
- int
- long
- float
- double
- boolean
- char

### Flow control keywords
There's 11 flow control keywords.
- if
- else
- switch
- case 
- default
- do
- while
- for
- break
- continue
- return 

### modifiers keywords
There's 11 modifiers in java , including ```default``` , the number is 12.
- public
- private
- default
- protected
- static
- final
- abstract
- synchronized
- native
- strictfp
- transient
- volatile


### Exception handling keywords
There's 6 exception handling keywords,

- try
- catch
- throw
- throws
- finnaly
- assert

### Class related keywords
There's 6 Class related keywords,

- class
- interface
- extends
- implements
- package
- import

### Object related keywords
There's 4 Object related keywords,

- new
- instanceof
- super
- this

### Return type keyword
There's 4 Return type keywords,

- void

### enum keywords
There's 4 enum type keywords,
-enum

### Data types
Java languange is strongly typed language. Every variable and expression must have some type.

Java is not a pure oo language as, 
- there are primitive data types (8), int, double, long, byte, short, float,double,boolean, char.
- java doesn't support operator overloading.
- there is no support of multiple inheritance.

Peimitive data type's are divided into 2 parts, numeric and non-numeric. 

Non-numeric primitive data types,
- char ( size: 2 bytes as it is unicode basis (2 bytes, 0 to 65536 options, java supports all language chars ), in c or c++ it is 1 byte as they are ascii char based (1 byte, 0 to 256 options) only) 
- boolean (size n/a as it depends on VM; Java boolean throughs compile time error for 0 and 1, it can only hold true or false)

numeric data types are divided into further 2 sections,integral and floating point.

Integral data types,
- byte (singed; positive and negative, 1 byte (8 bits), range: -128 to 127)
- short ( signed; 2 bytes(16 bits), range: - 32768 to 32767)
- int (signed; 4 bytes(32 bits), range: -2,147,483,648 to 2,147,483, 647)
- long (signed; 8 bytes(64 bits), range: 	-9,223,372,036,854,775,808 to 9,223,372,036,854,775,807)

Floating point data types,
- double ( 8 bytes (64 bits), range: ±1.79769313486231570E+308 , we want 14-15 decimal places,double precicion) 
- float ( 4 bytes (32 bits), range:,-1.7X10^38 to 1.7X10^38, we want 5-6 decimal places, single precicion)

```Note```:  ```null``` is only applicable for object type. It is the default value of object reference. we can't use it for primitives.



### Java literals

Literal is a constant assigned to the variable. 

```
int a= 10;
```
Here,

``` int ``` -----> Data type
``` a ```  -----> identifier/variable
``` = ``` -----> operator
``` 10 ``` -----> constant (Literal)
``` ; ``` -----> Specific symbol/ terminator

Java provided the following literals,

#### Integral/ Integer literals
 byte, short, int, long --> 10,20
 char --> 'a','b'

#### Floating point literals
 float --> 22.12f, 23.34f
 double --> 2324.234,23434.3435D

#### Boolean Literal
 boolean --> true, false

#### String literal
String --> "abc", "10","true"

To improve readability in Literals, java 7 supports a special notation '_' 

For example, 

```
double d=123456789.234;
```
You can write the above double declaration like following,

```
double d=12_34_56_789.334;  (12 core, 34 lakh,56 thousand, 789.234)
```

### Types of variables

There's 2 ways, we can classify java variables,

#### Based on types of value represented by variable, there are 2 types of variable in java.
 - Primitive variables
   For example, ``` int x=10; ```, here ```x``` is a primitive variable as the types of variable is primitive.

- Reference variables
  For example, ``` Customer customer=new Customer();```, here ```customer``` is a reference variable as it is the reference of ```Customer``` class.

#### Based on position of declaration and behaviour, there are 3 types of variables in java.
- Instance variables
    - Instance variables are declared in a class, but outside a method, constructor or any block.

    - When a space is allocated for an object in the heap, a slot for each instance variable value is created.

    - ``` Instance variables are created when an object is created ``` with the use of the keyword 'new' and destroyed when the object is destroyed.

    - Instance variables hold values that must be referenced by more than one method, constructor or block, or essential parts of an object's state that must be present throughout the class.

    - Instance variables can be declared in class level before or after use.

    - ``` Access modifiers``` can be given for instance variables.

    - The instance variables are visible for all methods, constructors and block in the class. Normally, it is recommended to make these variables private (access level). However, visibility for subclasses can be given for these variables with the use of access modifiers.

    - Instance variables have ``` default values```. For ```numbers ```, the default value is ```0```, for ```Booleans``` it is ```false```, and for ```object references``` it is ```null```. Values can be assigned during the declaration or within the constructor.

    - Instance variables can be accessed directly by calling the variable name inside the class. However, within static methods (when instance variables are given accessibility), they should be called using the fully qualified name. ObjectReference.VariableName.
   
    ```xml
    import java.io.*;
    public class Employee {

       // this instance variable is visible for any child class.
       public String name;

       // salary  variable is visible in Employee class only.
       private double salary;

       // The name variable is assigned in the constructor.
       public Employee (String empName) {
         name = empName;
       }

       // The salary variable is assigned a value.
       public void setSalary(double empSal) {
         salary = empSal;
       }

       // This method prints the employee details.
       public void printEmp() {
         System.out.println("name  : " + name );
         System.out.println("salary :" + salary);
       }

      public static void main(String args[]) {
        Employee empOne = new Employee("Ransika");
        empOne.setSalary(1000);
        empOne.printEmp();
      }
    }
    ```


- Local variables
    - Local variables are declared in methods, constructors, or blocks.

    - Local variables are created when the method, constructor or block is entered and the variable will be destroyed once it exits the method, constructor, or block.

    - ``` Access modifiers ``` cannot be used for local variables.

    - Local variables are visible only within the declared method, constructor, or block.

    - Local variables are implemented at stack level internally.

    - There is ```no default``` value for local variables, so local variables should be ``` declared and an initial``` value should be assigned before the first use.

    ```
        public class Test {
           public void pupAge() {
             int age = 0;
             age = age + 7;
             System.out.println("Puppy age is : " + age);
          }

        public static void main(String args[]) {
           Test test = new Test();
           test.pupAge();
          }
        }
```

- Class/Static variables


