# Orwell
## Monitorization Platform for 5G Testbeds

### Abstract
5G networks are fiercely developing and so are the vertical applications of this technology, in fields such as Automotive, 4.0 Industry or Public Protection and Disaster Relief. To develop new 5G applications, researchers need to test them. However, the price of 5G infrasctructure and the required expertise to assemble a fully functional testbed may be a barrier that some cannot overcome. This led to the creation of 5G testbeds with state-of-the-art technology which allow NetApp developers to have access to the required infrastructure to test their applications without having to worry about all the deployment process. These tests require a controlled environment, thus all the infrastructure has to be monitored. This work discusses an approach that complies with 5GASP directives and centralizes all the information on a unique time-series database. Moreover, the proposed methodologies were implemented in a proof of concept product which demonstrates the potential of the proposed approach on a working testbed.

### What is Orwell?

Orwell is a monitorization system created to keep track of 5G testbeds' metrics following the 5gasp directives.  
However, due to its modularity it is possible to use this monitoring system in a wide range of systems. It is easy to develop new modules which makes possible the use of any metrics collection tool, you just have to choose the ones you like the most. Besides monitoring the deployed VNFs, Orwell also collects data related to network performance using PerfSonar and 5G Core through Huawei's eSight API. Our system also provides security monitoring, via Suricata for network packets content and Infection Monkey for network exploitation. Orwell stands out for being:

- **Non intrusive**
    In order to make NetApp developers trust the testbed and test results, the less
interference in the tests, the better.  

- **Transparency**
    Another key point mentioned is that, regardless of the toolkit used, the information
must be available through an uniform access interface that offers all the information in a unique format.

- **Open Source**
    A big part of this project relies on open source tools and, since we wanted to contribute to the community, we followed the same path.

- **Modular**
    Testbeds’ infrastructures have big and complex architectures, sometimes with several
system admins and more than one project on the same infrastructure. For that reason, this project must
be as divisible as possible, so system admins can choose only what makes sense in their reality. Another
advantage of having a modular and a micro-service oriented architecture is the possibility of adapting
some modules without having to study all the code.

An API was developed to provide an uniform access interface which we consider to be the core and the orchestrator of out system. Orwell's robust core together with the developed modules provides multiple advantages, but this solution can be developed as desired in order to meet other use cases different from the initial scope of the project.

### Architecture

![Orwell Architecture](https://orwellmonitoring.github.io/assets/architecture.png)

All the modules presented in Orwell Architecture have a mechanism of one touch deployment (mostly Docker) which makes it easy to assemble your own architecture and solution based on your needs.

### Repositories

- [perfsonar-utils](https://github.com/OrwellMonitoring/perfsonar-utils): collection of tools that abstract the interaction with PerfSonar.
- [orwellmonitoring.github.io](https://github.com/OrwellMonitoring/orwellmonitoring.github.io): project's website source code
- [deliverables](https://github.com/OrwellMonitoring/deliverables): all the deliverables we developed throughout the course like presentations and posters
- [documentation](https://github.com/OrwellMonitoring/documentation): documentation web site source code
- [orwell-documentation](https://github.com/OrwellMonitoring/orwell-documentation): docussaurus code
- [orwell-middleware](https://github.com/OrwellMonitoring/orwell-middleware): Orwell's API, Gnocchi Puller and Service Discovery
- [orwell-translators](https://github.com/OrwellMonitoring/orwell-translators): source code for all translators
- [orwell-python-package](https://github.com/OrwellMonitoring/orwell-python-package): our python package source code
- [esight_connector](https://github.com/OrwellMonitoring/esight_connector): eSight's pull service
- [suricata_config](https://github.com/OrwellMonitoring/suricata_config): Suricata configuration files
- [orwell-manager](https://github.com/OrwellMonitoring/orwell-manager): Orwell's configuration WebApp 
- [report](https://github.com/OrwellMonitoring/report): our report's latex files
- [infection-monkey-api](https://github.com/OrwellMonitoring/infection-monkey-api): selenium API for Infection Monkey interface
- [orwell-boot-services](https://github.com/OrwellMonitoring/orwell-boot-services): all services used to produce OS Images with built in metrics exporters
- [orwell-storage-visualization](https://github.com/OrwellMonitoring/orwell-storage-visualization): Prometheus and Grafana configuration

---

Is you want to know more about this project, please consider taking a look at these assets:
- [Project website](https://orwellmonitoring.github.io/)
- [Documentation website](https://orwellmonitoring.github.io/documentation/)
- [Report](https://raw.githubusercontent.com/OrwellMonitoring/orwellmonitoring.github.io/main/docs/report.pdf)
- [Project Demo](https://orwellmonitoring.github.io/)
- [Project Promotional Video](https://www.youtube.com/watch?v=L7V7thHMmHw)

---

Project developed by:

- [Alexandre Serras](https://github.com/alexandreserras)
- [Gonçalo Leal](https://github.com/goncalo-leal)
- [Pedro Duarte](https://github.com/PedroDuarte536)
- [Vasco Regal](https://github.com/VascoRegal)

Advised by:

- [Rafael Direito](https://github.com/rafael-direito)
- [Diogo Gomes](https://github.com/dgomes)
