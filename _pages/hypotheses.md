---
---

## Prescriptiveness is good.

**We believe there are big wins in being prescriptive/opinionated**, in terms of system architecture, technologies, deployment strategy, etc. This is also known as "providing a ‘happy path to the preferred path'," or "convention over configuration." Doing so allows each new system to be assessed relatively easily because there is a smaller variance from multiple implementations. It also reduces the amount of effort of the project team, in not needing to figure out the security configuration, operating procedures, etc. of the underlying systems from scratch.

While this is possible (and usually desirable) at the team, division, or even agency/department level, it gets less realistic the further up you go. For example, NIST isn't going to tell everyone to use a particular IaaS or firewall, while an agency might do so for their systems.

## The ATO process improves teams as much as products.

The ATO process is a great opportunity for security-minded folks to think critically about software, but it doesn't happen in a vacuum; the ATO process generally requires input from the entire product team. One byproduct of this collaboration is that it encourages team members to frame their future work in light of compliance. (Said differently: Once a cook in a shared kitchen learn it's unsafe to touch a hot stove, they learn to wear gloves and/or avoid hot stoves in the future.)

By this logic, teams who collaboratively complete the ATO process are better prepared to think about, estimate, and address security issues for future releases. The ATO process therefore presents an opportunity to change the product team itself.

## It is in large vendors' interests to support small vendors.

The third hypothesis is that large software vendors (particularly Infrastructure/Platform providers) have a vested interest in making it easier for smaller companies and projects within government to get ATOs. These vendors often provide tools on which other projects can build, so making it easier for their customers to get ATOs means more business for the Infrastructure providers. Boise may be able to leverage these companies to get early feedback, as well as broader spread on anything we produce.

## Compliance burden is independent of security maturity.

**We believe a system's security maturity (that is, its real-world threat mitigations) has little-to-no bearing on its compliance burden.** Suppose there are two systems, System A and System B. Both systems are of similar size and complexity; both have the same confidentiality, integrity, and availability requirements; and both are ready to enter the ATO process. The only difference between the two is that System A's security is less mature than System B.

The fourth hypothesis suggests that although System B's ATO assessment may require slightly less back and forth compared to System A (because System B has a higher level of security maturity it will likely have fewer vulnerability findings and required remediations), **both systems will likely require the same amount of time to create their ATO package** (go through assessment, penetration testing, etc.).

The fourth hypothesis also suggests an important corollary: Improving security practices is insufficient if our goal is to materially reduce the ATO burden. Instead, we need to focus on improving the ATO process itself.
