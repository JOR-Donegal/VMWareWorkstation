# Installation

Installation used to be download and run the installer...not any more.

1. Finding a source of the installer is the first challenge. At time of writing you need to register for an account from Broadcom, then you download and install.
2. When you run for the first time, you select to that the license is for persoanl use, everything should work.

Now the real pain often starts.

Firstly Microsoft and VMWare don't play well together. If you have anything that uses Hyper-V or Docker already installed, then things may not work. Do some background reading on the problem and decide if its an issue for you.

&#x20;On most new systems, I now run the following from the command line.

```
bcdedit /set hypervisorlaunchtype off
```

Then I do a reboot.

I also ran **gpedit,** the policy editor.

