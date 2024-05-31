# A Certification Scheme Based on Blockchain for Modern Service-Based Systems

[**Nicola Bena**](https://homes.di.unimi.it/bena), [**Marco Pedrinazzi**](https://www.linkedin.com/in/marco-pedrinazzi), [**Marco Anisetti**](https://homes.di.unimi.it/anisetti), [**Omar Hasan**](https://perso.liris.cnrs.fr/omar.hasan/), [**Lionel Brunie**](https://perso.liris.cnrs.fr/lionel.brunie/index-us.html)

> Modern service-based systems are characterized by applications composed of heterogeneous services provided by multiple, untrusted providers, and deployed along the (multi-) cloud-edge continuum. This scenario of increasing pervasiveness, complexity, and multi-party service recruitment urgently calls for solutions to increase applications privacy and security, on the one hand, and guarantee that applications behave as expected and support a given set of non-functional requirements, on the other hand. Certification schemes became the widespread means to answer this call, but they still build on old-fashioned assumptions that hardly hold in today's services world. They assume that all actors involved in a certification process are trusted *by definition*, meaning that certificates are supposed to be correct and be safely usable for decision-making, such as certification-based service selection and composition. In this paper, we depart from such unrealistic assumptions and define the first certification scheme that is completely transparent to the involved actors and significantly more resistant to misbehavior (e.g., collusion). We design a blockchain-based architecture to support our scheme, re-defining the actors and their roles. The quality and performance of our scheme are evaluated in a case study scenario.

## About This Repository

This repository contains real-world evidence collected by real probes against a static website. They are part of the walkthrough.

File names match probe names according to the following rules

- *probe name* refers to the name used in the paper
- for each probe, we provide the corresponding evidence retrieved upon successful execution (i.e., the probe succeeds), and upon unsuccessful execution (i.e., the probe fails - file names ending in `-vuln`).

| **Probe name** | **File** | **Description**|
| - | - | - |
| `Observatory` | [`observatory.json`](observatory.json) and [`observatory-vuln.json`](observatory-vuln.json) | Probe evaluating the compliance to Mozilla [Observatory best practices](https://observatory.mozilla.org/). It returns :white_check_mark: when the latter are followed. |
| `Vuln-Scan-Host` | [`lightweight-vuln-scan.json`](lightweight-vuln-scan.json) and [`lightweight-vuln-scan-vuln.json`](lightweight-vuln-scan-vuln.json) | Probe looking for vulnerabilities in the hosting server. It returns :white_check_mark: when vulnerabilities are not found. |
| `Vuln-Scan-Web` | [`web-vuln-scan.json`](web-vuln-scan.json) and [`web-vuln-scan-vuln.json`](web-vuln-scan-vuln.json) | Probe looking for vulnerabilities in the web technology used by the target server. It returns :white_check_mark: when vulnerabilities are not found. |
| `HTTPS-Strength` | [`sslyze.json`](sslyze.json) and [`sslyze-vuln.json`](sslyze.json) | Probe inspecting the HTTPS setup looking for compliance to best practices. It returns :white_check_mark: when the latter are followed. |
| `HTTPS-Heartbleed` | [`heartbleed.json`](heartbleed.json) and [`heartbleed-vuln.json`](heartbleed-vuln.json) | Probe looking for vulnerability *heartbleed*. It returns :white_check_mark: when the vulnerability is not found. |
