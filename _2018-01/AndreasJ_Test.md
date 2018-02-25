---
| title  | author | category |
| :----: | :----: | :----: | 
| FMI Design meeting April 2018 in Dresden | Andreas Junghanns ([QTronic GmbH](https://www.qtronic.de/)) | ma |
---

![FMI logo](http://fmi-standard.org/assets/img/fmi-logo.svg "FMI image"){:width="50px"}

The FMI project is focusing its effort to produce the next version of the FMI standard 2.1. During the previous FMI
Design meeting in Munich (November 2017) a (preliminary) list of FMI Change Proposals (FCPs) was approved.
The next meeting in April 2018 will focus on organising compatibility between the different FCPs and prototype implementations.

### Current Alpha Feature List
 - Ports and Icons:
    Help the user to build consistent systems from FMUs and render the systems more intuitively with better representation of structured ports (for instance busses and physical connectors) in the modelDescription.xml.
 - Array variables:
    Allow FMUs to communicate multi-dimensional variables and change their sizes using structural parameters.
 - Clocks and Hybrid Co-Simulation:
    Introduces clocks for synchronization of variables changes across FMUs. Allows co-simulation with events.
 - Binary Data Type:
    Adds an opaque binary data type to FMU variables to allow, for instance, efficiently exchanging of complex sensor data.
 - Intermediate Output Values:
    Allow access of intermediate output values between communication time points from the FMU to disclose relevant subsystem behavior for analysis or advanced co-simulation master algorithms.
 - Source code FMUs:
    Adding more information to the modelDescription.xml file to improve automatic import of source code FMUs.

You are invited to join the discussions in Dresden provided your company signed the FMI Corporate Contributor License Agreement (CCLA).
