### 1. What is C#? Write its features?
`C# is an object-oriented programming language that was developed by Microsoft in 2000. It is supported by different operating systems. C# is the primary language that is used to create .Net software applications. It allows us to create Windows UI apps, backend services, controls, libraries, android apps, and even blockchain applications. C# works on the concept of classes and objects just like Java.`
**Some of the C# features are as follows:**

- Follows structured approach
- Parameters passing is easy
- Code can be compiled on a different platform
- Open-source
- Object-oriented
- Flexible and scalable 

### 2. Explain what are classes and objects in C#?

` C# is an object-oriented language and classes are its foundation. A class generally depicts the structure of data, how data is stored and managed within a program. A class has its own properties, methods, and other objects that define the class.`

`Objects are the real-world entity having some characteristics and is created using the class instance. These classes define the type of the defined object.`

`For example, if we consider a program that covers the object related to the book. We call the class a Book which has two properties: name and the author. In real programming, Vedas is an object and an instance of the class Book.`



### 3. What difference between Convert.toString and .toString() method?

`Here both the methods are used to convert the string but the basic difference between them is: "Convert" function handles NULLS, while "i.ToString()" does not it will throw a NULL reference exception error. So as good coding practice using "convert" is always safe.`

### 4. Describe the different C# classes in detail?

**here are 4 types of classes that we can use in C#:**

- **Static Class:** It is the type of class that cannot be instantiated, in other words, we cannot create an object of that class using the new keyword and the class members can be called directly using their class name.
- **Abstract Class:** Abstract classes are declared using the abstract keyword. Objects cannot be created for abstract classes. If you want to use it then it must be inherited in a subclass. You can easily define abstract or non-abstract methods within an Abstract class. The methods inside the abstract class can either have an implementation or no implementation.
- **Partial Class:** It is a type of class that allows dividing their properties, methods, and events into multiple source files, and at compile time these files are combined into a single class.
- **Sealed Class:**  One cannot inherit a sealed class from another class and restricts the class properties. Any access modifiers cannot be applied to the sealed class.

### 5. Explain different access modifiers in C#?

`These are the keywords that help to define the accessibility of class, member, and data type in the program. These keywords are used to restrict the use of some data manipulation done by other classes. There are 4 types of access modifiers- public, private, protected, and internal. These modifiers define 6 other accessibility levels when working together- public, protected, internal, protected internal, private, and private protected.`

### 6. How can you describe object-oriented concepts in detail?

`C# is an object-oriented programming language that supports 4 OOP concepts.`

- **Encapsulation:** defines the binding together code and the data and keeps it safe from any manipulation done by other programs and classes. It is a container that prevents code and data from being accessed by another program that is defined outside the container.
- **Abstraction:** this concept of object-oriented protects everything other than the relevant data about any created object in order to increase efficiency and security within the program.
- **Inheritance:** Inheritance is applied in such a way where one object uses the properties of another object. 
- **Polymorphism:** is a feature that allows one interface to act as a base class for other classes. This concept is often expressed as a "single interface but multiple actions". 

### 7.  Explain how code gets compiled in C#?

**It takes 4 steps to get a code to get compiled in C#. Below are the steps:**
- First, compile the source code in the managed code compatible with the C# compiler.
- Second, combine the above newly created code into assemblies.
- Third, load the CLR.
- Last, execute the assembly by CLR to generate the output.

### 8. What is break and continue statements in C#, explain?
**Below are the differences:**
<table>
<tbody>
<tr>
<td><strong>Break</strong></td>
<td><strong>Continue</strong></td>
</tr>
<tr>
<td>You can use break statements in both switch and loop (for, while, and do-while ) statements.</td>
<td>You can use continue statements only in the loop (for, while, do) statements.</td>
</tr>
<tr>
<td>The switch or loop statements terminate at the moment the break statement is executed and it ends abruptly from there.</td>
<td>You cannot make a continue statement terminate the loop, it carries on the loop to go to the next iteration level without executing the immediate next step.</td>
</tr>
<tr>
<td>The loop or switch exits immediately from the inner loop when the compiler encounters a break statement and comes out of the inner loop.</td>
<td>A continue that is placed inside a nested loop within a switch causes the next loop iteration.</td>
</tr>
</tbody>
</table>

### 9. What is the difference between public, static, and void?

`Public declared variables or methods are accessible anywhere in the application. Static declared variables or methods are globally accessible without creating an instance of the class. Static member are by default not globally accessible it depends upon the type of access modified used. The compiler stores the address of the method as the entry point and uses this information to begin execution before any objects are created. And Void is a type modifier that states that the method or variable does not return any value.`

### 10. How you can explain the use of ‘using’ statements in C# in detail?\

`The using statement is used to control the usage of one or more resources that are being used within the program. The resources are continuously consumed and released. The main function of this statement is to manage unused resources and release them automatically. Once the object is created which is using the resource and when you are done you make sure that the object’s dispose method is called to release the resources used by that object, this is where using statements works well.`

**For example:**
<pre style="background: #c5c5c5;">
using (MyResource abc = new MyResource())
{
 abc.program();
}
Gets translated to,
MyResource abc= new MyResource();
try
{
 myRes.program();
}
finally
{
 // Check for a null resource.
 if (abc!= null)
     // Call the object's Dispose method.
     ((IDisposable)abc).Dispose();
}
</pre>

### 11. Describe the C# dispose of the method in detail?

`The disposeof() method releases the unused resources by an object of the class. The unused resources like files, data connections, etc. This method is declared in the interface called IDisposable which is implemented by the class by defining the interface IDisposable body. Dispose method is not called automatically, the programmer has to implement it manually for the efficient usage of the resources.`

### 12. Explain in detail the finalize method in C#?

`The finalize () method is defined in the object class which is used for cleanup activities. This method is generally called by the garbage collector whenever the reference of any object is not used for a long time. Garbage collector frees that managed resources automatically but if you want to free the unused resources like filehandle, data connection, etc., then you have to implement the finalize method manually.`

### 13. How you can define the exception handling in C#?

`An exception is a raised problem that may occur during the execution of the program. Handling exceptions offers a simple way to pass the control within the program whenever an exception is raised. C# exceptions are handled by using 4 keywords and those are try, catch, finally, throw.`

**try:** `a raised exception finds a particular block of code to get handled. There is no limit on the number of catch blocks that you will use in your program to handle different types of exception raised.`

**catch:** `you can handle the raised exception within this catch block. You can mention the steps that you want to do to solve the error or you can ignore the error by suppressing it by the code.`

**Finally:** `irrespective of the error, if you still want some set of instructions to get displayed then you can use those statements within the finally block and it will display it on the screen.`

**throw:** `you can throw an exception using the throw statement. It will display the type of error you are getting.`

**Syntax :**

<pre>
try {
//exception handling starts with try block
} catch( ExceptionName ea1 ) {
   // errors are handled within the catch block
} catch( ExceptionName e2 ) {
   // more catch block
} catch( ExceptionName eN ) {
   // more catch block to handle multiple exception raised
} finally {
   // last block of the exception handling
} 
</pre>

### 14. Explain the concept of Destructor in detail. Explain it with an example?

`A destructor is a member that works just the opposite of the constructor. Unlike constructors, destructors mainly delete the object. The destructor name must match exactly with the class name just like a constructor. A destructor block always starts with the tilde (~) symbol.`

**Syntax : **
<pre>
~class_name()
{
//code
}
</pre>

**A destructor is called automatically:**

- when the program finishes its execution.
- Whenever a scope of the program ends that defines a local variable.
- Whenever you call the delete operator from your program.

### 15. Define method overloading with example?
`Method overloading allows programmers to use multiple methods but with the same name. Every defined method within a program can be differentiated on the basis of the number and the type of method arguments. It is a concept based on polymorphism.`

**Method overloading can be achieved by the following:**

- By changing the number of parameters in the given method
- By changing the order of parameters passed to a method
- By using different data types as the passed parameters

**For example:**
<pre>
public class Methodoveloading    
  {    
    public int sum(int a, int b)  //two int type Parameters method  
    {    
        return a + b;    
            }    
    public int sum(int a, int b,int c)  //three int type Parameters with same method same as above  
    {   
        return a + b+c;    
    }    
    public float sum(float a, float b,float c,float d)  //four float type Parameters with same method same as above two method 
    {    
        return a + b+c+d;    
    
    }    
  }   
</pre>

### 16. Explain the concept of boxing and unboxing of the value type and object type in C#?

**Boxing-** `is a process of converting a value type to an object type where value type is placed on the stack memory, and the object type is placed in the heap memory. This conversion is an implicit conversion and you can directly assign any value to an object, and C# will handle the rest of the conversion on its own.`

**Example :**

<pre>public void function()
{
Int a=111;
Object b=a; //implicit conversion
Console.WriteLine(b);
}</pre>

**Unboxing-** `it is the reverse process of the boxing process. It is a conversion of the object type to the value type and the value of the boxed object type placed on the heap memory which will be transferred to the value type which is placed on the stack. This conversion of the unboxing process has to be done explicitly.`

**Example :**

<pre>
public void function()
{
Object b=111;
Int a=(int)b; //implicit conversion
Console.WriteLine(a);
}
</pre>