SCALING

What, How, When, Why
---

One of the nicest problems that you could ever have is that you have a
service that is just so popular, that it struggles to handle serving all
of your users. It is certainly a much better problem to have than not
having any users at all! We intend to demonstrate the effects of high load
and scaling by using a project that we have made as part of the LSD-Course,
but we want to emphasize the fact that the problems and methods for finding
solutions are totally universal and apply to pretty much any project.

While the load put on the service we made for the LSD project is nowhere
near enough for it to break a sweat, we will simulate a higher load on a
weaker instance to demonstrate the issues and how they can be solved. 
Now obviously, the simplest and safest way to make a service faster is
to just scale vertically... right? Just put some more RAM in there and
all problems just go away, right? Not so fast. We'll get to that.

Steps needed to scale:
1. Measure and identify bottlenecks
2. Identify components that can be split up and made independent
3. Load balance

So first we replicated the entire setup on a small droplet.
These are the components of the service:

- main java server software
- mysql
- python server for misc perf charts

On our LSD project, all of these run on the same droplet.
