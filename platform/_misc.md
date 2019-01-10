# Misc

## Stack size
- Stack size for a single thread in .Net is ~ 1 MB
- The default stack size for a plain .NET application is 1 MB, 
  but you can change this in the PE header.
- If you're starting threads explicitly, you may also set a different    
  size via the constructor overload
- For ASP.NET applications the default stack size is only 256 KB.

https://blogs.msdn.microsoft.com/ericlippert/2009/04/27/the-stack-is-an-implementation-detail-part-one/
https://blogs.msdn.microsoft.com/ericlippert/2009/05/04/the-stack-is-an-implementation-detail-part-two/

## Value types and stack allocation
Value types are *sometimes* allocated on the stack. For example, the memory for an `int` field in a class type is part of the class instance's memory, which is allocated on the heap.
A local variable is hoisted to be implemented as a field of a hidden class if that local variable is an outer variable used by an anonymous method or in an iterator block; the storage associated with that local variable will be on the heap if it is of value type.

Windows typically provides 1 MB of stack memory per thread. This one-meg array could be an efficient place to store small amounts of short-lived data; however, it's not a requirement (of .NET CLI) that OS should provide it or that the JITter should use it. The jitter could choose to put every local "on the heap" and live with the performance cost of doing so, as long as the value type semantics were maintained.

Make the choice of value type vs reference type based on whether the type is semantically representing a value or semantically refering to something.

> Array of structs is layed out contiguosly in memory, which means that when performance is an issue an you can convert some of your objects to structs, ditch `List<T>` in favour of `Array.Resize` wrapped in a ref-parametered extension method (that hopefully would be inlined sometimes) and get your 10x speed increase for that part of the code thanks to the prefetch.

- Structs allow exact control of the memory layout.
- Structs allow bulk creation in a default, usable, well-defined state (as opposed to null).
- Structs can't be `null` ( `Nullable<T>` not withstanding). 
- Structs have a well-defined, non-referential, notion of equality.


## More:

https://blogs.msdn.microsoft.com/ericlippert/2012/01/16/what-is-the-defining-characteristic-of-a-local-variable/
https://blogs.msdn.microsoft.com/ericlippert/2011/11/28/why-have-a-stack/
https://blogs.msdn.microsoft.com/ericlippert/2010/10/11/debunking-another-myth-about-value-types/
https://blogs.msdn.microsoft.com/ericlippert/2010/09/30/the-truth-about-value-types/
https://blogs.msdn.microsoft.com/ericlippert/2010/01/21/whats-the-difference-between-a-destructor-and-a-finalizer/
https://blogs.msdn.microsoft.com/ericlippert/2009/02/17/references-are-not-addresses/


In Microsoft implementation of C# on the desktop CLR, 
_value types are stored on the stack_
when
  the value is
      a local variable 
    or
      a temporary 
such that
  the value is
    non-closed-over
     local variable
       belonging to 
           a lambda 
         or
           an anonymous method
       and 
         the method body is not an iterator block
       and 
         the jitter chooses not to en-register the value.








