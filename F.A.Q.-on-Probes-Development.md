A Probe is software component that is integrated in the cloud that is being monitored by the [TMA Framework](https://github.com/nmsa/tma-framework#trustworthiness-monitoring--assessment-framework). It integrates with `TMA Monitor Component` through the interface defined in [here](https://github.com/nmsa/tma-framework-m#tma-monitor-message-format).

## How does this probe's thing work?

A probe provides the raw data to the `TMA Framework`, which is responsible to calculate the metrics according to the quality model, and defines actions to potentially adapt the system under adaptation.

Some of the Work Packages will create their own probes. They are:

- **WP4: Cloud services managing Federated and Hybrid resources**: the probes for this WP will be created in the task T4.3 (Trustworthiness Measurements and Adaptive mechanisms);
- **WP5: Distributed Trustworthy Data Management Services**: the probes for this WP will be created in the task T5.4 (Trustworthiness Measurements and Adaptation Mechanisms for Data Management);
- **WP6: Trustworthy Data Processing Services**: the probes for this WP will be created in the task T6.4 (Data Processing Services Trustworthiness Measurement and Adaptation Mechanisms).

In order to perform a secure connection, each probe should have the certificate from Monitor component. With this certificate, probes assure the Monitor identity and are able to encrypt all communication with Monitor public key, which only allows Monitor to decrypt information with its private key.

## How can I create my own probe?

Instructions to create a probe in `Java` are [provided here](https://github.com/nmsa/tma-framework-m/tree/master/development/libraries/java-client-lib).
A demo probe showing the key features is [available here](https://github.com/nmsa/tma-framework-m/tree/master/development/probes/probe-java-demo).

Instructions to create a probe in `Python` are [provided here](https://github.com/nmsa/tma-framework-m/tree/master/development/libraries/python-client-lib).
A demo probe showing the key features is [available here](https://github.com/nmsa/tma-framework-m/tree/master/development/probes/probe-python-demo)

Instructions to create a probe in C# are [provided here](https://github.com/nmsa/tma-framework-m/tree/master/development/libraries/cs-client-lib).
A demo probe showing the key features is [available here](https://github.com/nmsa/tma-framework-m/tree/master/development/probes/probe-cs-demo)

## What will be the languages supported?
The monitor provides a REST API, therefore probes can be developed in any language.
We provide supporting libraries to make it easier to develop probes in `Java`, `Python` and `C#`.