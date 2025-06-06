# Host Only Network

1. Go to the tab **Edit->Virtual Network Editor**.
2. Create two new host-only networks without DHCP but with host connectivity as VMNet2 and VMNet3.
3. Document and sketch these networks as before.
4. Make sure your server VM is powered down.
   1. Create a linked clone of the server VM.
   2. Add a second network card to this clone and connect it to VMNet2.&#x20;
   3. Start the server clone.&#x20;
   4. Verify and confirm the configuration of the new NIC.
      1. What connectivity do you have from this NIC?
      2. Give it an appropriate IP address with a last octet of .103
5. Make sure your Desktop VM is powered down.
   1. Create a linked clone of the desktop VM.
   2. Change its network setting connect to VMNet2.
   3. Start the desktop VM and give it a valid IP address for VMNet2 with a last octet of .51
   4. Can you ping the server VM interface on VMNet2?&#x20;
   5. Can you ping the host interface on VMNet2?
   6. Can you ping the host interface on the physical LAN?

Now set the network interface on your client VM to DHCP and shut both clone VMs down.
