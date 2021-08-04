# Installing DynAdjust

The steps required to install DynAdjust on your system will depend upon your operating system, and whether or not you choose to [build from source code](BUILDING.md) or install pre-built binaries. In addition, installation may require the installation (or building) of one or more prerequisite applications that are external to DynAdjust but essential for its installation and use.

## Contents
- [Linux, Mac and Windows](#linux-mac-and-windows)
- [Windows only](#windows-only)
  

## Linux, Mac and Windows

[![docker build](https://img.shields.io/github/workflow/status/icsm-au/dynadjust/Build%20docker%20image?label=docker%20build)](https://hub.docker.com/repository/docker/icsm/dynadjust)
[![Docker Pulls](https://img.shields.io/docker/pulls/icsm/dynadjust)](https://hub.docker.com/repository/docker/icsm/dynadjust)

The DynAdjust repository comes with a [Dockerfile](https://github.com/icsm-au/DynAdjust/blob/master/Dockerfile) which builds a DynAdjust docker image for the Linux environment each time changes are pushed to the main repository. This means if you have docker installed on your system, a DynAdjust image can be run on your system (whether Linux, Mac or Windows) within a virtual enviroment managed by docker.

To access the latest docker image, please visit the [DynAdjust repo on Docker Hub](https://hub.docker.com/r/icsm/dynadjust).

Alternatively, you can pull a DynAdjust docker image from your system via:

  ``` bash
  $ docker pull icsm/dynadjust
  ```

## Windows only

[![GitHub Releases](https://img.shields.io/github/v/release/icsm-au/DynAdjust.svg)](https://github.com/icsm-au/DynAdjust/releases)

For each stable release, DynAdjust binaries are built using Microsoft Visual Studio 2017 and published on the [releases page](https://github.com/icsm-au/dynadjust/releases/latest).

To install DynAdjust on Windows:

1. Download the latest pre-built Windows (64-bit) binaries from the [releases page](https://github.com/icsm-au/dynadjust/releases/latest) to a dedicated folder (not the Desktop) on your system.  Add the location of this folder to your system's path environment variables so that DynAdjust can be executed from any location on your system.

2. Install the following (64-bit) libraries and dependencies:
   1. Apache Xerces-C++ XML Parser: <http://xerces.apache.org/xerces-c/download.cgi>
   2. Codesynthesis XSD XML Data Binding for C++: <https://www.codesynthesis.com/products/xsd/download.xhtml>
   3. Intel Math Kernel Library: <https://software.seek.intel.com/performance-libraries>
   4. Microsoft Visual C++ Redistributable for Visual Studio 2017: <https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads>, or <https://visualstudio.microsoft.com/downloads/> > _Other Tools and Frameworks_ > _Microsoft Visual C++ Redistributable for Visual Studio 2019_
