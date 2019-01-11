# Availability Challenges

Let's try to * in your environment? Here you can find some stuff from chaos engineering to performance engineering, from sysadmins to developers.

Most of then will come with examples, sources and books or videos. With time, I'll make some examples of each of them and publish on this repository and link than to their topic.

Let's contribute :D!

---

## Index

* [Chaos Engineering](https://github.com/LozanoMatheus/the_availability_challanges#chaos-engineering)
* [Injecting Failures](https://github.com/LozanoMatheus/the_availability_challanges#injecting-failures)
* [Tuning](https://github.com/LozanoMatheus/the_availability_challanges#tuning)
* [Hardening](https://github.com/LozanoMatheus/the_availability_challanges#hardening)
* [Testing the Environment](https://github.com/LozanoMatheus/the_availability_challanges#testing-the-environment)

---

## Chaos Engineering

This section we will follow the [Principles of Chaos Engineering](http://principlesofchaos.org). Basically, we will try to destroy and find ways to affect the availability in your environment.

### Tools

Some tools that we can use/test.

* [Kube Monkey](https://github.com/asobti/kube-monkey) - Bring the Chaos to Kubernetes. Wrote in Go and easy to use or customize.
  * [Example of use](https://medium.com/@andrewsrobertamary/chaos-testing-date-with-kube-monkey-dbffd86a6202) - An use example 
* [Janitor Monkey](https://github.com/Netflix/SimianArmy/wiki/Janitor-Home) - Clean up the unused on AWS.
* [Chaos Monkey](https://github.com/Netflix/SimianArmy/wiki/Chaos-Monkey) - Bring the Chaos to AWS Instances. It will terminate, randomly, the instances on AWS.
* [Chaos Toolkit](https://github.com/chaostoolkit/chaostoolkit) - Bring the Chaos to everything that you want. Wrote in Python, easy to customize and already has a lot of extensions.
  * Example of some extensions [chaostoolkit-aws](https://github.com/chaostoolkit-incubator/chaostoolkit-aws) and [chaostoolkit-azure](https://github.com/chaostoolkit-incubator/chaostoolkit-azure).

### Practices

This section is about theoretical stuff. Like best practices, some examples, feedback from other companies, roadmaps, etc.

* [List of Chaos Engineering resources](https://github.com/dastergon/awesome-chaos-engineering)
* [Principles Of Chaos Engineering](http://principlesofchaos.org/)
* [Book - Chaos Engineering](https://learning.oreilly.com/library/view/chaos-engineering/9781491988459/)

### Groups and channels

* [Community on Slack](https://slofile.com/slack/chaosengineering)
* [Group on LinkedIn](https://www.linkedin.com/groups/7057761/)
* [Group on Google Groups](https://groups.google.com/group/chaos-community)

---

## Injecting Failures

### Tools

Here we will look to error handling and how your system behaves with it.

* [Istio](https://istio.io/docs/tasks/traffic-management/fault-injection/) - We can use Istio generate a lot of types of injection. Like networking delay, HTTP return, etc.
* [tc](https://linux.die.net/man/8/tc) - With it, we can create a lot of things related with Network. Like package loss, delay (many ways and you can combine than)
* [Limiting Resources (CPU, Mem, etc)](https://blogs.rdoproject.org/2015/08/hands-on-linux-sandbox-with-namespaces-and-cgroups/) - Who our systems will behave if we can reduce the resources to less than they have or defined?

### Practices

* [Fault Injection Techniques and Tools](http://www.archive.ece.cmu.edu/~ece749/docs/faultInjectionSurvey.pdf)
* [Failure Injection and Chaos Engineering](https://medium.com/production-ready/the-limitations-of-chaos-engineering-2a74816c0df3)
* [Lineage Driven Failure Injection (LDFI)](https://medium.com/becloudy/chaos-engineering-review-lineage-driven-failure-injection-ldfi-a1c831abe504)

---

## Tuning

Looking for a bottleneck in network, OS, Kernel, JVM, etc.

### Practices

#### Networking

* AQM Algorithms
  * [CoDel Overview](https://www.bufferbloat.net/projects/codel/wiki/)
    * [fq_codel](https://tools.ietf.org/html/rfc8290)
    * [The concept](https://lwn.net/Articles/616241/)
  * [A pice of Cake - A qdisc](https://www.bufferbloat.net/projects/codel/wiki/CakeTechnical/)
    * [Some important details](https://www.bufferbloat.net/projects/codel/wiki/Cake/)
* [Understanding more about Networking](https://github.com/leandromoreira/linux-network-performance-parameters)
* [Queueing in the linux network stack](https://www.coverfire.com/articles/queueing-in-the-linux-network-stack/)
* [AQM - Controlling Queue Delay](https://queue.acm.org/detail.cfm?id=2209336)

---

## Hardening

_TBD_

---

## Testing the Environment

### Practices

### Difference between Testing Types

What is the difference between {load,performance,stress} tests?

* [Differences and examples](https://www.softwaretestinghelp.com/what-is-performance-testing-load-testing-stress-testing/)
* [Load, Performance and Stress - The Difference](https://www.blazemeter.com/blog/performance-testing-vs-load-testing-vs-stress-testing)

### Performance Test

_TBD_

### Load Test

_TBD_

### Stress Test

_TBD_
