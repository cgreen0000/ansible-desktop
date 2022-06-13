# ansible-desktop
Ansible playbook and roles for configuring desktop workstations. I use this for learning Ansible, managing my Linux desktops, and testing changes in VMs. It is unlikely you will want to run this as-is and you will likely want to modify it quite a bit to fit your needs.

The playbook and roles in this repo are functional but they are in a messy state. I'm currently in the process of splitting what was a single role into several smaller roles. Most of the conditional checks need to be moved out of individual tasks and into the main.yml of the individual roles. This is especially true for the conditionals that check variables.

The playbook currently targets the gnome desktop environment and the following distros:
- Arch Linux
- Fedora
- Ubuntu

Future plans include targeting other desktop environments such as KDE Plasma and targeting Windows workstations.