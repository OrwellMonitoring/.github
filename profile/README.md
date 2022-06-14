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


