# Lab-6

## Task - 1

1) systemd-analyze: 
Startup finished in 2.646s (userspace)
graphical.target reached after 2.640s in userspace

2) systemd-analyze blame:
1min 32.252s apt-daily-upgrade.service
     10.050s motd-news.service
       531ms apt-daily.service
       259ms man-db.service
       224ms dev-sdc.device
       182ms networkd-dispatcher.service
       159ms systemd-resolved.service
        69ms systemd-logind.service
        61ms apport.service
        59ms logrotate.service
        58ms systemd-udevd.service
        52ms user@1000.service
        51ms packagekit.service
        50ms e2scrub_reap.service
        44ms systemd-journal-flush.service
        42ms keyboard-setup.service
        42ms snapd.service
        39ms systemd-udev-trigger.service
        30ms systemd-journald.service
        27ms plymouth-read-write.service
        25ms dev-hugepages.mount
        24ms rsyslog.service
        24ms modprobe@configfs.service
        23ms dev-mqueue.mount
        23ms modprobe@drm.service
        23ms modprobe@efi_pstore.service
        22ms sys-kernel-debug.mount
        21ms sys-kernel-tracing.mount
        20ms modprobe@fuse.service
        19ms dev-loop0.device
        18ms systemd-sysusers.service
        18ms snap-bare-5.mount
        16ms plymouth-quit.service
        15ms systemd-tmpfiles-setup-dev.service
        14ms snap-core22-864.mount
        13ms systemd-tmpfiles-setup.service
        12ms snap-gtk\x2dcommon\x2dthemes-1535.mount
        10ms systemd-update-utmp.service
        10ms snap-snapd-20290.mount
         9ms snapd.seeded.service

3) uptime:
19:29:07 up  2:04,  1 user,  load average: 0.00, 0.00, 0.00

4) w:
 19:29:12 up  2:04,  1 user,  load average: 0.00, 0.00, 0.00
USER     TTY      FROM             LOGIN@   IDLE   JCPU   PCPU WHAT
sergey   pts/1    -                17:24    2:04m  0.01s  0.01s -bash

## Task 2

1) traceroute github.com:
traceroute to github.com (140.82.121.3), 30 hops max, 60 byte packets
 1  Sergey.mshome.net (172.27.0.1)  0.246 ms  0.235 ms  0.185 ms
 2  10.248.1.1 (10.248.1.1)  7.477 ms  7.548 ms  7.813 ms
 3  10.250.0.2 (10.250.0.2)  1.167 ms  13.254 ms  1.125 ms
 4  10.252.6.1 (10.252.6.1)  1.594 ms  1.475 ms  1.347 ms
 5  188.170.164.34 (188.170.164.34)  4.601 ms  5.218 ms  5.169 ms
 6  * * *
 7  * * *
 8  * * *
 9  * * *
10  83.169.204.82 (83.169.204.82)  54.763 ms 83.169.204.78 (83.169.204.78)  38.104 ms 83.169.204.82 (83.169.204.82)  41.214 ms
11  netnod-ix-ge-b-sth-1500.inter.link (194.68.128.180)  42.699 ms netnod-ix-ge-a-sth-1500.inter.link (194.68.123.180)  39.997 ms netnod-ix-ge-b-sth-1500.inter.link (194.68.128.180)  40.777 ms
12  r1-cph1-dk.as5405.net (94.103.180.38)  60.691 ms  59.358 ms  59.237 ms
13  r4-ber1-de.as5405.net (94.103.180.3)  79.027 ms  81.974 ms *
14  r3-ber1-de.as5405.net (94.103.180.2)  84.587 ms  84.721 ms  81.678 ms
15  r4-fra1-de.as5405.net (94.103.180.7)  83.822 ms  89.099 ms  79.316 ms
16  r3-fra1-de.as5405.net (94.103.180.6)  82.812 ms  82.097 ms  79.987 ms
17  r3-fra3-de.as5405.net (94.103.180.54)  116.789 ms  100.136 ms  98.937 ms
18  r1-fra3-de.as5405.net (94.103.180.24)  87.736 ms  87.467 ms  86.820 ms
19  cust-sid435.r1-fra3-de.as5405.net (45.153.82.39)  84.379 ms  84.374 ms  84.370 ms
20  * * *
21  * * *
22  * * *
23  * * *
24  * * *
25  * * *
26  * * *
27  * * *
28  * * *
29  * * *
30  * * *

2) dig github.com:

; <<>> DiG 9.18.28-0ubuntu0.22.04.1-Ubuntu <<>> github.com
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 52289
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
;; QUESTION SECTION:
;github.com.                    IN      A

;; ANSWER SECTION:
github.com.             31      IN      A       140.82.121.4

;; Query time: 0 msec
;; SERVER: 10.255.255.254#53(10.255.255.254) (UDP)
;; WHEN: Mon Sep 16 19:37:29 MSK 2024
;; MSG SIZE  rcvd: 55
