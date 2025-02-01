# Low-Spec Server Software

The software industry is obsessed with "scale." Applications are built assuming millions
of users, vastly unpredictable traffic, and an endless appetite for cloud scalability.
Yet, for most projects and the server software they need, this is completely
unnecessary and wasteful.

It's time that tech leaders start to prioritize efficiency,
simplicity, and reliable performance on modest hardware.

## The Problems with the "High-Spec" Mindset
When modern web applications assume they need to scale to a large number of users,
they hit a few problems:

1. **Infinite Scalability**: Cloud platforms make it easy to scale up, but most of
   us don't have infinite budgets to match.
3. **Complex Architectures**: Overengineering with microservices / serverless
   deployments when a simple monolith is perfectly reasonable. Complex Architectures
   are difficult to debug and test, leading to delays and downtime when the
   unexpected occurs.
4. **Generous Resources**: Assuming the latest multi-core CPUs and large amounts of
   RAM instead of minimizing resource usage.
5. **Environmental Impact**: Excessive resource consumption leads to higher energy
   usage, and continuously upgrading hardware leads to more e-waste and pollution.

These assumptions lead to bloated, expensive, and inefficient software that excludes
users with limited access to high-performance infrastructure.

## Why Low-Spec Software Matters
Server software can be much more efficient, simple, and accessible by focusing on
deployment to "low spec" servers. This focus would lead to:

- **Lower Costs**: Runs on minimal hardware, reducing both up-front and ongoing
  hosting expenses.
- **Broader Accessibility**: Works on older devices and in regions with limited
  access to high bandwidth.
- **Reliability**: Fewer dependencies and moving parts mean fewer points of failure.
- **Longer Uptimes and Lifespan**: Less need for hardware refreshes and continues
  performing well even on aging hardware.
- **Sustainability**: Consumes less energy, reducing environmental impact.
- **Self-Hosting**: Makes personal and small-scale deployments feasible.

Optimizing for lean, efficient server software benefits both your organization
and your users *TODAY*.

## Experience is key to adoption

We can't just focus on code and technology, to be successful in these goals the
server software MUST be easy to deploy and use. We have a few principles to
simplify deployment of low-spec server software:

1. **Single Binary**: The application should be a single binary, which can be
   copied anywhere suitable for execution. No lengthy installs, multiple
   configuration options, or need for a working docker setup.
2. **Simple Upgrades**: With a single binary, updated software should just drop
   in place and automatically perform any data migrations. Make it easy for your
   users to stay secure.
3. **Progressive Dependencies**: At a small scale, sqlite and a LRU cache in
   memory can work wonders. A basic install should "just work" with some
   reasonable defaults, as usage increases things can be scaled to external
   services like PostgreSQL or redis caches.
4. **Streamlined Setup**: Descriptive setup flows should be preferred to
   unwieldly manual editing of config files.
5. **Opt-in telemetry**: *NEVER* send data without positive confirmation first.
6. **Hardware benchmarks**: Include performance benchmarks so that people know
   what to expect for their available hardware and installation.

Together these principles will ensure that people WANT to install low-spec
server software that meets their needs. By making installation as easy and
unsurprising as possible, we can make an impact to hopefully offset the
extreme power usage caused by AI development and cryptocurrency projects.
