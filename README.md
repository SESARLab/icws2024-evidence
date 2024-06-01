# A Certification Scheme Based on Blockchain for Modern Service-Based Systems

[![CC BY 4.0][cc-by-shield]][cc-by]

[**Nicola Bena**](https://homes.di.unimi.it/bena), [**Marco Pedrinazzi**](https://www.linkedin.com/in/marco-pedrinazzi), [**Marco Anisetti**](https://homes.di.unimi.it/anisetti), [**Omar Hasan**](https://perso.liris.cnrs.fr/omar.hasan/), [**Lionel Brunie**](https://perso.liris.cnrs.fr/lionel.brunie/index-us.html)

> Modern service-based systems are characterized by applications composed of heterogeneous services provided by multiple, untrusted providers, and deployed along the (multi-) cloud-edge continuum. This scenario of increasing pervasiveness, complexity, and multi-party service recruitment urgently calls for solutions to increase applications privacy and security, on the one hand, and guarantee that applications behave as expected and support a given set of non-functional requirements, on the other hand. Certification schemes became the widespread means to answer this call, but they still build on old-fashioned assumptions that hardly hold in today's services world. They assume that all actors involved in a certification process are trusted *by definition*, meaning that certificates are supposed to be correct and be safely usable for decision-making, such as certification-based service selection and composition. In this paper, we depart from such unrealistic assumptions and define the first certification scheme that is completely transparent to the involved actors and significantly more resistant to misbehavior (e.g., collusion). We design a blockchain-based architecture to support our scheme, re-defining the actors and their roles. The quality and performance of our scheme are evaluated in a case study scenario.

## About

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

The complete material at the basis of our paper can be found [here](https://doi.org/10.13130/RD_UNIMI/FBGMZY).

## Citation

It is mandatory to cite our publication, according to our license.

The paper can be cited as follows:

```bibtex
@inproceedings{BPAHB.ICWS2024,
  author = {Bena, Nicola and Pedrinazzi, Marco and Anisetti, Marco and Hasan, Omar and Brunie, Lionel},
  title = {A Certification Scheme Based on Blockchain for Modern Service-Based Systems},
  booktitle = {Proc. of IEEE ICWS 2024},
  year = {2024},
  address = {Shenzhen, China},
  month = jul
}
```

## Acknowledgements

The work was partially supported by:

- project MUSA - Multilayered Urban Sustainability Action – project, funded by the European Union – NextGenerationEU, under the National Recovery and Resilience Plan (NRRP) Mission 4 Component 2 Investment Line 1.5: Strengthening of research structures and creation of R&D "innovation ecosystems", set up of "territorial leaders in R&D" (CUP G43C22001370007, Code ECS00000037)
- project SERICS (PE00000014) under the NRRP MUR program funded by the EU - NextGenerationEU
- Università degli Studi di Milano via the program "piano sostegno alla ricerca" and "One Health Action Hub: University Task Force for the resilience of territorial ecosystems" – PSR 2021 – GSA – Linea 6
- SCUSI projet – Région Auvergne-Rhône-Alpes

Views and opinions expressed are however those of the authors only and do not necessarily reflect those of the European Union or the Italian MUR. Neither the European Union nor the Italian MUR can be held responsible for them.

## License

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg