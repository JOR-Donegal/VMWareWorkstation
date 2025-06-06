# NAT’d Network

We cover NAT in detail in the network module, for now, do some background reading and at least understand the basics.

The default for any installation is for new VMs to be NAT’d to the outside network. Can you explain the advantages of this configuration?

1. Connect your client VM to the NAT network
   1. Boot your client VM and reconnoiter the NAT network.
   2. Check the client VM’s network card. It should have been connected to the NAT VLAN by default. Confirm this is the case.
   3. Using **traceroute** and **ping**, identify the network topology from your VM to the internet and ensure you can sketch it out. You may have to install traceroute!
   4. Can the host computer ping the client VM? How?
2. Shutdown your client VM. Always shut down from the operating system itself!
