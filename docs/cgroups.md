<details>
	<summary>
		_____ of memory cgroups trigger an Out-of-Memory killer inside them. A process will get killed when it goes above them.
	</summary>
		Hard limits
</details>

<details>
	<summary>
		Can cgroups limit I/O devices/operations usable by a process? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Can cgroups limit network bandwidth usable by a process? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		The file /proc/[pid]/cgroup contains the process's _____
	</summary>
		enclosing control group
</details>

<details>
	<summary>
		_____ allow you to set resource limits on processes and their children.
	</summary>
		cgroups
</details>

<details>
	<summary>
		_____ cgroup limits are not enforced.
	</summary>
		soft
</details>

<details>
	<summary>
		The _____ (crowd control) cgroup allows to freeze/thaw a group of processes, much like it is done by SIGSTOP signals. Unlike signals however, it CANNOT be detected by the processes. This is useful for cluster batch scheduling and process migration. Doesn't impede ptrace/debugging.
	</summary>
		freezer
</details>

<details>
	<summary>
		Can cgroups limit memory usable by a process? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Each cgroup can have its own _____ or hard limits
	</summary>
		soft
</details>

<details>
	<summary>
		The _____ cgroup controls what a group can do what on device nodes (read/write/mknod permissions etc). You can do it on /dev/net/tun, /dev/fuse, /dev/kvm, /dev/dri so you can have network interface manipulation, filesystems in user space, VMs and GPUs inside containers. Example: allow /dev/xxxx deny everything else
	</summary>
		device
</details>

<details>
	<summary>
		"The _____ cgroup keeps track of pages used by each group. Each page is """"charged"""" to a group and can be shared across groups. file (read/write/mmap from block devices) anonymous (stack, heap, anonymous mmap) active (recently accessed) inactive (candidate for eviction)"""
	</summary>
		memory
</details>

<details>
	<summary>
		_____ allow limiting the amount of resources usable by a process.
	</summary>
		cgroups
</details>

<details>
	<summary>
		When processes inside a Linux system are running out of memory, lower priority processes might be randomly killed by the kernel to free memory up. A _____ cgroup ensures that whenever a process inside it is running out of memory, only the processes inside that cgroup will be up for deletion in such a situation - never the ones outside it.
	</summary>
		memory
</details>

<details>
	<summary>
		Can a CPU cgroup set CPU weights? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		_____ cgroups pin groups of processes to a specific cpu or reserve cpus to specific apps, preventing processes from switching around CPUs.
	</summary>
		cpuset
</details>

<details>
	<summary>
		A _____ cgroup keeps track of user system cpu time, and usage per cpu.
	</summary>
		CPU
</details>

<details>
	<summary>
		The file _____ contains the process's enclosing control group
	</summary>
		/proc/[pid]/cgroup
</details>

<details>
	<summary>
		Do cgroups limit the resources a process can use (in quantity)? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		The _____ cgroup keeps track of IO for each group. You can set throttle limits and relative weights for each group.
	</summary>
		blkio
</details>

<details>
	<summary>
		_____ cgroups automatically set traffic class or priority for traffic generated by processes in the group. (only works for egress traffic) net_cls will assign traffic to a class (which then has to be matched with iptables)
	</summary>
		net_cls and net_prio
</details>

<details>
	<summary>
		"When a process needs to perform a root-account specific action, but you don't want it to have root account permissions, _____ can be set in order to """"break down"""" the root account into multiple fine-grained permissions."""
	</summary>
		capabilities Nevertheless, the CAP_SYS_ADMIN capability cannot be disabled
</details>

<details>
	<summary>
		Linux Containers are usually a combination of _____
	</summary>
		cgroups, namespaces, SELinux, AppArmor
</details>

<details>
	<summary>
		The command _____ can be used to move a process to a cgroup
	</summary>
		echo $PID > /sys/fs/cgroup/.../tasks
</details>

<details>
	<summary>
		The command echo $PID > /sys/fs/cgroup/.../tasks _____
	</summary>
		can be used to move a process to a cgroup
</details>

<details>
	<summary>
		Each cgroup can have its own soft or _____ limits
	</summary>
		hard
</details>

<details>
	<summary>
		Can you make a cgroup limit any kind of memory? (e.g. physical, kernel, total memory...) _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Can cgroups limit CPU time usable by a process? _____
	</summary>
		Yes
</details>

<details>
	<summary>
		Each cgroup can have its own soft or hard _____
	</summary>
		limits
</details>

<details>
	<summary>
		Can a CPU cgroup set CPU limits? _____
	</summary>
		No
</details>

<details>
	<summary>
		PID 1 is placed at the root of each cgroup. Are its children created inside the parent's groups? _____
	</summary>
		Yes
</details>

