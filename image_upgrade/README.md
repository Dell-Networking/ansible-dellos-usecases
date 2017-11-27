==========================================================================
Use Ansible to install or upgrade devices running Dell EMC Networking OS10
==========================================================================

This example explains how to use Ansible to install or upgrade the software image on a device running Dell EMC Networking OS10. The example playbook uses the *dellos-image-upgrade* role to upgrade or install an OS10 image on a specified switch. Before using Ansible to install the software image, you must download the software image via FTP/TFTP/SCP/HTTPDS, then specify the path to the image in the playbook. 

The *dellos-image-upgrade* role uses the ``dellos10_command`` to install or upgrade the switch, then and ``wait_for`` is used to identify the progress of the upgrade operation. Validation of the upgrade operation is handled using the ``dellos10_facts`` module.
