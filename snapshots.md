# Snapshots

A snapshot (the term is taken from photography) is the ability to take a copy of the state of a system at a definite point in time. In most cases an actual copy is not taken, the management system uses clever mechanisms to track changes which expose the snapshot functionality; it looks like there is a copy, there isn’t!

Databases and file systems may have the capability to support snapshots and most enterprise storage environments do.

One of the most useful features exposed by a virtual environment is the ability to take snapshots. Taking a snapshot of a virtual machine saves its current state and enables you to return to the same state repeatedly. When you take a snapshot, Workstation captures the entire state of the virtual machine. You can use the snapshot manager to review and act on the snapshots for an active virtual machine.

Note that this process is not fool proof. Suppose you snapshot a VM when it is in the middle of a transaction. If you then revert to that snapshot at a later time, the VM may not be consistent with whatever happened during the transaction. It is best to take snapshots of a VM which is shut down and also it is best to use snapshots with VMs that do not keep state. Taking snapshots of a live database server could cause issues!

We will commonly use this functionality before doing updates, or installing software, or when any event is imminent which might threaten the integrity of the VM. Although we can make multiple levels of snapshot, we rarely do. We also keep our snapshots short-lived. This is because of performance implications. In this practical, you will take, revert and delete snapshots.

## Exercise <a href="#exercise" id="exercise"></a>

Download “Using VMware Workstation for VMware Workstation X” from the VMWare site.

Review the section “Taking Snapshots of Virtual Machines”.

Clearly understand all the actions documented.

* Using Snapshots to preserve virtual machine states
* Using the Snapshot Manager
* Take a Snapshot of a Virtual Machine
* Revert to a Snapshot
* Deleting a Snapshot

List the files in the VM directory before taking a snapshot

Using your VM, exercise the above listed functions and test. During this process, check to see what file types are created, what size they are and whether they are deleted once you finish with the snapshots. Identify each file type and its extension.

## Testing <a href="#testing" id="testing"></a>

You should show that you have completed and tested the five specified topics. You should be able to draw some conclusions as to the application of this technique, where it might be used, duration, etc. Your records should demonstrate that you;

1. Fully understand the implications of snapshots.
2. You understand their application, where and when to use them.
3. Know the file types to expect while you have live snapshots, before and after.
