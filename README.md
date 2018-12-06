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
As a website's traffic increases, so does the load on server equipment. This can lead to long response times, instability and even complete service shutdowns, making it impossible to ensure a good experience for all of your users. By separating the hosting of your business logic and Relational Database, you can optimize workloads with a combination of vertical and horizontal scaling. This lets you deliver a stable, responsive experience to your users, at a lower cost than simply throwing money at your hosting provider.

- How to scale and load balance?


Example topics
- How does vertical up/down scaling affect the project response times
- Horizontal scaling and better latencies thanks to proximity
  - Simmulate load
- IDs determined berforehand, artificial issue
