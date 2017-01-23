## Summary
Experience building web applications and distributed systems with pretty much everything. Former AWS developer where I built and maintained large web services using Java, Clojure, Python, blood and sweat. Early technical member of a high growth startup where I learned some lessons on building teams and products. 

## Experience

#### STRIPE, SAN FRANCISCO, CA

##### Senior Software Engineer, March 2020 - Present
Initially I worked on Stripe's internal function-as-a-service platform, helping improve reliability and enforcing security invariants for over 1000+ internal applications that are collectively responsible for moving $3B/day in transaction volume. In 2021, I was recruited into the Security Infrastructure organization to bootstrap an org-wide effort to develop robust fine-grained access controls. 

##### Achievements
* Built a system to detect anomalous output from Stripe’s online feature compute platform. This alerted teams to erroneous outputs, protecting Stripe’s underwriting against poorly performing features or bad data.
* Led a project to migrate Stripe's internal event bus platform to Kubernetes while handling 100k+ rps with low delivery latency.
* Proactively identified a workload bottleneck and optimized Stripe's compute platform to save 10M+/year.
* Prototyped infrastructure for fault-tolerant workflow execution (using Temporal), the platform became widely adopted by critical teams at Stripe and a team was funded to run it.
* Core contributor to a large, cross-company project to enforce context-aware access controls using cryptographic identities. 
* Authored an internal proposal for deferred authorization using asymmetric encryption. This allows Stripe to use our existing context-aware access controls and policy semantics for authorizing queries that span across our infrastructure.
* Submitted patent application for a novel fault-tolerant bitmap encoding used to represent Stripe’s permissioning scheme in transit.

#### UBER, SAN FRANCISCO, CA

##### Senior Software Engineer, November 2017 - November 2019

In 2019, I moved to the Storage team to lead security-related projects and work on Uber's internal storage gateways. Previously, I had led Uber's mobile performance testing efforts, where my team and I did a ton of work to automatically detect performance regressions in our mobile applications before they could impact customers. As a technical lead, I worked with our stakeholders to holistically improve Uber’s reliability and security posture. I was responsible for setting the quarterly roadmap, participated in organizational planning cycles and reported to various layers of leadership on our progress weekly. The project I started ended up becoming a team of 4 engineers with a 5M+ hardware budget.

##### Achievements

* Built a scheduler/platform for executing tests against real devices (Go), including an Android daemon (Go) for reporting performance metrics, a low-level test executor (Python) and a developer-facing web application (React) for visualizing performance data.
* My team demonstrated a 100M+/year ROI for performance improvements that impacted Uber’s customer funnel. I helped convince leadership to continue investing in performance and secured a budget for hardware so we could expand our impact.
* Authored a library for authenticating and routing across Uber's internal edge network. This library dramatically improved the quality of life of our engineers and led to a deprecation of an insecure tunnel into our production environment.
* Built a service to automatically manage Uber’s storage credentials and integrate with our identity infrastructure. This service became critical to storage engine operations and helped secure Uber against bad actors.

#### QUARTET HEALTH, NEW YORK CITY, NY

##### Core APIs, July 2017 – October 2017
Lucky enough to be an early engineer, I was also the only engineer working on Quartet's real-time backend for most of 2016. I helped build up the engineering foundation: metrics aggregation, on call rotations, nightly report generation, automated deployments, general engineering housekeeping and many other mission critical pieces as we scaled our team post-series B. As the organization grew to 60 engineers, I grew into a senior engineering role and helped drive impact on some of the company's most important initiatives.

##### Achievements

* Built Quartet's early version of SmartMatch, which was a recommendation engine for finding the best behavioral health care provider.
* Migrated off of an existing monolithic REST API to a query-driven (think GraphQL) API written in Clojure (using Datomic) that unblocked our application developers. 
* Built an automated state machine system for long-lived business logic workflows. This project alone has saved 1000s of case worker hours and drives Quartet’s patient intake process.
* My team eventually grew to 6 engineers and became the Core Platform. We were responsible for architecting our central application data store, asynchronous background tasks, orchestrating distributed state (i.e. pushing data to Salesforce, building ElasticSearch indices, etc), and pretty much everything considered the backend.
* Served as the technical lead on a team of 4 engineers. Our team overhauled Quartet's insurance modeling, intake processes so we could improve our matching algorithm and get patients to the best providers.


#### AMAZON WEB SERVICES, SEATTLE, WA

##### Software Development Engineer, May 2013 – July 2015

I primarily worked in Amazon Web Services on the Elastic Block Store (EBS) service building distributed systems. I helped plan and execute long-running, complex software projects that impacted 30% of all traffic on the internet.

##### Achievements

* I started and facilitated a daily meeting in my organization to identify reliability anomalies and investigate them.
* I inherited the volume metering system, a critical system responsible for collating volume usage from disparate systems and producing a per-customer record for upstream billing teams. I worked with another engineer to redesign the system and improved the reliability dramatically. 
* Proactively built a service to continually test the EBS control plane from upstream consumers. The system was a success, and we identified AWS API regressions and externally facing bugs.
* Part of a new team that was created to design and launch a distributed key-value store (Physalia), built on top of a replicated log and Paxos. Built and launched the control plane and a reconciler service for restarting failed state transitions. 

## Education

#### TEXAS STATE UNIVERSITY, SAN MARCOS, TX
##### BS in Computer Science, Cum Laude, May 2013

## Awards

#### Uber Office of the CTO Recognition Award
I was one of a select few engineers (out of ~3000) to be formally recognized in 2017. Below is the nomination I received from my manager describing my contributions:

> Benjamin Mays has been a critical engineer that drove the Mobile Detective project - a system that
automatically detects mobile performance regression in our build pipeline. As the first
backend/full-stack engineer on the Mobile Platform team, Ben tackled this project single-handedly,
with very little support. Not only did he reach out and work with the relevant backend teams to build his pipeline, he made multiple systematic fixes and improvements to dependent projects as he went on. Along the way he also identified several org-level systematic issues affecting his workflows, and
communicated and refined his findings with various stakeholders. This culminated in a well-received
presentation to the Ark team. Not only is Benjamin an incredibly talented and productive engineer, he's able to surface problems in a respectful and collaborative manner, and thoroughly embodies Uber's values of ownership and collaboration.
