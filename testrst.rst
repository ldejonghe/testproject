Setting up a Windows Host
=========================
This document discusses the setup that is required before Ansible can communicate with a Microsoft Windows host.

.. contents:: Topics

Host Requirements
`````````````````
For Ansible to communicate to a Windows host and use Windows modules, the
Windows host must meet the following requirements:

* Ansible's supported Windows versions generally match those under current
  and extended support from Microsoft. Supported desktop OSs include
  Windows 7, 8.1, and 10, and supported server OSs are Windows Server 2008, 
  2008 R2, 2012, 2012 R2, and 2016.

* Ansible requires PowerShell 3.0 or newer and at least .NET 4.0 to be
  installed on the Windows host.

* A WinRM listener should be created and activated. More details for this can be
  found below.

.. Note:: While these are the base requirements for Ansible connectivity, some Ansible 
    modules have additional requirements, such as a newer OS or PowerShell
    version. Please consult the module's documentation page
    to determine whether a host meets those requirements.
