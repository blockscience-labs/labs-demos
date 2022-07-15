# Executing your Model & Generating Data
There are several different options for executing your cadCAD models on the Labs platform, each providing benefit for specific use cases.

## Distributed Execution via Labs
For this method of model execution, some preparation needs to be performed. Namely, we will need to provide the platform with an "entry point" into your model so that we can hook into it and accurately break down the model into independent "jobs" that can be distributed across our execution cluster for concurrent execution.

To do this, we first require a `labs.py` file to be added to the root directory of your projects Git repo. Second, we highly recommend adding a human readable model ID or name to each configuration that was added to your cadCAD experiment object.

See [Labs Conversion Checklist](docs/labs-conversion-checklist.md).

## Distributed Execution via Local
You can run your model on our execution cluster from your local environment by way of our SDK.

## JupyterLab Server Execution
You can use your JupyterLab server instance to run cadCAD models directly as you would locally.