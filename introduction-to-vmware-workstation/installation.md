# Installation

Installation used to be download and run the installer...not any more.

1. Finding a source of the installer is the first challenge. At time of writing you need to register for an account from Broadcom, then you download and install.
2. When you run for the first time, you select to that the license is for personal use, everything should work.

Now the real pain often starts.

Firstly Microsoft and VMWare don't play well together. If you have anything that uses Hyper-V or Docker already installed, then things may not work. Do some background reading on the problem and decide if its an issue for you.

## Nested Virtualization&#x20;

If you want to run Docker or Hyper-V in a VM (we will!) then you need nested virtualization. This is where VMWare can host an OS which also provides virtualization.

To test if this is working, create a VM and tick the box to enable nested virtualization.&#x20;

<p align="center"> <img src="../.gitbook/assets/Screenshot 2025-06-25 233411.png" alt=""></p>

On most new systems, when I try to run this VM, this fails!&#x20;

### The fix

I now run the following from the command line.

```
bcdedit /set hypervisorlaunchtype off
```

I also ran **gpedit,** the policy editor.

<figure><img src="../.gitbook/assets/Screenshot 2025-06-25 232657.png" alt=""><figcaption></figcaption></figure>

I had to turn off security to make nested virtualization work.

Then I do a reboot and test again.
