# Asynchronous programming Interview Questions

1. How can we write code to avoid blocking the event loop?
2. How can we handle a blocked event loop to exit the blocking state from the same process?
3. What is callback hell, and how can we avoid it?
4. What are async generators and iterators, how do they work, and what are their use cases?
5. How do we handle errors in async code?
6. When does try/catch capture async errors and when does it not?
7. Which async abstraction supports the `captureRejections` flag, and what is it for?
8. How can we avoid losing steps in the stack trace and improve debugging and understanding of control flow using async/await?
9. How can we cancell async operations?
10. What is the difference between async contracts: callbacks, events, async/await, promises, etc.?
11. How are async contracts (callbacks, events, async/await, promises) related, and is it possible to eliminate older ones?
12. What is the difference between `Promise.all()` and `Promise.allSettled()`?
13. What is the difference between `f2` and `f3` in the following expression: `promiseInstance.then(f1, f2).catch(f3)`?
14. When and why might we have multiple catch clauses: `promiseInstance.catch(f1).catch(f2).catch(f3)`?
15. Why do we have `Promise` method `finally`, and what are its use cases?
16. How can we write async code with sync generators? What are the advantages and disadvantages of this approach?
17. Provide examples of using `yield` in async programming. How to rewrite it in modern JavaScript?
18. Describe the differences between Web Workers, Shared Workers, and Worker Threads.
19. Describe microtasks and macrotasks and their relation to the event loop.
20. What are Worker Threads in Node.js, and how might we use this technique?
21. How can we measure I/O operations performance and resource usage?
22. What are `process.hrtime` and `process.hrtime.bigint()`, and what is the difference?
23. Tell us about the following Node.js API: `const { performance } = require('node:perf_hooks');`
24. How can we efficiently handle asynchronous API requests at the client side that return large amounts of data?
25. How can we efficiently handle API requests at the server side that return large amounts of data asynchronously?
26. How can we ensure state isolation between different asynchronous requests in a single Node.js process?
27. What is CLS (continuation local storage), and do we have a modern substitution for this async technique in Node.js?
28. Which event loop phases are related to pending callbacks?
29. Tell us about `Thenable` contract and its relation to `Promise`.
30. How can we associate some state (collection or data structure) with the chain of async calls?
31. How can we track the chain of async calls from external requests (originating from API call via HTTP, UDP, IPC, WebSocket)?
32. How can we ensure safe processing of competing requests to a resource?
33. Why do we need locks API, such as Web Locks?
34. How can we use parallel programming primitives (semaphore, mutex, critical section, etc.) in async programming?
35. Tell us about «Reactive programming» paradigm.
36. What is the difference between streams and signals approaches in reactive programming?
37. How can we handle and avoid deadlocks in asynchronous code?
38. How can we ensure high availability in asynchronous applications?
39. How can we handle asynchronous operations that depend on each other (parallel and sequential executions)?
40. What is a race condition, and how can we avoid it?
41. Provide use cases for `Promise.race`, `Promise.all`, and `Promise.allSettled`.
42. What are throttling and debouncing in the context of asynchronous programming?
43. How can we shape async calls (e.g., to limit request flow to an API)?
44. What abstractions implementing the `Observable` pattern do we have in JavaScript for backend and frontend?
45. Describe the `Signals` approach for reactive code.
46. Why are `Streams` useful to improve code semantics as a high-level abstraction?
47. What is back pressure?
48. What is the difference between creating a `Stream` with `extends` vs. passing `read`, `write`, or `transform` function to a revealing constructor?
49. Why do we have three sets of timers: in the global context (e.g., `setTimeout`), `node:timers`, and `node:timers.promises`?
50. What promisified APIs do you know, and how can we manually promisify other APIs?
51. Tell us about testing of asyncronous code.
52. Why can't TypeScript describe async contracts in all aspects?53. How can we prevent memory leaks in async code?
54. What are the best practices for managing concurrency in JavaScript?
55. How can we use async/await with `EventEmitter`?
56. What is the difference between `EventEmitter` and `EventTarget`?
57. What is the role of the `await` keyword in async functions?
58. What happens if we use `await` with non-promise values (or expressions)?
59. How can we add timeouts in async operations (including `await` syntax)?
60. What are the implications of the `process.nextTick` method?
61. How can we create custom async iterables and what are their use cases?
62. What are the advantages and disadvantages of using third-party async libraries like `Promise` polyfills and `async.js`?
63. How can we handle async code in legacy systems?
64. What is the difference between asynchronous, parallel, and I/O operations?
65. How can we parallelize I/O operations effectively?
66. How can we ensure thread safety in async programming?
67. How are `Atomics` related to asynchronous and parallel programming? What are they used for?
68. How can we optimize async code for performance?
69. How can we handle retries (calls, calculations, resource access) in async programming?
70. What are the common pitfalls of async programming?
71. How can we use async functions with `Array.prototype.map`?
72. How can we debug async code effectively?
73. How can we ensure data consistency in async operations?
74. What are the benefits of using `async/await` over callbacks?
75. Which operations can't be rewritten from callbacks to `async/await` syntax (but are possible with `Promises`)?
76. Propose use cases for `AbortSignal.timeout()`. Which well-known APIs support it?
77. Where and for what purposes can we use `AbortSignal.any(iterable)`?
78. What are the differences between `Promise` methods: `resolve` and `reject`?
79. How can we handle errors in `Promise.all`?
80. How can we chain async operations? (Please propose cases for as many contracts as you know)
81. What is the role of the event loop in async programming?
82. How can we handle long-running async operations? (Processes may exit, results may become obsolete, etc.)
83. How can we ensure idempotency in async operations and when do we need it?
84. Can we write a real-time application in JavaScript and asynchronous programming?
85. How can we ensure the order of async operations? Please suggest cases in which we might experience problems.
86. How can we handle async code in a high-availability system?
87. What are observables and how can we use them in JavaScript?
88. What are the main problems of handling state in asynchronous code in a stateful application?
89. When can we use internal async queues and when do we need external queue systems?
90. How can we use async functions with caching, memoization, and recalculations on state updates?
91. How can we use async functions with database connections and what are the use cases?
92. How can we separate async code from business logic and why might we want to do this?
93. What is the impact of async code on CPU-bound vs I/O-bound operations?
94. What are the security considerations in async programming?
95. How can we implement a priority queue for async tasks?
96. How can we use async functions with file system operations?
97. How can we ensure atomicity in async operations and what for?
98. What are the trade-offs between using `Promise` and `async/await`?
99. What is the difference between simple async programming and the RxJS approach?
100. What are async collections and how can they improve developer experience?
