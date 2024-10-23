# MultiThreaded Web Server using Java

<b>This project demonstrates Java's multithreading capabilities!.</b>
<br>
High-performance, Multithreaded web server capable of handling up to 1 million concurrent requests.<br>
Built with Java, the server utilizes efficient thread management and thread pooling to ensure optimal resource utilization and minimal latency.

<br>
<h3> What is a Server? </h3> 
<br>
A Server serves static/dynamic content to users.

<hr>
If too many (example 10k) clients hit the server --> multiprocessing server will open 10k threads. 1 thread for each request
Thread block of 10 k threads will consume too much memory and Resources of the system that it may crash.

Making it impossible to serve 10k RPS. 

To solve this probem - a Thread Pool can be used.
It is a pool of Threads, ready to serve incoming requests.

Thread which is done with execution is reused again so no need to create more (> 100) threads.
Tasks wait in Queue till a thread is available to take up a task.
