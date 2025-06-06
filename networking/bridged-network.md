# Bridged Network

This exercise requires administrator privildge, you cannot carry it out on University laboratory computers.

1. In VMWare Workstation, set your Client VM to connect to the bridged LAN, this is normally VMNet0.
2. Start the Client VM and let it boot.
3. Use **ip a** to identify your IP address.

Draw the network from the perspective of the GUI VM; What can you connect to?

Note that the bridged only network can cause disruption on the host’s LAN and you should not use it without first discussing with your lecturer. If you have more than one network card, you can have more than one bridged network.

<figure><img src="https://johnoraw.gitbook.io/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2Fy9wLtYbbKRlZNsu2a7G7%2Fblobs%2FP4WxgY9SL2UQRpGpRmwX%2Fimage.png&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=f5884225&#x26;sv=2" alt=""><figcaption><p>Fig. 2 The network configuration on my laptop</p></figcaption></figure>

In Fig 2., I manually set vmnet0 to a built-in network card. I then created a new vmnet2 and manually bridged it to a separate network card. I can select either vmnet in each of my VMs, or I can add a virtual network adapter and use both.
