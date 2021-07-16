# ansible_tutorial
There has been a change in this file in the Workstation VM.

The .cfg file contains the inventory file we need to use for the demo. It also has the location of the private SSH key we created for our Ansible server to connect to host machines via SSH. The SSH keys have already been copied to each of the host specified in the inventory file and an initial connection has been made.

The connectivity to all hosts can be verified by running the command: "ansible all -m ping" in the working directory. This fetches the result and the connectivity can be ensured. The "all" denotes we need to run the command against all hosts, "-m" denotes module of the ansible package and "ping" is the module name that pings each of the host.

In this demo I cloned this repository in my WorkstationVM using the git clone command. The series of guides that I followed to do these tasks are at this link: https://www.youtube.com/playlist?list=PLT98CRl2KxKEUHie1m24-wkyHpEsa4Y70

The repo has plabooks with explanations added in each playbook. The steps to setup the VM infrastructure as well as installing Ansible is in the documenations submitted with this repo.

We run an ansible playbook using the command "ansible-playbook --ask-become-pass example.yml". The --ask-become-pass asks us the sudo passsword for the host amchines so that we connect to them as sudo users to run the various taks that require that level of privilege.

Refer to the files in following order:

1. inventory
2. ansible.cfg
3. remove_apache.yml and install-apche.yml to compare the diffrences between two.
4. site.yml for the copy module.
5. run_shell.yml for shell module
6. run_shell_git.yml to run a script on a host machine that is stored in a git repo. 

The repo also has VirtualBox_Documenation.pdf that describes how to setup VMs for this demo as well as the Ansible_Documenation.pdf that explains setting up SSH keys for Ansible and installing Ansible on the WorksationVM. 
