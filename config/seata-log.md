[root@lavm-k3gi2y76q2 docker-app]# ls -la ./seata/
total 44
drwxr-xr-x 5 root root 4096 Sep 26 15:57 .
drwxr-xr-x 6 root root 4096 Sep 26 15:41 ..
-rw-r--r-- 1 root root 3842 Sep 26 15:57 application.example.yml
-rw-r--r-- 1 root root 3299 Sep 26 15:57 application.yml
-rw-r--r-- 1 root root  664 Sep 26 15:57 banner.txt
drwxr-xr-x 2 root root 4096 Sep 26 15:57 logback
-rw-r--r-- 1 root root 2602 Sep 26 15:57 logback-spring.xml
drwxr-xr-x 3 root root 4096 Sep 26 15:57 lua
drwxr-xr-x 3 root root 4096 Sep 26 15:57 META-INF
-rw-r--r-- 1 root root 1406 Sep 26 15:57 README.md
-rw-r--r-- 1 root root 1400 Sep 26 15:57 README-zh.md
[root@lavm-k3gi2y76q2 docker-app]# docker logs leadnews_seata --tail=100
Slab:              93116 kB
SReclaimable:      59400 kB
SUnreclaim:        33716 kB
KernelStack:        7792 kB
PageTables:         6996 kB
NFS_Unstable:          0 kB
Bounce:                0 kB
WritebackTmp:          0 kB
CommitLimit:     1006996 kB
Committed_AS:    2762212 kB
VmallocTotal:   34359738367 kB
VmallocUsed:       18244 kB
VmallocChunk:          0 kB
Percpu:             1232 kB
HardwareCorrupted:     0 kB
AnonHugePages:    442368 kB
ShmemHugePages:        0 kB
ShmemPmdMapped:        0 kB
FileHugePages:         0 kB
FilePmdMapped:         0 kB
CmaTotal:              0 kB
CmaFree:               0 kB
HugePages_Total:       0
HugePages_Free:        0
HugePages_Rsvd:        0
HugePages_Surp:        0
Hugepagesize:       2048 kB
Hugetlb:               0 kB
DirectMap4k:      806756 kB
DirectMap2M:     1290240 kB
DirectMap1G:           0 kB


CPU:total 2 (initial active 2) (1 cores per cpu, 2 threads per core) family 6 model 85 stepping 5, cmov, cx8, fxsr, mmx, sse, sse2, sse3, ssse3, sse4.1, sse4.2, popcnt, avx, avx2, aes, clmul, erms, rtm, 3dnowpref, lzcnt, ht, tsc, bmi1, bmi2, adx

/proc/cpuinfo:
processor       : 0
vendor_id       : GenuineIntel
cpu family      : 6
model           : 85
model name      : Intel(R) Xeon(R) Gold 6267 CPU @ 2.60GHz
stepping        : 5
microcode       : 0x1
cpu MHz         : 2599.998
cache size      : 16384 KB
physical id     : 0
siblings        : 2
core id         : 0
cpu cores       : 1
apicid          : 0
initial apicid  : 0
fpu             : yes
fpu_exception   : yes
cpuid level     : 13
wp              : yes
flags           : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon rep_good nopl xtopology cpuid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single pti ibrs ibpb fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rtm mpx avx512f avx512dq rdseed adx smap clflushopt clwb avx512cd avx512bw avx512vl xsaveopt xsavec xgetbv1 arat
bugs            : cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs taa itlb_multihit
bogomips        : 5199.99
clflush size    : 64
cache_alignment : 64
address sizes   : 46 bits physical, 48 bits virtual
power management:

processor       : 1
vendor_id       : GenuineIntel
cpu family      : 6
model           : 85
model name      : Intel(R) Xeon(R) Gold 6267 CPU @ 2.60GHz
stepping        : 5
microcode       : 0x1
cpu MHz         : 2599.998
cache size      : 16384 KB
physical id     : 0
siblings        : 2
core id         : 0
cpu cores       : 1
apicid          : 1
initial apicid  : 1
fpu             : yes
fpu_exception   : yes
cpuid level     : 13
wp              : yes
flags           : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc arch_perfmon rep_good nopl xtopology cpuid tsc_known_freq pni pclmulqdq ssse3 fma cx16 pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave avx f16c rdrand hypervisor lahf_lm abm 3dnowprefetch invpcid_single pti ibrs ibpb fsgsbase tsc_adjust bmi1 hle avx2 smep bmi2 erms invpcid rtm mpx avx512f avx512dq rdseed adx smap clflushopt clwb avx512cd avx512bw avx512vl xsaveopt xsavec xgetbv1 arat
bugs            : cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs taa itlb_multihit
bogomips        : 5199.99
clflush size    : 64
cache_alignment : 64
address sizes   : 46 bits physical, 48 bits virtual
power management:



Memory: 4k page, physical 2013992k(70740k free), swap 0k(0k free)

vm_info: OpenJDK 64-Bit Server VM (25.342-b07) for linux-amd64 JRE (1.8.0_342-b07), built on Jul 16 2022 09:19:19 by "openjdk" with gcc 4.4.7 20120313 (Red Hat 4.4.7-23)

time: Fri Sep 26 16:09:28 2025
timezone: CST
elapsed time: 0.011551 seconds (0d 0h 0m 0s)

[root@lavm-k3gi2y76q2 docker-app]#