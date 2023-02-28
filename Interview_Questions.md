# Interview Questions

Q: Why is multi-threading so popular in golang ?

A: Most of the programming languages create `kernel-level` threads, which incurs a large amount of overhead and may lead to expensive context switches.
Whereas in Go the threads are `user-level`. The Go runtime, which is built in Go and offers a lightweight scheduler that can effectively handle dozens or even millions of Go routines.

Also the fact that Go routines share an address space and heap makes the routines light weight because there is no need to duplicate
data between threads or processes in order for them to communicate and share information.

Because of the above reasons, writing concurrent code in Go is simple and doesn't need thinking about problems
like deadlocks, race situations, or memory synchronization. 

Q: Can you eloborate the difference between user-level and kernal-level threads ?

A: User-level threads and kernel-level threads are two different approaches to implementing threads in an operating system. 
Here is a detailed difference between the two:

**Management:** User-level threads are managed by the user-level thread library that is implemented in the application or programming language, while kernel-level threads are managed by the operating system kernel.

**Scheduling:** User-level threads are scheduled by the user-level thread library, which uses its own scheduling algorithm and decides which thread to run next. Kernel-level threads are scheduled by the operating system kernel, which uses its own scheduling algorithm and decides which process or thread to run next.

**Context Switching:** In user-level threads, context switching is done entirely in user space, which means that switching between threads does not involve a context switch to the kernel. This makes context switching faster and more efficient, but it also means that user-level threads cannot take advantage of kernel-level features like hardware interrupts, which can cause delays in I/O operations. In kernel-level threads, context switching involves a context switch to the kernel, which makes it slower and more expensive, but it allows kernel-level threads to take advantage of hardware interrupts and other kernel-level features.

**Resource Allocation:** User-level threads are allocated resources by the user-level thread library, which means that the library can allocate resources based on its own policies and priorities. Kernel-level threads are allocated resources by the operating system kernel, which means that resource allocation is based on the kernel's policies and priorities.

**Scalability:** User-level threads are generally more scalable than kernel-level threads because they can be implemented with a lightweight thread library that does not rely on the operating system kernel. This makes it possible to create and manage thousands or even millions of user-level threads in a single application. In contrast, kernel-level threads require more resources and overhead, which can limit scalability.

Q: What is the difference between both the lines ?

`var a int = 5`
`var a = 5`

A: In the first declaration, user has explicitly defined the variable types as intiger. Whereas in the second line, go compiler automatically determine the data type of a variable based on its initialization value. So, Go has the capability to infer the type of initialized variables.

However, it is still a good practice to declare the variable type explicitly, even if Go can infer it. Explicitly declaring the variable type can make the code more readable and can also help to prevent errors. For example, if you accidentally initialize a variable with a different data type than what you intended, the compiler will still infer the wrong type, and it may cause unexpected behavior or errors in the program.
