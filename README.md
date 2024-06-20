# Asynchronous programming Interview Questions

1. How can we write code not to block the event loop?
2. How to handle a blocked event loop to exit the blocking state from the same process?
3. What is a callback hell and how to avoid it?
4. What are async generators & iterators, how do they work and propose use cases?
5. How to handle errors in async code?
6. Where try/catch does not capture async errors and when it does?
7. Which async abstraction supporting flag `captureRejections` do we have and what for?8. How to avoid loss of steps in stack trace and how to improve debugging and understanding of control flow by stack traces using async/await?
9. How to abort async operations?
10. What is the difference between async contracts: callbacks, events, async/await, promises, etc.?
11. How async contracts (callbacks, events, async/await, promises) are related and is it possible to get rid of old ones?
12. What is the difference between `Promise.all()` and `Promise.allSettled()`?
13. What is the difference between `f2` and `f3` in the following expression: `promiseInstance.then(f1, f2).catch(f3)`?
14. When and why we may have multiple catch clauses: `promiseInstance.catch(f1).catch(f2).catch(f3)`?
15. Why do we have `Promise` method `finally`? Provide use cases.
16. How to write async code with sync generators? Propose advantages and disadvantages of this syntax and approach.
17. Provide examples of using `yield` in async programming and who to rewrite it in modern JavaScript?
18. Describe difference between Web workers, Shared workers, and Worker threads.
19. Describe the micro and macro tasks and how it is related to the event loop?
20. What are Worker threads in Node.js and what for we may use this technique?
21. How to measure I/O operations, performance, resource usage?
22. What do we have `process.hrtime` and `process.hrtime.bigint()`? What is the difference?
23. Tell us about following node.js API: `const { performance } = require('node:perf_hooks');`
24. How to efficiently handle asynchronous API requests at the client side that return large amounts of data?
25. How to efficiently handle API requests at the server side that return large amounts of data asynchronously?
26. How to ensure state isolation between different asynchronous requests in a single Node.js process?
27. What is CLS (continuation local storage) and do we have substitution of this async technique in modern node.js?
28. Which event loop phases are related to pending callbacks?
29. Tell us about `Thenable` contract and its relation to `Promise`.
30. How to associate some state (collection or data structure) with the chain of async calls?
31. How to track the chain of async calls from external requests (originated from api call via http, udp, ipc, ws)?
32. How to ensure safe processing of competing requests to a resource?
33. Why do we need locks api e.g. Web locks?
34. How can we use parallel programming primitives (semaphore, mutex, critical section and so on) in async programming?
35. Tell us about reactive programming paradigm?
36. What is the difference between streams and signals approach in reactive programming?
37. How to handle and avoid deadlocks in asynchronous code?
38. How to ensure high availability in asynchronous applications?
39. How to handle asynchronous operations that depend on each other? (parallel and sequential executions)
40. What is race condition and how to avoid it?
41. Provide use cases for `Promise.race`, `Promise.all`, `Promise.allSettled`.
42. What are «throttling» and «debouncing» in the context of asynchronous programming?
43. How to shape async calls (for example to limit request flow to API)?
44. What abstractions implementing pattern `Observable` do we have in JavaScript backend and frontend?
45. Describe `Signals` approach for reactive code?
46. Why are `Streams` useful as a higher level abstraction?
47. What is back pressure?
48. What is the difference in creating `Stream` with `extends` vs passing `read`, `write`, or `transform` function to revealing constructor?
49. Why do we have three sets of timers: in global context (for example `setTimeout`) , `node:timers`, and even `node:timers.promises`?
50. What promisified APIs do you know and how can we manually promisify other APIs?
51. Tell us about debugging and testing async code.
52. Why TypeScript can't describe async contracts in all aspects?
