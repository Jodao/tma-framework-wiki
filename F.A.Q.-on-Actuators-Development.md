An Actuator is software component that is integrated into the cloud that is being monitored by the [TMA Framework](https://github.com/nmsa/tma-framework#trustworthiness-monitoring--assessment-framework). It integrates with `TMA Execute Component` through the interface defined in [here](https://github.com/nmsa/tma-framework-k#message-format-for-actions-registration).

## How does this actuator's thing work?

An actuator contains operations known by the `TMA Framework`, which is responsible to call them when an adaptation is needed according to the quality model and its thresholds.

Some of the Work Packages will create their own actuators. They are:

- **WP4: Cloud services managing Federated and Hybrid resources**: the actuators for this WP will be created in the task T4.3 (Trustworthiness Measurements and Adaptive mechanisms);
- **WP5: Distributed Trustworthy Data Management Services**: the actuators for this WP will be created in the task T5.4 (Trustworthiness Measurements and Adaptation Mechanisms for Data Management);
- **WP6: Trustworthy Data Processing Services**: the actuators for this WP will be created in the task T6.4 (Data Processing Services Trustworthiness Measurement and Adaptation Mechanisms).

In order to perform a secure connection, each actuator should have the Executor component certificate. With it, actuators assure the Executor identity and are able to encrypt all communication with Executor public key, which only allows Executor to decrypt information with its private key.

## How can I create my own actuator?
Instructions to create an actuator in `Java` are [provided here](https://github.com/nmsa/tma-framework-e/tree/master/development/libraries/java-actuator-base).
A demo actuator showing the key features is [available here](https://github.com/nmsa/tma-framework-e/tree/master/development/actuators/demo-actuator-java).

Instructions to create an actuator in `Python` are [provided here](https://github.com/nmsa/tma-framework-e/tree/master/development/libraries/python-actuator-base).
A demo actuator showing the key features is [available here](https://github.com/nmsa/tma-framework-e/tree/master/development/actuators/demo-actuator-python).

## What will be the languages supported?
The executor performs a REST API request; therefore, actuators can be developed in any language.
We provide supporting libraries to make it easier to develop actuators in `Java`.