<!-- QuESTION 1 -->
The event loop is a programming construct that allows a program to efficiently handle asynchronous events. It is used in event-driven programming, where the program waits for events such as user input or messages from other programs, and then responds to them.

<!-- QUESTION 2 -->
The six phases of the event loop includes;
a) Timer phase: It is the first phase of the event loop where it checks if any registered timers have expired. Executes callbacks using timers. If there are timers set to 0 ms or setImmediate(), they will run here. Incomplete timers will run in later iterations of the loop.
b) I/O callbacks phase: In this phase, the event loop checks for any I/O events that have completed, for example, a file being read from disk. If any I/O events have completed, their associated callback functions are added to the event queue.
c) Idle/prepare phase: This phase is used to prepare the event loop for the next iteration. For example, it may update internal state or perform other setup tasks.
d) Poll phase: In this phase, the event loop waits for new events to arrive. This is where the event loop blocks until a new event is detected and processes any I/O callbacks that has been completed
e) Check phase: Once a new event has been detected, the event loop checks the event queue for any pending callbacks that need to be executed immediately. It executes any setImmediate() timers added in the Poll phase
f) Close callbacks phase: The final phase of the event loop is used to handle any 'close' events, such as closing a file handle. Any associated callbacks are executed in this phase. Loop continues if there are more timers or I/O calls. If all timers and I/O calls are done, the loop closes and the process ends.

<!-- QUESTION 3 -->
a) Keep code small
b) Document your code
c) Focus on code quality
d) Handle errors
e) Prefer ES6+ and Async/Await
f) Secure your code

<!-- QUESTION 4 -->
NPM means Node Package Manager. It is a package manager for JavaScript. It is used to install and manage third-party packages, modules, and libraries for use in Node.js projects. It manages project dependencies via command line and a website hosting more than 1 million third-party packages.

<!-- QUESTION 5 -->
To initialize a package in npm, use the "npm init" command in a terminal or command prompt. "npm init -y" command is used to accept all the default values.

<!-- QUESTION 6 -->
To run a script in the package.json file, use the "npm run" command followed by the script name. For example, if the script name is "prettier" in the package.json file, run it with the command "npm run prettier".
