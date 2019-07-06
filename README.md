brand-concepts
==============

[Offscale.io](https://offscale.io) / [Sydney Scientific Pty Ltd](https://scientific.sydney)—and possibly Sydney Scientific Foundation Ltd—is seeking brand concepts for websites, apps, and presentations.

## License
[Open-source](https://en.wikipedia.org/wiki/Open-source_software). ([MIT](https://opensource.org/licenses/MIT) OR [Apache-2.0](https://opensource.org/licenses/Apache-2.0)) multi-licensed. No patents.

---

## Principles
Scalable from 1 node to 10,000. Build low-level, functional, structures.

With the excpetion of frontends (e.g.: 3/4 of CDD)—and our multicloud—everything is built with [Rust](https://www.rust-lang.org). Which has serious performance advantages—beating C++ in some benchmarks—while also being safer.

### Scaling on the low end
Other [Mesos](https://mesos.apache.org/)-based solutions don't come close to 1 node usability. Really 5 minimum, 11 prefered minimum.

A key differentiator is support on a single node—e.g.: a developer's laptop—all the way up to a clustered deployment (3 nodes), to serious scale (10,000 maximum).

---

## Products

### [CI/CD](https://en.wikipedia.org/wiki/CI/CD) pipelines
[CI](https://en.wikipedia.org/wiki/Continuous_integration)/[CD](https://en.wikipedia.org/wiki/Continuous_deployment) pipelines allow developers to go from code to production deployments, by automating testing, packaging, binding (ports; DNS), and audience-specific feature releases ([canary](https://martinfowler.com/bliki/CanaryRelease.html)).

#### [Dotfile](https://en.wikipedia.org/wiki/Dotfile) style
*Examples: [Travis CI](https://travis-ci.com); [Appveyor](https://www.appveyor.com); [Gitlab CI](https://docs.gitlab.com/ee/ci); [Azure Pipelines](https://azure.microsoft.com/en-au/services/devops/pipelines); [Dockerfile](https://docs.docker.com/engine/reference/builder); & other competitors*.

Take any CI/CD config format as input, produce any as output.

Have own format also, and a static binary that can run on this format.

So now you can self-host your own [CircleCI](https://circleci.com) competitor.

#### [Mesosphere](https://mesosphere.com) style
[Datacentre operating systems](https://dcos.io). Again, like all Mesos-based technologies, it's for medium to large scale deployments only. With Offscale.io's contributions, it can now work on a single node.

### Compiler Driven Development (CDD)
An alternative to [Xamarin (C#) from Microsoft](https://visualstudio.microsoft.com/xamarin) and [Flutter (Dart) from Google](https://flutter.dev), which doesn't tradeoff development speed for: application runtime overhead; debuggability; testing; best-practice, and extensibility. Additionally, *CDD* also handles backends.

Code natively: [iOS (Swift)](https://developer.apple.com/swift); [Android (Java)](https://developer.android.com/reference); web ([Angular: TypeScript & HTML](https://angular.io)); backend (Rust: [actix](https://actix.rs) & [diesel](https://diesel.rs)). Translate model changes automatically across—and within—language boundaries. 36× speedup.

#### Designer
Similar to [Microsoft Access](https://products.office.com/en-au/access) and [Google Forms](https://gsuite.google.com.au/intl/en_au/products/forms), *[the designer](https://github.com/offscale/model-designer-rfc/blob/master/rfcs/index.md)* allows non-technical *creator-users* to create model-driven workflows for their *end-users*.

Builds upon [CDD](#compiler-driven-development-cdd) base and CI/CD pipelines, to enable release of new applications (backend, web to DNS names [possibly on a CDN], native mobile apps to app stores), all at the fingertips of the *creator-user*.

Engineers can then optimise and extend what's created, as it's all statically generated best-practice conforming code.

Concrete schemas also have significant advantages for data-analytics, especially on the performance side.

---

## Inspiration
Conceptual similarities can be found from our major competitors, in particular: [HashiCorp](https://www.hashicorp.com); Mesosphere; Flutter; and Google Forms.

HashiCorp probably does it best, with different websites for each product, and a central website showing them all. Each product in their 'suite' can be used independently, most are open-source, and their themes are variations of the [master](https://en.wikipedia.org/wiki/Web_template_system). See: [Consul](https://www.consul.io); [Terraform](https://www.terraform.io); [Vagrant](https://www.vagrantup.com); [Vault](https://www.vaultproject.io); [Packer](https://www.packer.io); [Sentinel](https://www.hashicorp.com/sentinel); and [Nomad](https://www.hashicorp.com/products/nomad).
