# UFO-blog-entry-Lasse-Kristjan
Blog entry for Lasse and Kristjan

### More bang for the buck
```
Every piece in the software stack has knobs that can be tweaked and
configured for optimal performance, but it can be hard to make informed
decisions on what to change and why. What level of swappiness is reasonable
in your kernel config? What are reasonable cache sizes? What GC should you
use for Java and what is a fitting heap size? If you answer "I have no idea"
to these questions you better read this document.
Misconfiguring can have dire consequences and there is no guarantee that the
defaults are optimal, so it is important to know how to tune things properly.
This document explores which settings matter the most and why.
```
### Scaling (Hypothetical)
As a website's traffic increases, so does the load on server equipment.
```
Each connection requires some additional bookkeeping which means more
resource contention and overhead. It seems only reasonable to expect
there to be natural limits to how far fixed hardware can be pushed.
```
This can lead to long response times, instability and even complete service shutdowns, making it impossible to ensure a good experience for all of your users.
```
It goes without saying that just throwing more money at something is
not a silver bullet. Horizontal scaling doesn't implement itself,
and the concept of diminishing returns should also be taken into
account.
```
By separating the hosting of your business logic and Relational Database, you can optimize workloads with a combination of vertical and horizontal scaling.
```
Scaling an application means allocating resources to match its needs. There is no one-size-fits-all solution: For example,
most Relational Database Systems (MySQL, MS SQL Server, PostgreSQL) are designed to be monolithic and scale vertically, 
while newer paradigms like Distributed Databases are designed to make effective use of horizontal scaling. 
```
This lets you deliver a stable, responsive experience to your users, at a lower cost than simply throwing money at your hosting provider.
```
Scaling up can be an expensive investment, and choosing the right method of scaling for each technology is essential to achieving the greatest possible return on that investment. A powerful machine running under no load equals wasted money, but so do multiple load-balancing nodes if they're not pulling their weight.
```

- How to scale and load balance?


Example topics
- How does vertical up/down scaling affect the project response times
- Horizontal scaling and better latencies thanks to proximity
  - Simmulate load
- IDs determined berforehand, artificial issue
