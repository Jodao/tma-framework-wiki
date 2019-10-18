# Welcome to the TMA Framework wiki!


The following pages provide links for relevant information. 

* [F.A.Q. on Probes Development](F.A.Q.-on-Probes-Development);
* [F.A.Q. on Platform Deployment](F.A.Q.-on-Platform-Deployment);
* [F.A.Q. on Actuators Development](F.A.Q.-on-Actuators-Development).

## Repositories Structure

The [`TMA Framework`](https://github.com/eubr-atmosphere/tma-framework) will follow an adaption of the `MAPE-K` concepts. 
Therefore, a repository structure was defined that is based on [this repository](https://github.com/eubr-atmosphere/tma-framework), which contains the general information of the framework, including architecture and design information.
It also acts as the umbrella repository for 5 other repositories that map with each of the main components of the of the `MAPE-K` loop, as follows:
* [**M**onitor](https://github.com/eubr-atmosphere/tma-framework-m)
* [**A**nalyze](https://github.com/eubr-atmosphere/tma-framework-a)
* [**P**lanning](https://github.com/eubr-atmosphere/tma-framework-p)
* [**E**xecute](https://github.com/eubr-atmosphere/tma-framework-e)
* [**K**nowledge](https://github.com/eubr-atmosphere/tma-framework-k)

Each repository maintains its own issues and projects, while the [umbrella project](https://github.com/eubr-atmosphere/tma-framework) only manages general issues that affect more than one component.



***

## Usage instructions:

Specific tutorial containing usage instructions for parts of the platform will be included here.
However, this is still under development.

* [Integrate TMA Monitor Client in your Java Probe](https://github.com/eubr-atmosphere/tma-framework-m/tree/master/development/libraries/java-client-lib)
* [Integrate TMA Monitor Client in your Python Probe](https://github.com/eubr-atmosphere/tma-framework-m/tree/master/development/libraries/python-client-lib)
* [Integrate TMA Monitor Client in your C# Probe](https://github.com/eubr-atmosphere/tma-framework-m/tree/master/development/libraries/cs-client-lib)
* [Deploy TMA Monitor in Kubernetes](https://github.com/eubr-atmosphere/tma-framework-m/tree/master/development/server)
* [Deploy TMA Planning in Kubernetes](https://github.com/eubr-atmosphere/tma-framework-p/tree/master/development)
* [Deploy TMA Execute in Kubernetes](https://github.com/eubr-atmosphere/tma-framework-e/tree/master/development/executor)
* [Deploy TMA Knowledge in Kubernetes](https://github.com/eubr-atmosphere/tma-framework-k/tree/master/development)

