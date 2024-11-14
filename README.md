# CloudComputing_PA3

### Scaffolding
The Scaffolding Folder contains the files necessary for the Ansible plays to set up and provision the VMs. It contains the master playbook which can be ran to create the VMs, install the necessary packages, and set the firewall rules. It contains all child playbooks and the structures necessary to provision the Vms.

### P1Files
The P1Files folder contains the enhanced producer logic in order to log response times. It contains details about adding an additional thread that behaves as a consumer to collect end-to-end response times that will help us determine impacts on latency as the number of producers is varied. These results are saved to files for plotting graphs to analyze latency depending on varied workloads.

It also contains the code for the DB Consumer, ML Consumer, and ML Inference server. Additionally, it contains the dockerfiles used to build Docker images on each VM in order to run the files from containers. These are the updated files which contain the changes we made from PA2 in order to get it to work with this data pipeline.

### K8_Deployment
This folder contains the necessary files for the Kubernetes deployment. It specifies the yaml files for the producer and consumers and the configurations for running them.

The final_deployment contain the final files we used to actually deploy the pods. We had to make changes to the original files, so these are the ones we ended up using.
