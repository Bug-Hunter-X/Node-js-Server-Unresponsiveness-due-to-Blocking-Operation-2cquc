# Node.js Server Unresponsiveness

This repository demonstrates a common performance issue in Node.js applications: server unresponsiveness due to a long-running synchronous operation that blocks the event loop.

The `server.js` file contains a Node.js HTTP server with a request handler that simulates a long-running task. This task keeps the CPU busy for 5 seconds, blocking the event loop and preventing the server from responding to other requests during that time.

The `serverSolution.js` file provides a solution to this problem by using asynchronous operations or offloading the long-running task to a worker thread.