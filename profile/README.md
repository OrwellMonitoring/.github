# Orwell   
5G networks are fiercely developing and so are the vertical applications of this technology, in fields such as Automotive, 4.0 Industry or Public Protection and Disaster Relief. To develop new 5G applications, researchers need to test them. However, the price of 5G infrasctructure and the required expertise to assemble a fully functional testbed may be a barrier that some cannot overcome. This led to the creation of 5G testbeds with state-of-the-art technology which allow NetApp developers to have access to the required infrastructure to test their applications without having to worry about all the deployment process. These tests require a controlled environment, thus all the infrastructure has to be monitored. This work discusses an approach that complies with 5GASP directives and centralizes all the information on a unique time-series database. Moreover, the proposed methodologies were implemented in a proof of concept product which demonstrates the potential of the proposed approach on a working testbed.
## What is Orwell

Orwell is a monitorization system created to keep track of 5G testbeds' metrics following the 5gasp standards.  
However, due to its modularity it is possible to use this monitoring system in a wide range of systems. It is easy to develop new modules which makes possible the use of any metrics collection tool, you just have to choose the ones you like the most.

- **Be non intrusive**
    As shown earlier in this document, there are already some solutions for monitoring
testbeds. However, in order to make NetApp developers trust the testbed and test results, the less
interference in the tests, the better.  

- **Transparency**
    Another key point mentioned is that, regardless of the toolkit used, the information
must be available through an uniform access interface that offers all the information in a unique format.

- **Open Source**
    A big part of this project relies on open source tools, so this project must give back
to the community what the community has given it. Besides, 5GASP aims to speed up the research
process offering tools to test new 5G applications, so Orwell must follow the same purpose.

- **Modularity**
    Testbeds’ infrastructures have big and complex architectures, sometimes with several
system admins and more than one project on the same infrastructure. For that reason, this project must
be as divisible as possible, so system admins can choose only what makes sense in their reality. Another
advantage of having a modular and a micro-service oriented architecture is the possibility of adapting
some modules without having to study all the code.
