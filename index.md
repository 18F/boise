---
path: /
---

# Project Boise

_Discovery Overview_

## Overview

- The process by which software staged for use in the federal government is checked for security compliance is known as the “Authority to Operate (ATO)” process. The ATO process is usually handled by either government staff or a third-party vendor.
- “Project Boise” is a working title for a Discovery (exploratory) phase of research that builds upon 18F’s [Compliance Toolkit](https://github.com/18F/compliance-toolkit). The Project Boise team is led by Aidan Feldman, with help from designer Andrew Maier and strategist Timothy Jones.
- In the short term, the Project Boise team will evaluate the ATO landscape and determine where GSA can provide the most value. In the long term, the Project Boise team hopes to reduce the burden (time, cost, and pain) and improve the effectiveness of the federal government’s software security compliance processes.

## Knowns

- ATO is a very broad concept, and involves a large number of stakeholders.  
- The ATO process is universally painful for folks both inside and outside government.
- ATOs impose a significant burden on all agency software projects / acquisitions. They are a consistent blocker to delivery.
- Requirements and processes vary by agency and context (such as internal systems vs. SaaS), so making a one-size-fits-all solution is difficult.
- There is lots of [ATO improvement work](https://docs.google.com/document/d/1LZSoi5JEGIIz3jpwpAD313MTcIXj83wjK4Ujsh7IIvQ/edit) already happening in/around government. Assessing their scope, their “completeness”, their effectiveness, and then the gaps will inform the our future work. We may also find opportunities for consolidation/collaboration between existing efforts.
- GSA/TTS has no regulatory authority. We will need to collaborate with NIST, DHS, and/or OMB if we want to induce policy changes.

## Stakeholders

The ATO process exists at nearly every federal agency, and there are similar processes at state and city levels. Any company selling software to government is required to go through an ATO processes or something similar to it. That said, our primary stakeholders are:

### Agencies/programs

The following agencies/programs help issue security-related policies, requirements, and/or guidance:

- [Department of Homeland Security (DHS) Continuous Diagnostics and Mitigation (CDM)](https://www.dhs.gov/cdm)
- Office of Management and Budget (OMB) / Office of American Innovation (OAI)
- National Institute of Standards and Technology (NIST)
- General Services Administration (GSA)’s Federal Risk and Authorization Management Program (FedRAMP)

### Roles

Within each agency, the following roles are tasked with setting, adapting, enforcing, and/or abiding by their agency’s ATO processes:

- Chief Information Security Officers (CISOs) and their staff
    - Information System Security Managers (ISSMs) and Officers (ISSOs)
- Third-party assessment organizations (3PAOs)
- Authorizing Officials (AOs)
- Teams building/selling federal information systems
    - Software vendors
    - In-house development teams

### Target market

The groups we want our future phases to have measurable impact on are:

- Civilian federal government, not limited to TTS or GSA
- Small-to-medium software vendors and Cloud Service Providers (CSPs), who are current or potential suppliers to government

## Goals

### Long-term

The Project Boise team’s long-term goals include:

- Reducing the burden (time, cost, and pain) around compliance.
- Designing compliance processes that better evaluate the security of systems
- Providing paths and removing barriers to increasing the security of systems
- Improving the visibility of and confidence in the security of systems

### Short-term

More tactically, here are the primary things that Boise will complete in the first ~month:

1. First, we will pick up existing conversations that members of the Boise team have had around ATOs, making sure they are aware of Boise, and submit this pitch for feedback.
1. Second, we will identify and map common compliance journeys. While NIST’s [Risk Management Framework](http://csrc.nist.gov/groups/SMA/fisma/framework.html) provides a high-level view, our team wants to more fully understand the information ecosystems created across federal agencies: what are the various touchpoints, by the various stakeholders, etc? From there we want to categorize what detailed parts of the process are hard vs. soft requirements, and which are government-wide vs. varying by agency.
1. Third, we will finish mapping the areas of ATO work. We will take those various efforts and see where they fall along the mapping, to understand overlap/gaps. This will help steer Boise towards a specific area of the ATO process that is un(der)addressed.

## Hypotheses

### 1. Prescriptiveness is good.

We believe there are big wins in being prescriptive/opinionated, in terms of architecture, technologies, deployment strategy, etc. This is also known as “providing a ‘happy path to the preferred path’,” or “convention over configuration.” Doing so allows each new system to be assessed relatively easily because there is a smaller variance from multiple implementations. It also reduces the amount of effort of the project team, in not needing to figure out the security configuration, operating procedures, etc. of the underlying systems from scratch.

While this is possible (and usually desirable) at the team, division, or even agency/department level, it gets less realistic the further up you go. For example, NIST isn’t going to tell everyone to use a particular IaaS or firewall, while an agency might do so for their systems.

### 2. The ATO process improves teams as much as products.

The ATO process is a great opportunity for security-minded folks to think critically about software, but it doesn’t happen in a vacuum; the ATO process generally requires input from the entire product team. One byproduct of this collaboration is that it encourages team members to frame their future work in light of compliance. (Said differently: Once a cook in a shared kitchen learn it’s unsafe to touch a hot stove, they learn to wear gloves and/or avoid hot stoves in the future.)

By this logic, teams who collaboratively complete the ATO process are better prepared to think about, estimate, and address security issues for future releases. The ATO process therefore presents an opportunity to change the product team itself.

### 3. It is in large vendors’ interests to support small vendors.

The third hypothesis is that large software vendors (particularly Infrastructure/Platform providers) have a vested interest in making it easier for smaller companies and projects within government to get ATOs. These vendors often provide tools on which other projects can build, so making it easier for their customers to get ATOs means more business for the Infrastructure providers. Boise may be able to leverage these companies to get early feedback, as well as broader spread on anything we produce.

### 4. Compliance burden is independent of security maturity.

We believe a system’s security maturity (that is, its real-world threat mitigations) has little-to-no bearing on its compliance burden. Suppose there are two systems, System A and System B. Both systems are of similar size and complexity; both have the same confidentiality, integrity, and availability requirements; and both are ready to enter the ATO process. The only difference between the two is that System A’s security is less mature than System B.

The fourth hypothesis suggests that although System B’s ATO assessment may require slightly less back and forth compared to System A (because System B has a higher level of security maturity it will likely have fewer vulnerability findings and required remediations), both systems will likely require the same amount of time to create their ATO package (go through assessment, penetration testing, etc.).

The fourth hypothesis also suggests an important corollary: Improving security practices is insufficient if our goal is to materially reduce the ATO burden. Instead, we need to focus on improving the ATO process itself.
