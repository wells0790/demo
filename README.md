# vagrantbox
A project for using vagrant with VirtualBox on Mac OS X

=== Pre-requisites
This simple project assumes you already have git and ansible installed on
Mac OS X.  If you downloaded this file using means other than git, try running
"git" at the terminal's bash prompt to see if it displays a version or if it
offers to install xcode (Apple includes git with xcode).  Install xcode if it
isn't installed already.

To install ansible, follow the instructions on their web site.  As of this
writting, installing ansible on Mac OS X is a matter of running these commands:

  sudo easy_install pip
  sudo pip install ansible

=== Bootstrapping the VirtualBox environment
Use ansible to install VirtualBox, vagrant, and other support files.

  ansible-playbook vagrantbox-setup.yml
