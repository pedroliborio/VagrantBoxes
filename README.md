# VagrantBoxes
Vagrant files to provision the phd-vm, Debian 9.12 (stretch), with all pre-requisites to run a ns3 project. The idea is to have a ready OOTB VM just runninng the 'vagrant up' command.

Requirements:
<ol>
  <li>Install virtual box and virtual box extensions pack - https://www.virtualbox.org/wiki/Downloads<li>
  <li>Install Vagrant: https://www.vagrantup.com/<li>
</ol>

In the basebox folder:
<ol>
  <li>Clone repo</li>
  <li>In the basebox folder create the basebox typing:<code>vagrant up</code></li>
  <li>After finish creation of the basebox VM, create a local package:<code>vagrant package --output basebox.box</code></li>
  <li>In the phd-vm folder type: <code>vagrant up</code></li>
  <li>For now on to access the VM you need only to type: <code>vagrant up</code> followed by <code>vagrant ssh</code></li>
</ol>

Notes:
By default the Vagrantfile create synced folder located at /vagrant in the VM. This folder is mapped to the phd-vm folder. 
Take a look on the vagrant file comments to understand the meaning of each command. Enjoy ;)
