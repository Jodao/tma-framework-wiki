# Deployment of TMA Monitor
To deploy a testing mode of TMA Monitor, the first step is to deploy all components of TMA Monitor. To do that you should follow the instructions presented in the page that explains how to [Deploy TMA Monitor in kubernetes](Deploy-TMA-Monitor-in-Kubernetes).

# Testing

In order to verify TMA Monitor is ready to start serving and running properly, you can a use a test script. For that you should follow these [instructions](https://github.com/nmsa/tma-framework-m/blob/master/development/server/README.md#testing). Before you run the script mentioned in those instructions, make sure the certificate in that folder, the file `cert.pem`, is the same as the one used by monitor. Making sure to use the same certificate will enable communication between the parts and thus avoid an unexpected output.
