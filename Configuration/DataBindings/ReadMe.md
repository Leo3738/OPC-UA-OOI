# OPC UA DataBinding library

## Introduction

This project is aimed at implementing an editor of the **UA Data Application** configuration file. For more extensive examples, see the [OPC UA Data Processing Outside the Server](../../SemanticDataSolution#opc-ua-data-processing-outside-the-server).

The schema of the configuration files is available at:  [ConfigurationData.xsd](../../Configuration/Networking/Serialization/ConfigurationData.xsd) and detailed description of the configuration is captured in the document [UA Data Networking Configuration](../../Configuration/Networking/ReadMe.md#ua-data-networking-configuration).

The code help documentation is available at:
[UAOOI.Configuration.DataBindings Namespace](http://www.commsvr.com/download/OPC-UA-OOI/?topic=html/N-UAOOI.Configuration.DataBindings.htm)

The main changes and Version History are provided by the document [ReadMe.txt](./ReadMe.txt)

The Nuget package is available here: [OPC UA DataBindings Library 1.0.15](https://www.nuget.org/packages/UAOOI.DataBindings/).

To install OPC UA DataBindings Library, run the following command in the  Package Manager Console  

> PM>  Install-Package UAOOI.DataBindings

## Getting Started Tutorial

The topics contained in this section are intended to give you quick exposure to the **UA Data Application** network based data exchange programming experience. Working through this tutorial gives you an introductory understanding of the steps required to create **UA Data Application** configuration custom editor. The editor is to be used by an universal tool supporting OPC UA Information Model design process. For more information on deploying OPC UA Information Model read the document: [OPC UA Information Model Deployment](http://www.commsvr.com/InternetDSL/commserver/P_DowloadCenter/P_Publications/20140301E_DeploymentInformationModel.pdf)

The configuration files are managed using the `UAOOI.Configuration.Networking` component.

### How to implement the custom editor

This section provides hints how to implement a custom editor of any **UA Data Application** processing data. For example the following applications are good candidate to support this role:

* HMI device - displaying incoming data on the screen;
* Supervisory Control and Data Acquisition (SCADA) - equipped with the driver compliant with the standard
* PLC - updating the internal registers using data recovered from the incoming messages.
