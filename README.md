# Carbon Measurement Engine (Carmen)

<img src="./docs/static/carmen-logo.svg" alt="Carmen logo" width="125" />

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GSF Project](https://img.shields.io/badge/GSF-Software_Project-brightgreen)](https://greensoftware.foundation)

> **Carbon Measurement Engine for Cloud Applications**

Managed by the [Software Standards Working Group](https://github.com/Green-Software-Foundation/software-standards-wg) in the [Green Software Foundation](https://greensoftware.foundation).

---

## Overview

Carmen (Carbon Measurement Engine) is an open-source tool that enables organizations to measure the carbon footprint of their cloud-based software at two critical levels:

- **Infrastructure Level** - Monitor energy consumption and carbon emissions from Virtual Machines, storage, and other cloud services
- **Application Level** - Track the carbon footprint of individual applications and workloads running in your cluster

Carmen integrates seamlessly with industry-standard tools like Kubernetes, Prometheus, and Kube State Metrics, and is built on top of the Impact Framework developed by the Green Software Foundation.

### Appointments

The project is led by:
* [Florent Morel (Amadeus)](https://github.com/florent-morel)
* [Robin Castellon (Amadeus)](https://github.com/robin-castellon)

### Status

**This is draft software only and has not been approved or adopted by the Green Software Foundation. this draft may not be relied upon for any purpose other than review of the current state of development.**

## Motivation

Carmen was created by a group of Amadeus engineers in response to the growing importance of sustainability in the tech industry. As carbon emissions from digital infrastructure continue to rise, organizations need accurate tools to measure and reduce their environmental impact.

Our primary goal is to empower engineering teams to understand the carbon footprint of their cloud applications, enabling them to make informed decisions and take meaningful action toward sustainability. By open-sourcing Carmen, we hope to help companies worldwide join the movement toward greener software.

In 2026, Amadeus donated Carmen to the Green Software Foundation, assigning the copyright in the project to the Foundation. Carmen is now owned and managed by the GSF under the Software Standards Working Group, and remains MIT-licensed.

## Key Features

### Infrastructure Monitoring

The Carmen daemon collects Virtual Machine usage data and processes it through the Impact Framework to generate comprehensive reports on energy consumption and carbon emissions for each VM. Future releases will extend this capability to storage and other cloud services.

### Application Monitoring

Carmen's API can be deployed as a sidecar container within your Kubernetes cluster. By connecting to your local Prometheus instance, Carmen retrieves CPU and memory usage metrics from your pods and computes detailed insights into the energy consumption and carbon footprint of your workloads over any specified time range.

## Is Carmen the right tool for you?

Carmen is an **engineering tool**, built by engineers for engineers. It is for **optimisation and introspection** — identifying concrete parts of your infrastructure where you can reduce emissions. 

Carmen is probably **not** the right tool if you need:
- Carbon figures for corporate/ESG reporting
- Numbers for a press release or marketing material
- Compliance or regulatory disclosures

Carmen **is** the right tool if you want to:
- Know which services, VMs, or pods in your stack emit the most CO2
- Compare components and prioritise reductions
- Feed per-component carbon scores into your own FinOps dashboards or internal tooling
- Give developers granular, actionable insights into the carbon footprint of their code

## Documentation

### [Quick Start Guide](./docs/quick-start-guide.md)

For more detailed information on using Carmen, refer to our comprehensive guides:

- **[Carmen as a Service](./docs/carmen-as-a-service.md)** - Deploy Carmen as an API service in your Kubernetes cluster
- **[Carbon Reporting Daemon](./docs/carmen-daemon.md)** - Generate infrastructure-level carbon reports using the Carmen daemon
- **[Methodology](./docs/methodology.md)** - Understand how Carmen calculates carbon emissions
- **[Comparison with Other Tools](./docs/comparison-with-other-tools.md)** - See how Carmen compares to alternative solutions

## Contributing

We welcome contributions from the community! Whether you're fixing bugs, adding features, improving documentation, or sharing feedback, your input helps make Carmen better for everyone.

Please read our [Contributing Guide](./docs/CONTRIBUTING.md) to get started.

## License

Carmen is released under the [MIT License](./LICENSE).

## Acknowledgments

Carmen is built on the shoulders of the open-source community. We're grateful to:

- **[Impact Framework](https://github.com/Green-Software-Foundation/if)** by the Green Software Foundation - The core framework that powers Carmen's carbon calculations
- **[Cloud Carbon Footprint](https://www.cloudcarbonfootprint.org/)** - For pioneering work in cloud carbon measurement methodologies
- The Kubernetes, Prometheus, and open-source monitoring communities

### Carmen original Team

Carmen was developed and maintained by these outstanding people:

**Carmen creators & project leaders:**
- Robin CASTELLON
- Florent MOREL

**Contributors:**
- Adam Hafiz BIN AHMAD
- Ahmad ELGHOBASHY
- Ahmed ASHOUR
- Amulya LAKKU
- Ashly Maria PRINCE
- Berkay ALKAN
- Cosmin BANICA
- Dariel BEZERRA DE SOUSA
- Eleonore GUEIT
- Kevin COUTELLIER
- Mohamed-Akram MASROUR
- Mouhamad AL MOUNAYAR
- Nicolas GAZELLE DOUKHAN
- Pierre-Luc NOEL
- Pranjal RAJ
- Sami GHARBI
- Selen UYGUN
- Sertay AKPINAR
- Thibaut CHASSIGNET
- Xu HE
- Yannick DEVAUX
