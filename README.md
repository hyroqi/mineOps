# This is MineOps

This is a project i did to learn the basic uses of **Ansible** , and to provide myself a "one-liner" code that i can use to install and run a minecraft server on any archlinux machine.


# Content
There are 2 folders, **Manual** is what i used for testing, and **Ansible** contains the playbook in which to use for the "one-liner" install script.

## Manual

To run manual, you just have to run **"java -jar -Xmx{MaxRAM} -Xms{MinRAM} -jar server.jar nogui"** in the CLI, replace the {value} after Xmx and Xms with RAM values to specify the max and minimum amount of ram used respectively. *e.g. -Xmx1024M -Xms 1024M*

## Ansible
To run the Ansible playbook locally, invoke it with **ansible-playbook ansible/minecraftarchinstall.yml** , and it'll automatically install the latest version of server.jar and set a system service to automatically activate the server on reboot, if you want to make changes to how much ram is used, edit the -Xmx and -Xms values in the **ansible/minecraftansible.service file**