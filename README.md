# packer-omv
Packer files to build an OMV vagrant .box file

## Prerequisites
* Packer installed (https://www.packer.io/)
* Vagrant installed (https://www.vagrantup.com/)
* VirtualBox installed (https://www.virtualbox.org/)
* If you're on Windows you need Cygwin with ssh and rsyn support (https://www.cygwin.com/)

## Instructions
* Clone the repo
* Download the 3.0.2 beta iso of OMV (https://sourceforge.net/projects/openmediavault/files/3.0beta/) and place it in the same folder as the json file.
* Edit both the json and preseed (in the hhtp folder) files to set up machine specs and language config
* Run "packer build omv-3.2.0.json" and wait for it to complete
* Import the new .box file into Vagrant
