openetcs-updatesite
===================
<pre>
Copyright (c) 2014
Fraunhofer-Institut für Eingebettete Systeme und Kommunikationstechnik ESK

Hansastr. 32
80686 Munich
Germany
</pre>

Eclipse Update Site
===================

Add the following link as an additional update site to Eclipse. 

<pre>https://raw.github.com/astante/openetcs-updatesite/master</pre>

Contents
========

OpenETCS SysML / Scade Integration
----------------------------------

The plugin contains a transformation of SysML to Scade utilizing the Scade API (Esterel Scade Suite License necessary). The purpose of the integration is to transform the OpenETCS WP3 SysML architecture models to Scade for software design. Within the project certain extension were made (for example introduction of a Data Dictionary) which is not supported via the integration shipped with Scade.

Installation
============

Prerequisits
------------

* Valid Scade Suite installation
* OpenETCS Toolchain 

Steps
-----

Launch the OpenETCS Toolchain and select `Help > Install New Software...`.

![][install-new-software]

Add Update Site for the Scade API by selecting `Add` and providing the following information:
* Name: Scade API
* Location: Path to the Scade Update Side in the installation directory, for example `C:\Program Files\Esterel Technologies\SCADE R15.2\SCADE\eclipse`
 
The update site can be selected via the `Local` button.

![][scade-updatesite]

Install the following plugins from the udpate site:

![][scade-plugins]

Add another update site for the OpenETCS Scade Integration by providing the following information:
* Name: OpenETCS Scade Integration
* Location: https://raw.github.com/astante/openetcs-updatesite/master
 
After installation you can use the plugin by right clicking on a Papyrus model and selecting `OpenETCS > Generate SCADE Suite Project`

![][usage-scade-integration]

[install-new-software]: https://raw.github.com/wiki/astante/openetcs-updatesite/images/install-new-software.png "Install New Software"
[scade-updatesite]:  https://raw.github.com/wiki/astante/openetcs-updatesite/images/scade-udpatesite.png "Add Scade Update Site"
[scade-plugins]: https://raw.github.com/wiki/astante/openetcs-updatesite/images/scade-plugins.png "Install Scade Plugins"
[usage-scade-integration]: https://raw.github.com/wiki/astante/openetcs-updatesite/images/usage-scade-integration.png "Use Scade Integration"
