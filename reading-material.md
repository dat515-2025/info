# Reading Material for the Cloud Computing Course

Below is a list of resources that I have collected over the last year or so from [Hacker News](https://news.ycombinator.com/) postings.
They are a collection of tutorials, blogs, popular science articles, and links to companies offering various cloud-related services.

I have read many of the articles and blogs and found them helpful.
I have not included resources that failed to meet my criteria for quality and relevance.
However, I have not read every resource, so please use your judgment when exploring these materials.
I have used ChatGPT to categorize and summarize the resources, including the ratings.
So please take the ratings with a big grain of salt, although I have found them to be generally accurate.

If you have feedback on the rating or any resource, please share it with me on Discord.

These are **optional resources** for exploration and inspiration when picking technologies to learn and use for the course's project.
You may use the **ratings** to prioritize your time:

- ⭐️⭐️⭐️ = High importance (strongly recommended)
- ⭐️⭐️ = Medium importance (worth checking if interested)
- ⭐️ = Low importance (niche or advanced interest)

---

## 1. Machine Learning

- **The Pragmatic Programmer for Machine Learning** ⭐️⭐️
  Practical guide to ML development—covers data handling, algorithms, and tooling.
  [ppml.dev][1]

---

## 2. Cloud Development Tutorials

- **Earthly Tutorials** ⭐️⭐️⭐️
  A wide set of hands-on tutorials across languages, frameworks, and CI/CD topics.
  [earthly.dev][2]

- **Blacksmith Guides** ⭐️⭐️
  DevOps-focused guides covering Docker, GitHub Actions, and build optimization.
  [blacksmith.sh][4]

---

## 3. Containers

- **macpine** ⭐️⭐️
  Lightweight Linux VMs for macOS—useful for local containerized development.
  [macpine][6]

- **Podman Quadlets** ⭐️⭐️
  Simplifies container orchestration using Podman systemd integration.
  [podman-quadlet][7]

- **ko.build** ⭐️⭐️⭐️
  Build and deploy Go applications directly to containers, with Kubernetes integration.
  [ko.build][8]

- **Distroless Images (Google)** ⭐️⭐️⭐️
  Minimal container images without OS bloat—reduced attack surface, smaller size.
  [distroless][9]

- **Containerd (Client Guide)** ⭐️
  Tutorial for building custom containerd clients for low-level container work.
  [containerd][10]

---

## 4. Virtualization

- **Unikraft** ⭐️⭐️⭐️
  Framework for building custom unikernels—lightweight, performant, secure.
  [unikraft][12]

- **Firecracker (microVMs)** ⭐️⭐️⭐️
  Ultra-lightweight VMs from AWS—secure, fast, designed for serverless workloads.
  [firecracker][11]

- **The Big Idea Around Unikernels** ⭐️⭐️
  Conceptual article explaining unikernel advantages and challenges.
  [unikernels-bigidea][13]

- **Nanos + OPS.city** ⭐️
  Tools for running unikernels with simple CLI and very fast boot times.
  [nanos][14], [ops.city][15]

---

## 5. Networking

- **XPipe** ⭐️⭐️⭐️
  Connection manager for SSH, containers, tunnels, and terminals in one interface.
  [xpipe][16]

- **Tailscale** ⭐️⭐️⭐️
  Zero-trust VPN enabling secure connectivity across devices and clouds.
  [tailscale][17]

- **Tailscale in Practice** ⭐️
  Blog post describing real-world workflows with Tailscale.
  [tailscale-blog][18]

- **Localhost & Reverse Proxy Tricks** ⭐️
  Explains how to simplify local development with custom domain tricks.
  [inclouds][19]

---

## 6. Infrastructure and Orchestration

- **Talos Linux** ⭐️⭐️⭐️
  Immutable OS built specifically for running Kubernetes clusters.
  [talos][23]

- **Terraform (HashiCorp)** ⭐️⭐️⭐️
  Industry-standard infrastructure as code tool.
  [terraform][20]

- **Dagger** ⭐️⭐️⭐️
  Modern toolkit for defining portable CI/CD pipelines with composable building blocks.
  [dagger.io][3]

- **Nomad (HashiCorp)** ⭐️⭐️
  Simpler alternative to Kubernetes for scheduling containers and VMs.
  [nomad][21]

- **Edka.io** ⭐️⭐️
  Affordable Kubernetes cluster provisioning on Hetzner.
  [edka][22]

---

## 7. Kubernetes

- **Rancher RKE2** ⭐️
  Enterprise-ready Kubernetes distribution.
  [rke2][25]

- **Rancher Desktop** ⭐️⭐️
  Kubernetes and container management directly from desktop.
  [rancher-desktop][26]

- **Kubetail** ⭐️⭐️
  Kubernetes log tailing tool—aggregate logs from pods in real time.
  [kubetail][27]

- **Kubernetes & Databases** ⭐️⭐️
  New approaches for managing stateful workloads with Kubernetes.
  [kube-databases][28]

- **Kubernetes 2.0 Speculation** ⭐️
  Thought experiment on what a redesign of Kubernetes might look like.
  [kube2][29]

- **Kubernetes Problems** ⭐️⭐️
  Critical blog post on Kubernetes complexity and pain points.
  [kube-problems][30]

- **Kubernetes vs Virtual Machines** ⭐️
  Compares Kubernetes orchestration with VM-based approaches.
  [kube-vs-vm][31]

- **First Contact with Kubernetes** ⭐️⭐️
  Blog post narrating a developer’s skeptical journey into Kubernetes.
  [kube-first-contact][32]

- **Replacing Kubernetes with systemd** ⭐️
  Argues that Kubernetes may be overengineered for simpler deployments.
  [kube-systemd][33]

---

## 8. System Design

- **Good System Design (Blog)** ⭐️⭐️⭐️
  Critique of common system design advice, with pragmatic alternatives.
  [system-design][34]

- **How to Write a Design Document** ⭐️⭐️
  Practical tips for clear and effective technical design docs.
  [design-doc][35]

---

## 9. Security

- **Why Bloat Is Still Software’s Biggest Vulnerability** ⭐️⭐️
  Explores risks from unnecessary software complexity.
  [ieee-bloat][36]

- **Principles of Software Memory Safety** ⭐️⭐️⭐️
  Argues for standardized memory-safe practices in modern development.
  [cacm-memory-safety][37]

---

## 10. Cloud Providers

- **Netcup** ⭐️
  Low-cost provider of bare-metal and virtualized servers.
  [netcup][38]

- **Vultr High-Frequency Compute** ⭐️⭐️
  Affordable compute with global availability.
  [vultr][39]

- **Fly.io** ⭐️⭐️⭐️
  Global edge hosting platform—deploy apps close to users.
  [flyio][40]

- **Tigris Data (Fly.io Partner)** ⭐️
  Managed NoSQL data service integrated with Fly.io.
  [tigris][41]

---

## 11. Perspectives and Critiques

- **Meta Hyperscale Infrastructure (CACM)** ⭐️⭐️⭐️
  Insights into Meta’s massive infrastructure architecture.
  [meta-infra][45]

- **Microservices for Startups** ⭐️⭐️⭐️
  Explains why startups should usually begin with monoliths, not microservices.
  [microservices-startups][43]

- **Don’t Microservice, Do Module** ⭐️⭐️
  Suggests modular monoliths as a simpler alternative to microservices.
  [dont-microservice][44]

- **The Future Is Not Self-Hosted** ⭐️⭐️
  Blog arguing that cloud reliance is inevitable—"the cloud is someone else’s computer."
  [future-not-selfhosted][42]

- **DBOS Blog** ⭐️
  Describes a new "three-tier" architecture using DBOS cloud runtime.
  [dbos][24]

[1]: https://ppml.dev/index.html
[2]: https://earthly.dev/blog/
[3]: https://dagger.io/
[4]: https://www.blacksmith.sh/guides
[6]: https://github.com/beringresearch/macpine
[7]: https://podman-desktop.io/blog/podman-quadlet
[8]: https://ko.build
[9]: https://github.com/GoogleContainerTools/distroless
[10]: https://github.com/containerd/containerd/blob/main/docs/getting-started.md#implementing-your-own-containerd-client
[11]: https://firecracker-microvm.github.io
[12]: https://unikraft.org
[13]: https://changelog.com/posts/the-big-idea-around-unikernels
[14]: https://nanos.org/thebook
[15]: https://ops.city
[16]: https://xpipe.io/
[17]: https://tailscale.com
[18]: https://chameth.com/how-i-use-tailscale/
[19]: https://inclouds.space/localhost-domains
[20]: https://developer.hashicorp.com/terraform
[21]: https://www.hashicorp.com/en/pricing?tab=nomad
[22]: https://edka.io/
[23]: https://www.talos.dev
[24]: https://www.dbos.dev/blog/new-three-tier-application
[25]: https://github.com/rancher/rke2/tree/v1.33.1%2Brke2r1
[26]: https://github.com/rancher-sandbox/rancher-desktop
[27]: https://github.com/kubetail-org/kubetail
[28]: https://thenewstack.io/kubernetes-finally-solves-its-biggest-problem-managing-databases/
[29]: https://matduggan.com/what-would-a-kubernetes-2-0-look-like/
[30]: https://blog.adamchalmers.com/kubernetes-problems/
[31]: https://iximiuz.com/en/posts/kubernetes-vs-virtual-machines/
[32]: https://blog.davidv.dev/posts/first-contact-with-k8s/
[33]: https://blog.yaakov.online/replacing-kubernetes-with-systemd/
[34]: https://www.seangoedecke.com/good-system-design/
[35]: https://grantslatton.com/how-to-design-document
[36]: https://spectrum.ieee.org/lean-software-development
[37]: https://cacm.acm.org/opinion/it-is-time-to-standardize-principles-and-practices-for-software-memory-safety/
[38]: https://www.netcup.com/en
[39]: https://www.vultr.com/products/high-frequency-compute/
[40]: https://fly.io
[41]: https://www.tigrisdata.com/docs/overview/
[42]: https://www.drewlyton.com/story/the-future-is-not-self-hosted/
[43]: https://nexo.sh/posts/microservices-for-startups/
[44]: https://yekta.dev/posts/dont-microservice-do-module/
[45]: https://cacm.acm.org/research/metas-hyperscale-infrastructure-overview-and-insights/
