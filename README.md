# ansible_tutorial
There has been a change in this file in the Workstation VM.

The .cfg file contains the inventory file we need to use for the demo. It also has the location of the private SSH key we created for our Ansible server to connect to host machines via SSH. The SSH keys have already been copied to each of the host specified in the inventory file and an initial connection has been made.

The connectivity to all hosts can be verified by running the command: "ansible all -m ping" in the working directory. This fetches the result and the connectivity can be ensured. The "all" denotes we need to run the command against all hosts, "-m" denotes module of the ansible package and "ping" is the module name that pings each of the host.
