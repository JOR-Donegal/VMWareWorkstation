# Linked clone

Make a linked clone of the existing client VM.

Check how long it takes

Examine the disk files afterwards, for both the parent and child VM.

Call the new VM <mark style="color:red;">OS</mark>-<mark style="color:blue;">L00xxxxxx-</mark><mark style="color:green;">Date</mark> where;

* <mark style="color:red;">OS</mark> is the OS type, for example UB2404
* <mark style="color:blue;">L00xxxxxx</mark> is your L number
* <mark style="color:green;">Date</mark> is todays date.

Linked clones are normally ephemeral, putting a date on is a useful note to yourself that this can be deleted once used.

Restart and test the parent and child VMs.

* Can they all use the network?
* Check the MAC address of the network card on both.
* Are they the same?

You should be able to draw some conclusions as to the comparative efficiency and application of full and linked clones.

Delete the linked clone and clean up as you are finished.
