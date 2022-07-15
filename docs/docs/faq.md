# BlockScience Labs: Frequently Asked Questions

## How are my simulations executed on the Labs platform?
Simulations are distributed over a cluster to be executed concurrently by their respective monte carlo runs. If your model is configured for a single run, distribution over the cluster will not necessarily improve your execution time when compared to your local environment. However, as more monte carlo runs are configured, the better your overall execution time will be as each run is executed along side the others rather than being run sequentially.

## What is simulation execution time?
Simulation execution time is the time the simulation took to complete, inclusive of all monte carlo runs. Because monte carlo runs are not necessarily scheduled at the exact same moment, simulation execution time is the period of time between the first monte carlo run starting and the last monte carlo run finishing. This metric is NOT the sum of all monte carlo run times.

## What version(s) of cadCAD is/are supported?
Currently, BlockScience Labs only supports cadCAD v0.4.27 or newer.

## Can the cadCAD CLI be used to scaffold a Labs-ready project?
Yes! At the moment, the CLI ships with a template called labs that can be used to scaffold a mid-complexity Labs-ready project.

## How do I work with the data results of my simulation?
After a simulation completes, you will see an option to download the results in CSV form. These results can be imported and converted to a Pandas DataFrame easily by using the BlockScience Labs SDK. Example usage can be found in the cadCAD CLI labs template mentioned above.

## Help! I'm running out of resources on my JupyterLab instance -- what can I do?
Notebook resources are currently fixed but we are very interested in hearing from those who need more! Please contact us at support@blocksciencelabs.com to talk more about how we can accommodate.