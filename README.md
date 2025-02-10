# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js where a server hangs due to a long-running operation within a request handler.  The provided `server.js` file contains a simple HTTP server that simulates a 5-second delay.  During this delay, the server is unresponsive to new requests.

## Solution

The solution, found in `serverSolution.js`, utilizes asynchronous operations to prevent blocking the event loop.  Asynchronous operations allow the server to continue handling requests while the long-running task executes in the background.