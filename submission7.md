# Lab-6

## Task - 1

1)VirtualBox version number - 7.10

2) download iso file, and create VM
3) ![img.png](img.png)

## Task 2

1) ubuntu@ubuntu:~$ lscpu
Architecture:             x86_64
CPU op-mode(s):         32-bit, 64-bit
Address sizes:          39 bits physical, 48 bits virtual
Byte Order:             Little Endian
CPU(s):                   6
On-line CPU(s) list:    0-5
Vendor ID:                GenuineIntel
Model name:             11th Gen Intel(R) Core(TM) i5-11400H
@ 2.70GHz
CPU family:           6
Model:                141
Thread(s) per core:   1
Core(s) per socket:   6
Socket(s):            1
Stepping:             1
BogoMIPS:             5375.99
Flags:                fpu vme de pse tsc msr pae mce cx8 a
pic sep mtrr pge mca cmov pat pse36
clflush mmx fxsr sse sse2 ht syscall
nx rdtscp lm constant_tsc rep_good
nopl xtopology nonstop_tsc cpuid tsc
_known_freq pni pclmulqdq ssse3 cx16
pcid sse4_1 sse4_2 movbe popcnt aes
rdrand hypervisor lahf_lm abm 3dnow
prefetch ibrs_enhanced fsgsbase bmi1
bmi2 invpcid rdseed adx clflushopt
sha_ni arat md_clear flush_l1d arch_
capabilities
Virtualization features:  
Hypervisor vendor:      KVM
Virtualization type:    full
Caches (sum of all):      
L1d:                    288 KiB (6 instances)
L1i:                    192 KiB (6 instances)
L2:                     7.5 MiB (6 instances)
L3:                     72 MiB (6 instances)
NUMA:                     
NUMA node(s):           1
NUMA node0 CPU(s):      0-5
Vulnerabilities:          
Gather data sampling:   Not affected
Itlb multihit:          Not affected
L1tf:                   Not affected
Mds:                    Not affected
Meltdown:               Not affected
Mmio stale data:        Not affected
Reg file data sampling: Not affected
Retbleed:               Mitigation; Enhanced IBRS
Spec rstack overflow:   Not affected
Spec store bypass:      Vulnerable
Spectre v1:             Mitigation; usercopy/swapgs barriers
and __user pointer sanitization
Spectre v2:             Mitigation; Enhanced / Automatic IBR
S; RSB filling; PBRSB-eIBRS SW seque
nce; BHI SW loop, KVM SW loop
Srbds:                  Not affected
Tsx async abort:        Not affected

2) ubuntu@ubuntu:~$ vmstat
procs -----------memory---------- ---swap-- -----io---- -system-- -------cpu-------
r  b   swpd   free   buff  cache   si   so    bi    bo   in   cs us sy id wa st gu
3  0      0 124776  11948 6684240    0    0 22078     4 6740   14 15 17 67  2  0  0
3) ubuntu@ubuntu:~$ ifconfig
Command 'ifconfig' not found, but can be installed with:
sudo apt install net-tools
ubuntu@ubuntu:~$ ^C
ubuntu@ubuntu:~$ sudo apt install net-tools
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following NEW packages will be installed:
net-tools
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 204 kB of archives.
After this operation, 811 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu noble/main amd64 net-tools amd64 2.10-0.1ubuntu4 [204 kB]
Fetched 204 kB in 22s (9,402 B/s)  
Selecting previously unselected package net-tools.
(Reading database ... 210856 files and directories currently installed.)
Preparing to unpack .../net-tools_2.10-0.1ubuntu4_amd64.deb ..
.
Unpacking net-tools (2.10-0.1ubuntu4) ...
Setting up net-tools (2.10-0.1ubuntu4) ...
Processing triggers for man-db (2.12.0-4build2) ...
4) ubuntu@ubuntu:~$ ifconfig
enp0s3: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
inet 10.0.2.15  netmask 255.255.255.0  broadcast 10.0.2.255
inet6 fe80::a00:27ff:fe41:22b0  prefixlen 64  scopeid 0x20<link>
inet6 fd00::a00:27ff:fe41:22b0  prefixlen 64  scopeid 0x0<global>
inet6 fd00::ee:c19c:871a:f6