# Introduction to GoLang

## Why Golang ?

Go was created to specifically answer the following objectives:

- Concurrency: Go has built-in concurrency support, which makes it easier to write concurrent and parallel programs. Other languages like Java has concurrency support as well, but it can be more complex and require more code to achieve the same results.

- Scalability: To satisfy the needs of contemporary distributed systems, Go was created to be able to manage big codebases and scale horizontally.

- Performance: Go was designed with performance in mind, This is partly due to Go's garbage collector, which is optimized for low-latency and high-throughput scenarios.

- Lightweight threads: goroutines and integrated concurrency mechanism make it simple to construct concurrent and parallel programmes.

- Efficiency: Go's garbage collector was designed to produce quick and efficient code in low-latency, high-throughput applications.

- Simple syntax: Go was created with an emphasis on readability and maintainability and a short, uniform language syntax to make it simple to learn and use.

- Cross-platform compatibility: Go was made to compile to a variety of platforms, making it simple to create programmes that work across several operating systems and architectures. 

- Deployment: Go produces a single binary file that is self contained. Which means this binary can be easily deployed to different platforms without dependencies. This makes it easier to distribute and deploy Go applications. 

## Self Contained Binaries

The Go compiler, which is a component of the Go installation, takes your source code and creates a binary executable file with all the required libraries and dependencies when you compile a Go program. The destination system does not need to have the Go installation or any other dependencies in order for this binary file to run because it is self-contained.

Because to this, it is simple to distribute and run Go applications across several platforms without worrying about the target system's Go version or any other requirements. 

## Better than Java ?

Golang is better than Java in few scenarios only. It is better to evaluate your use-case before choosing any option. 

The advantages of using golang is well described in the above section(Why Golang?). However, Java on the other hand is a very mature programming language in its own ways.

- Java has a strong type system, which can help catch errors at compile time.

- Strong enterprise frameworks

- Large community compared to Golang.

So, it is not completely correct to say Golang is better than Java or Java is better than Golang.

## Why DevOps Applications are written in Golang ?

It is a known fact that popular devops applications such as Kubernetes, Docker and many are written in Golang. But why ? 

As Go was created with concurrency in mind, writing concurrent and parallel programs is made simpler. Applications for DevOps, which frequently need to handle numerous containers or processes at once, should pay special attention to this. This is one of the primary reasons why Golang is a popular choice in DevOps community.
