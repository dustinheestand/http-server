# HTTP Server

I built the [HTTP server in Rust from The Book](https://doc.rust-lang.org/book/ch20-00-final-project-a-web-server.html). But of course it's one thing to build along with a tutorial, and another thing entirely to build from scratch. Since I've got only a fuzzy memory of the steps I undertook, I'm going to try to redo the project from first principles, using as my guide the first nineteen chapters as the book as well as general research on HTTP servers.

This readme is going to serve as my place for notes on the process.

## Threads

I'm primarily a JS developer, so threads are a new concept for me. In JS, we've got the event loop, which executes all synchronous code, then checks to see if the results of any asynchronous operations are available for processing and deals with those. It's a big part of the magic of Node and a reason to build your backend in Node rather than, say, Python.

### The Event Loop: Drawbacks

I can't speak to this yet.

### The Approach

Since Rust is a systems language, I'm sure I could implement an event loop in it. And perhaps that's my next project. But for now, I'll use Rust's threading capabilities to implement a thread pool.
