Welcome to Ubuntu 26.04 LTS (GNU/Linux 7.0.0-22-generic x86_64)

 * Documentation:  https://docs.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro

This system has been minimized by removing packages and content that are
not required on a system that users do not log into.

To restore this content, you can run the 'unminimize' command.
root@my:~# sudo apt update -y && sudo apt install -y curl && bash <(curl -Ls https://raw.githubusercontent.com/MHSanaei/3x-ui/master/install.sh)
Get:1 http://security.ubuntu.com/ubuntu resolute-security InRelease [137 kB]
Hit:2 http://archive.ubuntu.com/ubuntu resolute InRelease
Get:3 http://archive.ubuntu.com/ubuntu resolute-updates InRelease [137 kB]
Get:4 http://archive.ubuntu.com/ubuntu resolute-backports InRelease [137 kB]
Get:5 http://security.ubuntu.com/ubuntu resolute-security/main amd64 Packages [526 kB]
Get:6 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 Packages [674 kB]
Get:7 http://archive.ubuntu.com/ubuntu resolute-updates/main Translation-en [159 kB]
Get:8 http://security.ubuntu.com/ubuntu resolute-security/main Translation-en [123 kB]
Get:9 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 Components [97.8 kB]             
Get:10 http://security.ubuntu.com/ubuntu resolute-security/main amd64 Components [46.7 kB]          
Get:11 http://archive.ubuntu.com/ubuntu resolute-updates/restricted amd64 Packages [457 kB]                  
Get:12 http://security.ubuntu.com/ubuntu resolute-security/restricted amd64 Packages [437 kB]
Get:13 http://archive.ubuntu.com/ubuntu resolute-updates/restricted Translation-en [90.8 kB]
Get:14 http://security.ubuntu.com/ubuntu resolute-security/restricted Translation-en [86.2 kB]
Get:15 http://security.ubuntu.com/ubuntu resolute-security/universe amd64 Packages [177 kB]               
Get:16 http://archive.ubuntu.com/ubuntu resolute-updates/universe amd64 Packages [302 kB]
Get:17 http://security.ubuntu.com/ubuntu resolute-security/universe Translation-en [56.3 kB]
Get:18 http://security.ubuntu.com/ubuntu resolute-security/universe amd64 Components [43.4 kB]
Get:19 http://archive.ubuntu.com/ubuntu resolute-updates/universe Translation-en [96.7 kB]           
Get:20 http://security.ubuntu.com/ubuntu resolute-security/multiverse amd64 Packages [10.8 kB]               
Get:21 http://archive.ubuntu.com/ubuntu resolute-updates/universe amd64 Components [190 kB]                  
Get:22 http://security.ubuntu.com/ubuntu resolute-security/multiverse Translation-en [2844 B]
Get:23 http://archive.ubuntu.com/ubuntu resolute-updates/multiverse amd64 Packages [11.6 kB]
Get:24 http://archive.ubuntu.com/ubuntu resolute-updates/multiverse Translation-en [3172 B]
Get:25 http://archive.ubuntu.com/ubuntu resolute-backports/universe amd64 Packages [3132 B]
Get:26 http://archive.ubuntu.com/ubuntu resolute-backports/universe Translation-en [7988 B]
Get:27 http://archive.ubuntu.com/ubuntu resolute-backports/universe amd64 Components [1056 B]
Fetched 4015 kB in 1s (4801 kB/s)               
157 packages can be upgraded. Run 'apt list --upgradable' to see them.
Upgrading:                      
  curl  libcurl3t64-gnutls  libcurl4t64

Summary:
  Upgrading: 3, Installing: 0, Removing: 0, Not Upgrading: 154
  Download size: 1120 kB
  Space needed: 14.3 kB / 22.0 GB available

Get:1 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 curl amd64 8.18.0-1ubuntu2.7 [272 kB]
Get:2 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libcurl4t64 amd64 8.18.0-1ubuntu2.7 [428 kB]
Get:3 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libcurl3t64-gnutls amd64 8.18.0-1ubuntu2.7 [419 kB]
Fetched 1120 kB in 0s (4705 kB/s)           
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79, <STDIN> line 3.)
debconf: falling back to frontend: Readline
(Reading database ... 125313 files and directories currently installed.)
Preparing to unpack .../curl_8.18.0-1ubuntu2.7_amd64.deb ...
Unpacking curl (8.18.0-1ubuntu2.7) over (8.18.0-1ubuntu2.1) ...
Preparing to unpack .../libcurl4t64_8.18.0-1ubuntu2.7_amd64.deb ...
Unpacking libcurl4t64:amd64 (8.18.0-1ubuntu2.7) over (8.18.0-1ubuntu2.1) ...
Preparing to unpack .../libcurl3t64-gnutls_8.18.0-1ubuntu2.7_amd64.deb ...
Unpacking libcurl3t64-gnutls:amd64 (8.18.0-1ubuntu2.7) over (8.18.0-1ubuntu2.1) ...
Setting up libcurl4t64:amd64 (8.18.0-1ubuntu2.7) ...
Setting up libcurl3t64-gnutls:amd64 (8.18.0-1ubuntu2.7) ...
Setting up curl (8.18.0-1ubuntu2.7) ...
Processing triggers for libc-bin (2.43-2ubuntu2) ...
Scanning processes...                                                                                                                                                                                                                        
Scanning linux images...                                                                                                                                                                                                                     

Running kernel seems to be up-to-date.

No services need to be restarted.

No containers need to be restarted.

No user sessions are running outdated binaries.

No VM guests are running outdated hypervisor (qemu) binaries on this host.
The OS release is: ubuntu
Arch: amd64
Running...
Hit:1 http://archive.ubuntu.com/ubuntu resolute InRelease
Hit:2 http://security.ubuntu.com/ubuntu resolute-security InRelease
Hit:3 http://archive.ubuntu.com/ubuntu resolute-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu resolute-backports InRelease
Reading package lists... Done
Reading package lists...
Building dependency tree...
Reading state information...
curl is already the newest version (8.18.0-1ubuntu2.7).
ca-certificates is already the newest version (20260601~26.04.1).
ca-certificates set to manually installed.
Solving dependencies...
The following additional packages will be installed:
  cron-daemon-common libssl3t64 openssl-provider-legacy
Suggested packages:
  anacron logrotate checksecurity supercat bat default-mta | mail-transport-agent
The following NEW packages will be installed:
  cron cron-daemon-common socat
The following packages will be upgraded:
  libssl3t64 openssl openssl-provider-legacy tar tzdata
5 upgraded, 3 newly installed, 0 to remove and 149 not upgraded.
Need to get 4604 kB of archives.
After this operation, 2062 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 tar amd64 1.35+dfsg-4ubuntu0.4 [258 kB]
Get:2 http://archive.ubuntu.com/ubuntu resolute/main amd64 cron-daemon-common all 3.0pl1-200ubuntu1 [15.7 kB]
Get:3 http://archive.ubuntu.com/ubuntu resolute/main amd64 cron amd64 3.0pl1-200ubuntu1 [88.6 kB]
Get:4 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 openssl-provider-legacy amd64 3.5.5-1ubuntu3.5 [39.7 kB]
Get:5 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libssl3t64 amd64 3.5.5-1ubuntu3.5 [2363 kB]
Get:6 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 openssl amd64 3.5.5-1ubuntu3.5 [1243 kB]
Get:7 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 tzdata all 2026c-0ubuntu0.26.04.1 [193 kB]
Get:8 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 socat amd64 1.8.1.1-1ubuntu0.1 [403 kB]
Fetched 4604 kB in 0s (15.0 MB/s)
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79, <STDIN> line 8.)
debconf: falling back to frontend: Readline
Preconfiguring packages ...
(Reading database ... 125313 files and directories currently installed.)
Preparing to unpack .../tar_1.35+dfsg-4ubuntu0.4_amd64.deb ...
Unpacking tar (1.35+dfsg-4ubuntu0.4) over (1.35+dfsg-4) ...
Setting up tar (1.35+dfsg-4ubuntu0.4) ...
Selecting previously unselected package cron-daemon-common.
(Reading database ... 125313 files and directories currently installed.)
Preparing to unpack .../cron-daemon-common_3.0pl1-200ubuntu1_all.deb ...
Unpacking cron-daemon-common (3.0pl1-200ubuntu1) ...
Setting up cron-daemon-common (3.0pl1-200ubuntu1) ...
Creating group 'crontab' with GID 986.
Selecting previously unselected package cron.
(Reading database ... 125332 files and directories currently installed.)
Preparing to unpack .../cron_3.0pl1-200ubuntu1_amd64.deb ...
Unpacking cron (3.0pl1-200ubuntu1) ...
Preparing to unpack .../openssl-provider-legacy_3.5.5-1ubuntu3.5_amd64.deb ...
Unpacking openssl-provider-legacy (3.5.5-1ubuntu3.5) over (3.5.5-1ubuntu3.2) ...
Setting up openssl-provider-legacy (3.5.5-1ubuntu3.5) ...
(Reading database ... 125361 files and directories currently installed.)
Preparing to unpack .../libssl3t64_3.5.5-1ubuntu3.5_amd64.deb ...
Unpacking libssl3t64:amd64 (3.5.5-1ubuntu3.5) over (3.5.5-1ubuntu3.2) ...
Setting up libssl3t64:amd64 (3.5.5-1ubuntu3.5) ...
(Reading database ... 125361 files and directories currently installed.)
Preparing to unpack .../openssl_3.5.5-1ubuntu3.5_amd64.deb ...
Unpacking openssl (3.5.5-1ubuntu3.5) over (3.5.5-1ubuntu3.2) ...
Preparing to unpack .../tzdata_2026c-0ubuntu0.26.04.1_all.deb ...
Unpacking tzdata (2026c-0ubuntu0.26.04.1) over (2026a-3ubuntu1) ...
Selecting previously unselected package socat.
Preparing to unpack .../socat_1.8.1.1-1ubuntu0.1_amd64.deb ...
Unpacking socat (1.8.1.1-1ubuntu0.1) ...
Setting up cron (3.0pl1-200ubuntu1) ...
Created symlink '/etc/systemd/system/multi-user.target.wants/cron.service' → '/usr/lib/systemd/system/cron.service'.
Setting up tzdata (2026c-0ubuntu0.26.04.1) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline

Current default time zone: 'Etc/UTC'
Local time is now:      Sun Sep 27 07:38:20 UTC 2026.
Universal Time is now:  Sun Sep 27 07:38:20 UTC 2026.
Run 'dpkg-reconfigure tzdata' if you wish to change it.

Setting up socat (1.8.1.1-1ubuntu0.1) ...
Setting up openssl (3.5.5-1ubuntu3.5) ...
Processing triggers for libc-bin (2.43-2ubuntu2) ...
Scanning processes...                                                                                                                                                                                                                        
Scanning candidates...                                                                                                                                                                                                                       
Scanning linux images...                                                                                                                                                                                                                     

Running kernel seems to be up-to-date.

Restarting services...
 /etc/needrestart/restart.d/systemd-manager
 /etc/needrestart/restart.d/systemd-user
 systemctl restart ssh.service systemd-journald.service systemd-udevd.service

Service restarts being deferred:
 systemctl restart networkd-dispatcher.service
 systemctl restart systemd-logind.service
 systemctl restart unattended-upgrades.service

No containers need to be restarted.

User sessions running outdated binaries:
 root @ session #1: sshd-session[1291]
 root @ user manager: (sd-pam)[1300]

No VM guests are running outdated hypervisor (qemu) binaries on this host.
Got x-ui latest version: v3.8.5, beginning the installation...
  % Total    % Received % Xferd  Average Speed  Time    Time    Time   Current
                                 Dload  Upload  Total   Spent   Left   Speed
  0      0   0      0   0      0      0      0                              0
100 78.54M 100 78.54M   0      0 48.59M      0   00:01   00:01         54.75M
Checksum verified: 6a85c110a04a727613c933c54ae602b8d37dab8876c6e20a6d46623010dd9d3c
  % Total    % Received % Xferd  Average Speed  Time    Time    Time   Current
                                 Dload  Upload  Total   Spent   Left   Speed
100 132.4k 100 132.4k   0      0  3.52M      0                              0
x-ui/
x-ui/x-ui.service.debian
x-ui/x-ui
x-ui/x-ui.sh
x-ui/x-ui.service.rhel
x-ui/x-ui.service.arch
x-ui/bin/
x-ui/bin/mtg-linux-amd64
x-ui/bin/xray-linux-amd64
x-ui/bin/geoip_RU.dat
x-ui/bin/geosite.dat
x-ui/bin/geoip.dat
x-ui/bin/geosite_IR.dat
x-ui/bin/geoip_IR.dat
x-ui/bin/README.md
x-ui/bin/geosite_RU.dat
x-ui/bin/LICENSE
x-ui/bin/tuic-server

═══════════════════════════════════════════
     Database Selection                    
═══════════════════════════════════════════
  1) SQLite     (default — recommended for < 500 clients)
  2) PostgreSQL (recommended for high client counts / many nodes)
Choose [1]: 2

  3) Install PostgreSQL locally and create a dedicated user/db (recommended)
  4) Use an existing PostgreSQL server (enter DSN)
Choose [1]: 1
Installing PostgreSQL — this may take a moment...
Hit:1 http://security.ubuntu.com/ubuntu resolute-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu resolute InRelease
Hit:3 http://archive.ubuntu.com/ubuntu resolute-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu resolute-backports InRelease
Reading package lists... Done
Reading package lists...
Building dependency tree...
Reading state information...
Solving dependencies...
The following additional packages will be installed:
  libc-bin libc-dev-bin libc-gconv-modules-extra libc6 libc6-dev libcommon-sense-perl libjson-perl libjson-xs-perl libpq5 libsensors-config libsensors5 libtypes-serialiser-perl libxslt1.1 locales logrotate postgresql-18
  postgresql-18-jit postgresql-client-18 postgresql-client-common postgresql-common ssl-cert sysstat
Suggested packages:
  libpq-oauth lm-sensors bsd-mailx | mailx postgresql-doc postgresql-doc-18 isag
The following NEW packages will be installed:
  libcommon-sense-perl libjson-perl libjson-xs-perl libpq5 libsensors-config libsensors5 libtypes-serialiser-perl libxslt1.1 locales logrotate postgresql postgresql-18 postgresql-18-jit postgresql-client-18 postgresql-client-common
  postgresql-common ssl-cert sysstat
The following packages will be upgraded:
  libc-bin libc-dev-bin libc-gconv-modules-extra libc6 libc6-dev
5 upgraded, 18 newly installed, 0 to remove and 144 not upgraded.
Need to get 29.8 MB of archives.
After this operation, 70.8 MB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libc-dev-bin amd64 2.43-2ubuntu2.4 [23.3 kB]
Get:2 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libc6-dev amd64 2.43-2ubuntu2.4 [2294 kB]
Get:3 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libc-gconv-modules-extra amd64 2.43-2ubuntu2.4 [1362 kB]
Get:4 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libc6 amd64 2.43-2ubuntu2.4 [2104 kB]
Get:5 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libc-bin amd64 2.43-2ubuntu2.4 [701 kB]
Get:6 http://archive.ubuntu.com/ubuntu resolute/main amd64 libjson-perl all 4.10000-1 [81.9 kB]
Get:7 http://archive.ubuntu.com/ubuntu resolute/main amd64 postgresql-client-common all 290ubuntu1 [49.4 kB]
Get:8 http://archive.ubuntu.com/ubuntu resolute/main amd64 ssl-cert all 1.1.3ubuntu2 [18.8 kB]
Get:9 http://archive.ubuntu.com/ubuntu resolute/main amd64 postgresql-common all 290ubuntu1 [101 kB]
Get:10 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 locales all 2.43-2ubuntu2.4 [4225 kB]
Get:11 http://archive.ubuntu.com/ubuntu resolute/main amd64 logrotate amd64 3.22.0-1build1 [53.7 kB]
Get:12 http://archive.ubuntu.com/ubuntu resolute/main amd64 libsensors-config all 1:3.6.2-2build1 [6862 B]
Get:13 http://archive.ubuntu.com/ubuntu resolute/main amd64 libsensors5 amd64 1:3.6.2-2build1 [28.9 kB]
Get:14 http://archive.ubuntu.com/ubuntu resolute/main amd64 sysstat amd64 12.7.7-0ubuntu2 [517 kB]
Get:15 http://archive.ubuntu.com/ubuntu resolute/main amd64 libcommon-sense-perl amd64 3.75-3build5 [20.5 kB]
Get:16 http://archive.ubuntu.com/ubuntu resolute/main amd64 libtypes-serialiser-perl all 1.01-1 [11.6 kB]
Get:17 http://archive.ubuntu.com/ubuntu resolute/main amd64 libjson-xs-perl amd64 4.040-1 [84.4 kB]
Get:18 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 libpq5 amd64 18.6-0ubuntu0.26.04.1 [163 kB]
Get:19 http://archive.ubuntu.com/ubuntu resolute/main amd64 libxslt1.1 amd64 1.1.45-0.1 [165 kB]
Get:20 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 postgresql-client-18 amd64 18.6-0ubuntu0.26.04.1 [1401 kB]
Get:21 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 postgresql-18 amd64 18.6-0ubuntu0.26.04.1 [6002 kB]
Get:22 http://archive.ubuntu.com/ubuntu resolute/main amd64 postgresql all 18+290ubuntu1 [18.6 kB]
Get:23 http://archive.ubuntu.com/ubuntu resolute-updates/main amd64 postgresql-18-jit amd64 18.6-0ubuntu0.26.04.1 [10.4 MB]
Fetched 29.8 MB in 1s (38.5 MB/s)
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79, <STDIN> line 23.)
debconf: falling back to frontend: Readline
Preconfiguring packages ...
/var/cache/debconf/tmp.ci/postgresql.config.Tz6Ryv: 12: pg_lsclusters: not found
(Reading database ... 125404 files and directories currently installed.)
Preparing to unpack .../libc-dev-bin_2.43-2ubuntu2.4_amd64.deb ...
Unpacking libc-dev-bin (2.43-2ubuntu2.4) over (2.43-2ubuntu2) ...
Preparing to unpack .../libc6-dev_2.43-2ubuntu2.4_amd64.deb ...
Unpacking libc6-dev:amd64 (2.43-2ubuntu2.4) over (2.43-2ubuntu2) ...
Preparing to unpack .../libc-gconv-modules-extra_2.43-2ubuntu2.4_amd64.deb ...
Unpacking libc-gconv-modules-extra:amd64 (2.43-2ubuntu2.4) over (2.43-2ubuntu2) ...
Setting up libc-gconv-modules-extra:amd64 (2.43-2ubuntu2.4) ...
(Reading database ... 125404 files and directories currently installed.)
Preparing to unpack .../libc6_2.43-2ubuntu2.4_amd64.deb ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Unpacking libc6:amd64 (2.43-2ubuntu2.4) over (2.43-2ubuntu2) ...
Setting up libc6:amd64 (2.43-2ubuntu2.4) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
(Reading database ... 125404 files and directories currently installed.)
Preparing to unpack .../libc-bin_2.43-2ubuntu2.4_amd64.deb ...
Unpacking libc-bin (2.43-2ubuntu2.4) over (2.43-2ubuntu2) ...
Setting up libc-bin (2.43-2ubuntu2.4) ...
Selecting previously unselected package libjson-perl.
(Reading database ... 125404 files and directories currently installed.)
Preparing to unpack .../00-libjson-perl_4.10000-1_all.deb ...
Unpacking libjson-perl (4.10000-1) ...
Selecting previously unselected package postgresql-client-common.
Preparing to unpack .../01-postgresql-client-common_290ubuntu1_all.deb ...
Unpacking postgresql-client-common (290ubuntu1) ...
Selecting previously unselected package ssl-cert.
Preparing to unpack .../02-ssl-cert_1.1.3ubuntu2_all.deb ...
Unpacking ssl-cert (1.1.3ubuntu2) ...
Selecting previously unselected package postgresql-common.
Preparing to unpack .../03-postgresql-common_290ubuntu1_all.deb ...
Adding 'diversion of /usr/bin/pg_config to /usr/bin/pg_config.libpq-dev by postgresql-common'
Unpacking postgresql-common (290ubuntu1) ...
Selecting previously unselected package locales.
Preparing to unpack .../04-locales_2.43-2ubuntu2.4_all.deb ...
Unpacking locales (2.43-2ubuntu2.4) ...
Selecting previously unselected package logrotate.
Preparing to unpack .../05-logrotate_3.22.0-1build1_amd64.deb ...
Unpacking logrotate (3.22.0-1build1) ...
Selecting previously unselected package libsensors-config.
Preparing to unpack .../06-libsensors-config_1%3a3.6.2-2build1_all.deb ...
Unpacking libsensors-config (1:3.6.2-2build1) ...
Selecting previously unselected package libsensors5:amd64.
Preparing to unpack .../07-libsensors5_1%3a3.6.2-2build1_amd64.deb ...
Unpacking libsensors5:amd64 (1:3.6.2-2build1) ...
Selecting previously unselected package sysstat.
Preparing to unpack .../08-sysstat_12.7.7-0ubuntu2_amd64.deb ...
Unpacking sysstat (12.7.7-0ubuntu2) ...
Selecting previously unselected package libcommon-sense-perl:amd64.
Preparing to unpack .../09-libcommon-sense-perl_3.75-3build5_amd64.deb ...
Unpacking libcommon-sense-perl:amd64 (3.75-3build5) ...
Selecting previously unselected package libtypes-serialiser-perl.
Preparing to unpack .../10-libtypes-serialiser-perl_1.01-1_all.deb ...
Unpacking libtypes-serialiser-perl (1.01-1) ...
Selecting previously unselected package libjson-xs-perl.
Preparing to unpack .../11-libjson-xs-perl_4.040-1_amd64.deb ...
Unpacking libjson-xs-perl (4.040-1) ...
Selecting previously unselected package libpq5:amd64.
Preparing to unpack .../12-libpq5_18.6-0ubuntu0.26.04.1_amd64.deb ...
Unpacking libpq5:amd64 (18.6-0ubuntu0.26.04.1) ...
Selecting previously unselected package libxslt1.1:amd64.
Preparing to unpack .../13-libxslt1.1_1.1.45-0.1_amd64.deb ...
Unpacking libxslt1.1:amd64 (1.1.45-0.1) ...
Selecting previously unselected package postgresql-client-18.
Preparing to unpack .../14-postgresql-client-18_18.6-0ubuntu0.26.04.1_amd64.deb ...
Unpacking postgresql-client-18 (18.6-0ubuntu0.26.04.1) ...
Selecting previously unselected package postgresql-18.
Preparing to unpack .../15-postgresql-18_18.6-0ubuntu0.26.04.1_amd64.deb ...
Unpacking postgresql-18 (18.6-0ubuntu0.26.04.1) ...
Selecting previously unselected package postgresql.
Preparing to unpack .../16-postgresql_18+290ubuntu1_all.deb ...
Unpacking postgresql (18+290ubuntu1) ...
Selecting previously unselected package postgresql-18-jit.
Preparing to unpack .../17-postgresql-18-jit_18.6-0ubuntu0.26.04.1_amd64.deb ...
Unpacking postgresql-18-jit (18.6-0ubuntu0.26.04.1) ...
Setting up logrotate (3.22.0-1build1) ...
Created symlink '/etc/systemd/system/timers.target.wants/logrotate.timer' → '/usr/lib/systemd/system/logrotate.timer'.
logrotate.service is a disabled or a static unit, not starting it.
Setting up postgresql-client-common (290ubuntu1) ...
Setting up libsensors-config (1:3.6.2-2build1) ...
Setting up libpq5:amd64 (18.6-0ubuntu0.26.04.1) ...
Setting up libcommon-sense-perl:amd64 (3.75-3build5) ...
Setting up locales (2.43-2ubuntu2.4) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Generating locales (this might take a while)...
Generation complete.
Setting up ssl-cert (1.1.3ubuntu2) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Created symlink '/etc/systemd/system/multi-user.target.wants/ssl-cert.service' → '/usr/lib/systemd/system/ssl-cert.service'.
Setting up libsensors5:amd64 (1:3.6.2-2build1) ...
Setting up libtypes-serialiser-perl (1.01-1) ...
Setting up libjson-perl (4.10000-1) ...
Setting up libxslt1.1:amd64 (1.1.45-0.1) ...
Setting up libc-dev-bin (2.43-2ubuntu2.4) ...
Setting up sysstat (12.7.7-0ubuntu2) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Creating config file /etc/default/sysstat with new version
update-alternatives: using /usr/bin/sar.sysstat to provide /usr/bin/sar (sar) in auto mode
update-alternatives: warning: skip creation of /usr/share/man/man1/sar.1.gz because associated file /usr/share/man/man1/sar.sysstat.1.gz (of link group sar) does not exist
Created symlink '/etc/systemd/system/sysstat.service.wants/sysstat-collect.timer' → '/usr/lib/systemd/system/sysstat-collect.timer'.
Created symlink '/etc/systemd/system/sysstat.service.wants/sysstat-rotate.timer' → '/usr/lib/systemd/system/sysstat-rotate.timer'.
Created symlink '/etc/systemd/system/sysstat.service.wants/sysstat-summary.timer' → '/usr/lib/systemd/system/sysstat-summary.timer'.
Created symlink '/etc/systemd/system/multi-user.target.wants/sysstat.service' → '/usr/lib/systemd/system/sysstat.service'.
Setting up libjson-xs-perl (4.040-1) ...
Setting up postgresql-client-18 (18.6-0ubuntu0.26.04.1) ...
update-alternatives: using /usr/share/postgresql/18/man/man1/psql.1.gz to provide /usr/share/man/man1/psql.1.gz (psql.1.gz) in auto mode
Setting up postgresql-common (290ubuntu1) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Creating config file /etc/postgresql-common/createcluster.conf with new version
Building PostgreSQL dictionaries from installed myspell/hunspell packages...
Removing obsolete dictionary files:
Created symlink '/etc/systemd/system/multi-user.target.wants/postgresql.service' → '/usr/lib/systemd/system/postgresql.service'.
Setting up libc6-dev:amd64 (2.43-2ubuntu2.4) ...
Setting up postgresql-18 (18.6-0ubuntu0.26.04.1) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Creating new PostgreSQL cluster 18/main ...
/usr/lib/postgresql/18/bin/initdb -D /var/lib/postgresql/18/main --auth-local peer --auth-host scram-sha-256 --no-instructions
The files belonging to this database system will be owned by user "postgres".
This user must also own the server process.

The database cluster will be initialized with locale "C.UTF-8".
The default database encoding has accordingly been set to "UTF8".
The default text search configuration will be set to "english".

Data page checksums are enabled.

fixing permissions on existing directory /var/lib/postgresql/18/main ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... posix
selecting default "max_connections" ... 100
selecting default "shared_buffers" ... 128MB
selecting default time zone ... Etc/UTC
creating configuration files ... ok
running bootstrap script ... ok
performing post-bootstrap initialization ... ok
syncing data to disk ... ok
Setting up postgresql-18-jit (18.6-0ubuntu0.26.04.1) ...
Setting up postgresql (18+290ubuntu1) ...
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79.)
debconf: falling back to frontend: Readline
Processing triggers for systemd (259.5-0ubuntu3) ...
Processing triggers for libc-bin (2.43-2ubuntu2.4) ...
Scanning processes...                                                                                                                                                                                                                        
Scanning candidates...                                                                                                                                                                                                                       
Scanning linux images...                                                                                                                                                                                                                     

Running kernel seems to be up-to-date.

Restarting services...
 systemctl restart chrony.service cron.service multipathd.service qemu-guest-agent.service ssh.service systemd-journald.service systemd-udevd.service

Service restarts being deferred:
 /etc/needrestart/restart.d/dbus.service
 systemctl restart getty@tty1.service
 systemctl restart networkd-dispatcher.service
 systemctl restart systemd-logind.service
 systemctl restart unattended-upgrades.service

No containers need to be restarted.

User sessions running outdated binaries:
 root @ session #1: bash[1339,1515], sshd-session[1291,1336]
 root @ user manager: (sd-pam)[1300]

No VM guests are running outdated hypervisor (qemu) binaries on this host.
Synchronizing state of postgresql.service with SysV service script with /usr/lib/systemd/systemd-sysv-install.
Executing: /usr/lib/systemd/systemd-sysv-install enable postgresql
CREATE ROLE
CREATE DATABASE
ALTER ROLE
Would you like to customize the Panel Port settings? (If not, a random port will be applied) [y/n]: 
Generated random port: 58212
Port set successfully: 58212
Username and password updated successfully
Base URI path set successfully

═══════════════════════════════════════════
     SSL Certificate Setup (RECOMMENDED)   
═══════════════════════════════════════════
SSL is strongly recommended. Skip only if a reverse proxy
or SSH tunnel handles TLS for you.
Let's Encrypt now supports both domains and IP addresses!

Choose SSL certificate setup method:
1. Let's Encrypt for Domain (90-day validity, auto-renews)
2. Let's Encrypt for IP Address (6-day validity, auto-renews)
3. Custom SSL Certificate (Path to existing files)
4. Skip SSL (advanced — behind reverse proxy / SSH tunnel only)
Note: Options 1 & 2 require port 80 open. Option 3 requires manual paths.
Note: Option 4 serves the panel over plain HTTP — only safe behind nginx/Caddy or an SSH tunnel.
Choose an option (default 2 for IP): 2
Using Let's Encrypt for IP certificate (shortlived profile)...
Is 2.27.209.35 the correct incoming public IPv4 address for this server? [Default y]: n
Please enter your server's public IPv4 address: 13.143.192.84
Do you have an IPv6 address to include? (leave empty to skip): 
Setting up Let's Encrypt IP certificate (shortlived profile)...
Note: IP certificates are valid for ~6 days and will auto-renew.
Default listener is port 80. If you choose another port, ensure external port 80 forwards to it.
Installing acme.sh for SSL certificate management...
acme.sh installed successfully
Port to use for ACME HTTP-01 listener (default 80): 
Using port 80 for standalone validation.
Port 80 is free and ready for standalone validation.
Issuing IP certificate for 13.143.192.84...
[Sun Sep 27 07:46:13 UTC 2026] Using CA: https://acme-v02.api.letsencrypt.org/directory
[Sun Sep 27 07:46:13 UTC 2026] Standalone mode.
[Sun Sep 27 07:46:13 UTC 2026] Account key creation OK.
[Sun Sep 27 07:46:13 UTC 2026] Registering account: https://acme-v02.api.letsencrypt.org/directory
[Sun Sep 27 07:46:15 UTC 2026] Registered
[Sun Sep 27 07:46:15 UTC 2026] ACCOUNT_THUMBPRINT='2tDvWYHVWuPnRkE3JuWuuV1C4mzCkdOAEsmZAtcgT4s'
[Sun Sep 27 07:46:15 UTC 2026] Creating domain key
[Sun Sep 27 07:46:15 UTC 2026] The domain key is here: /root/.acme.sh/13.143.192.84_ecc/13.143.192.84.key
[Sun Sep 27 07:46:15 UTC 2026] Single domain='13.143.192.84'
[Sun Sep 27 07:46:17 UTC 2026] Getting webroot for domain='13.143.192.84'
[Sun Sep 27 07:46:18 UTC 2026] Verifying: 13.143.192.84
[Sun Sep 27 07:46:18 UTC 2026] Standalone mode server
[Sun Sep 27 07:46:20 UTC 2026] Pending. The CA is processing your order, please wait. (1/30)
[Sun Sep 27 07:46:24 UTC 2026] Success
[Sun Sep 27 07:46:24 UTC 2026] Verification finished, beginning signing.
[Sun Sep 27 07:46:24 UTC 2026] Let's finalize the order.
[Sun Sep 27 07:46:24 UTC 2026] Le_OrderFinalize='https://acme-v02.api.letsencrypt.org/acme/finalize/3796487486/562354177326'
[Sun Sep 27 07:46:25 UTC 2026] Downloading cert.
[Sun Sep 27 07:46:25 UTC 2026] Le_LinkCert='https://acme-v02.api.letsencrypt.org/acme/cert/060a7aaa58f268beaf6b2f88a8f32fd9d577'
[Sun Sep 27 07:46:26 UTC 2026] Cert success.
-----BEGIN CERTIFICATE-----
MIIDSzCCAtKgAwIBAgISBgp6qljyaL6vay+IqPMv2dV3MAoGCCqGSM49BAMDMDMx
CzAJBgNVBAYTAlVTMRYwFAYDVQQKEw1MZXQncyBFbmNyeXB0MQwwCgYDVQQDEwNZ
RTIwHhcNMjYwOTI3MDY0NzU0WhcNMjYxMDAzMjI0NzUzWjAAMFkwEwYHKoZIzj0C
AQYIKoZIzj0DAQcDQgAEBCA/bLp0KgSQ5nX9eMEJSqVZhnhPmO2En/s7glboRM2D
aKaQLZO7fusWsczYR7rGJ8xq7al/PkLGmEjHf4pQEaOCAfcwggHzMA4GA1UdDwEB
/wQEAwIHgDATBgNVHSUEDDAKBggrBgEFBQcDATAMBgNVHRMBAf8EAjAAMB8GA1Ud
IwQYMBaAFLlZ8o7PIvCG0zdI/3YUGLqC2FWHMDMGCCsGAQUFBwEBBCcwJTAjBggr
BgEFBQcwAoYXaHR0cDovL3llMi5pLmxlbmNyLm9yZy8wEgYDVR0RAQH/BAgwBocE
DY/AVDATBgNVHSAEDDAKMAgGBmeBDAECATAvBgNVHR8EKDAmMCSgIqAghh5odHRw
Oi8veWUyLmMubGVuY3Iub3JnLzEyMC5jcmwwggEMBgorBgEEAdZ5AgQCBIH9BIH6
APgAdgDLOPcViXyEoURfW8Hd+8lu8ppZzUcKaQWFsMsUwxRY5wAAAaDh1FjdAAAE
AwBHMEUCIDz/ao6B+exVVf3PgH9oyEjdKBud4u3Q4zfXHFpVTdR8AiEAm6HLv+65
Wgl4VOXxPLEjQNLH84i2vykYmjSPgE4/AIAAfgBGr4Y9Oz7ln6V33qgkXTaw2e0i
oiP0YXdBIpRS7pVQXwAAAaDh1FjvAAgAAAUANoVETgQDAEcwRQIgcw0sNXloW9Xu
hCjvNjL/CORTqRdJ5E2KTUAWWPNZs0ECIQDDeWyT/znsmOIAQx1qP2ZvogmZJ+Rs
/laRYGR1TaS9aTAKBggqhkjOPQQDAwNnADBkAjB73D1gxFk8+zW3nj/CpoyzO5DW
gqNqnFMcqXSELwGJ7zGvbieqzpsky+WXg5evYHUCMFtPiMXJ7wcD43Ew/Cf7xvZM
j62lP2ZEWaOY5CTvyegREflF0KPjZ7jof6HSIOpK5g==
-----END CERTIFICATE-----
[Sun Sep 27 07:46:26 UTC 2026] Your cert is in: /root/.acme.sh/13.143.192.84_ecc/13.143.192.84.cer
[Sun Sep 27 07:46:26 UTC 2026] Your cert key is in: /root/.acme.sh/13.143.192.84_ecc/13.143.192.84.key
[Sun Sep 27 07:46:26 UTC 2026] The intermediate CA cert is in: /root/.acme.sh/13.143.192.84_ecc/ca.cer
[Sun Sep 27 07:46:26 UTC 2026] And the full-chain cert is in: /root/.acme.sh/13.143.192.84_ecc/fullchain.cer
[Sun Sep 27 07:46:27 UTC 2026] ARI suggestedWindow: 2026-09-30T13:41:43Z to 2026-09-30T16:52:33Z
[Sun Sep 27 07:46:27 UTC 2026] Next renewal time picked from ARI window: 2026-09-30T14:05:40Z
Certificate issued successfully, installing...
[Sun Sep 27 07:46:28 UTC 2026] The domain '13.143.192.84' seems to already have an ECC cert, let's use it.
[Sun Sep 27 07:46:28 UTC 2026] Installing key to: /root/cert/ip/privkey.pem
[Sun Sep 27 07:46:28 UTC 2026] Installing full chain to: /root/cert/ip/fullchain.pem
[Sun Sep 27 07:46:28 UTC 2026] Running reload cmd: systemctl restart x-ui 2>/dev/null || rc-service x-ui restart 2>/dev/null || true
[Sun Sep 27 07:46:28 UTC 2026] Reload successful
Certificate files installed successfully
Setting certificate paths for the panel...
set certificate public key success
set certificate private key success
set certificate for subscription public key success
set certificate for subscription private key success
Certificate paths configured successfully
IP certificate installed and configured successfully!
Certificate valid for ~6 days, auto-renews via acme.sh cron job.
acme.sh will automatically renew and reload x-ui before expiry.
✓ Let's Encrypt IP certificate configured successfully

═══════════════════════════════════════════
     Panel Installation Complete!         
═══════════════════════════════════════════
Username:    ZsJEHeyip2
Password:    l3PTyp0zpt
Port:        58212
WebBasePath: SE5X6HjJWgWwTbYdB5
Database:    PostgreSQL (WbXswTID@127.0.0.1:5432/xui)
Access URL:  https://13.143.192.84:58212/SE5X6HjJWgWwTbYdB5
API Token:   7Vxn6NB8ymdbeJOEjUVDB8VptDo5EqLXAhr1ujzQxzOWQKQu
═══════════════════════════════════════════
⚠ IMPORTANT: Save these credentials securely!
⚠ SSL Certificate: Enabled and configured

PostgreSQL backup & restore is built into the panel:
  https://13.143.192.84:58212/SE5X6HjJWgWwTbYdB5 → Backup & Restore
  Back Up downloads a pg_dump .dump file; Restore reloads it via pg_restore.

═══════════════════════════════════════════
     PostgreSQL Credentials               
═══════════════════════════════════════════
DB Name:    xui
Username:   WbXswTID
Password:   MnoqEAQ8W7p0sWDYVxyuWf2t
Host:       127.0.0.1
Port:       5432
DSN:        postgres://WbXswTID:MnoqEAQ8W7p0sWDYVxyuWf2t@127.0.0.1:5432/xui?sslmode=disable
Env file:   /etc/default/x-ui
-------------------------------------------
Connect from this server:
  sudo -u postgres psql -d xui      (as the postgres superuser)
  PGPASSWORD='MnoqEAQ8W7p0sWDYVxyuWf2t' psql -h 127.0.0.1 -p 5432 -U WbXswTID -d xui
═══════════════════════════════════════════
⚠ The panel reads these credentials from /etc/default/x-ui.
⚠ Save the password — it is not stored anywhere else in plain text.
Install result written to /etc/x-ui/install-result.env (mode 600).
Start migrating database...
Migration done!
Service files not found in tar.gz, downloading from GitHub...
Setting up systemd unit...
Created symlink '/etc/systemd/system/multi-user.target.wants/x-ui.service' → '/etc/systemd/system/x-ui.service'.
Setting up Fail2ban for the IP Limit feature...
The OS release is: ubuntu
Fail2ban is not installed. Installing now...!

Hit:1 http://security.ubuntu.com/ubuntu resolute-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu resolute InRelease
Hit:3 http://archive.ubuntu.com/ubuntu resolute-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu resolute-backports InRelease
Reading package lists... Done
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Solving dependencies... Done
The following additional packages will be installed:
  libjs-sphinxdoc python3-packaging python3-wheel
Recommended packages:
  build-essential python3-dev
The following NEW packages will be installed:
  libjs-sphinxdoc python3-packaging python3-pip python3-wheel
0 upgraded, 4 newly installed, 0 to remove and 144 not upgraded.
Need to get 1531 kB of archives.
After this operation, 10.9 MB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu resolute/main amd64 libjs-sphinxdoc all 8.2.3-12 [28.4 kB]
Get:2 http://archive.ubuntu.com/ubuntu resolute/main amd64 python3-packaging all 26.0-1 [58.7 kB]
Get:3 http://archive.ubuntu.com/ubuntu resolute/universe amd64 python3-wheel all 0.46.3-2 [27.9 kB]
Get:4 http://archive.ubuntu.com/ubuntu resolute/universe amd64 python3-pip all 25.1.1+dfsg-1ubuntu2 [1416 kB]
Fetched 1531 kB in 0s (6619 kB/s)    
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79, <STDIN> line 4.)
debconf: falling back to frontend: Readline
Selecting previously unselected package libjs-sphinxdoc.
(Reading database ... 128114 files and directories currently installed.)
Preparing to unpack .../libjs-sphinxdoc_8.2.3-12_all.deb ...
Unpacking libjs-sphinxdoc (8.2.3-12) ...
Selecting previously unselected package python3-packaging.
Preparing to unpack .../python3-packaging_26.0-1_all.deb ...
Unpacking python3-packaging (26.0-1) ...
Selecting previously unselected package python3-wheel.
Preparing to unpack .../python3-wheel_0.46.3-2_all.deb ...
Unpacking python3-wheel (0.46.3-2) ...
Selecting previously unselected package python3-pip.
Preparing to unpack .../python3-pip_25.1.1+dfsg-1ubuntu2_all.deb ...
Unpacking python3-pip (25.1.1+dfsg-1ubuntu2) ...
Setting up python3-packaging (26.0-1) ...
Setting up libjs-sphinxdoc (8.2.3-12) ...
Setting up python3-wheel (0.46.3-2) ...
Setting up python3-pip (25.1.1+dfsg-1ubuntu2) ...
Scanning processes...                                                                                                                                                                                                                        
Scanning candidates...                                                                                                                                                                                                                       
Scanning linux images...                                                                                                                                                                                                                     

Running kernel seems to be up-to-date.

Restarting services...

Service restarts being deferred:
 /etc/needrestart/restart.d/dbus.service
 systemctl restart getty@tty1.service
 systemctl restart networkd-dispatcher.service
 systemctl restart systemd-logind.service
 systemctl restart unattended-upgrades.service

No containers need to be restarted.

User sessions running outdated binaries:
 root @ session #1: bash[1339], sshd-session[1291,1336]
 root @ user manager: (sd-pam)[1300]

No VM guests are running outdated hypervisor (qemu) binaries on this host.
Collecting pyasynchat
  Downloading pyasynchat-1.0.5-py3-none-any.whl.metadata (4.0 kB)
Collecting pyasyncore>=1.0.2 (from pyasynchat)
  Downloading pyasyncore-1.0.5-py3-none-any.whl.metadata (4.3 kB)
Downloading pyasynchat-1.0.5-py3-none-any.whl (7.9 kB)
Downloading pyasyncore-1.0.5-py3-none-any.whl (10 kB)
Installing collected packages: pyasyncore, pyasynchat
Successfully installed pyasynchat-1.0.5 pyasyncore-1.0.5
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager, possibly rendering your system unusable. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv. Use the --root-user-action option if you know what you are doing and want to suppress this warning.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Solving dependencies... Done
The following additional packages will be installed:
  libnftables1 libnftnl11 python3-pyasyncore python3-pyinotify whois
Suggested packages:
  mailx system-log-daemon monit sqlite3 firewalld python-pyinotify-doc
The following NEW packages will be installed:
  fail2ban libnftables1 libnftnl11 nftables python3-pyasyncore python3-pyinotify whois
0 upgraded, 7 newly installed, 0 to remove and 144 not upgraded.
Need to get 1049 kB of archives.
After this operation, 4182 kB of additional disk space will be used.
Get:1 http://archive.ubuntu.com/ubuntu resolute/main amd64 libnftnl11 amd64 1.3.1-1 [72.3 kB]
Get:2 http://archive.ubuntu.com/ubuntu resolute/main amd64 libnftables1 amd64 1.1.6-1 [390 kB]
Get:3 http://archive.ubuntu.com/ubuntu resolute/main amd64 nftables amd64 1.1.6-1 [76.2 kB]
Get:4 http://archive.ubuntu.com/ubuntu resolute/universe amd64 fail2ban all 1.1.0-9 [421 kB]
Get:5 http://archive.ubuntu.com/ubuntu resolute/main amd64 python3-pyasyncore all 1.0.2-3build1 [10.4 kB]
Get:6 http://archive.ubuntu.com/ubuntu resolute/main amd64 python3-pyinotify all 0.9.6-5build1 [25.5 kB]
Get:7 http://archive.ubuntu.com/ubuntu resolute/main amd64 whois amd64 5.6.6 [52.5 kB]
Fetched 1049 kB in 0s (4204 kB/s)
debconf: unable to initialize frontend: Dialog
debconf: (No usable dialog-like program is installed, so the dialog based frontend cannot be used. at /usr/share/perl5/Debconf/FrontEnd/Dialog.pm line 79, <STDIN> line 7.)
debconf: falling back to frontend: Readline
Selecting previously unselected package libnftnl11:amd64.
(Reading database ... 128941 files and directories currently installed.)
Preparing to unpack .../0-libnftnl11_1.3.1-1_amd64.deb ...
Unpacking libnftnl11:amd64 (1.3.1-1) ...
Selecting previously unselected package libnftables1:amd64.
Preparing to unpack .../1-libnftables1_1.1.6-1_amd64.deb ...
Unpacking libnftables1:amd64 (1.1.6-1) ...
Selecting previously unselected package nftables.
Preparing to unpack .../2-nftables_1.1.6-1_amd64.deb ...
Unpacking nftables (1.1.6-1) ...
Selecting previously unselected package fail2ban.
Preparing to unpack .../3-fail2ban_1.1.0-9_all.deb ...
Unpacking fail2ban (1.1.0-9) ...
Selecting previously unselected package python3-pyasyncore.
Preparing to unpack .../4-python3-pyasyncore_1.0.2-3build1_all.deb ...
Unpacking python3-pyasyncore (1.0.2-3build1) ...
Selecting previously unselected package python3-pyinotify.
Preparing to unpack .../5-python3-pyinotify_0.9.6-5build1_all.deb ...
Unpacking python3-pyinotify (0.9.6-5build1) ...
Selecting previously unselected package whois.
Preparing to unpack .../6-whois_5.6.6_amd64.deb ...
Unpacking whois (5.6.6) ...
Setting up whois (5.6.6) ...
Setting up fail2ban (1.1.0-9) ...
Created symlink '/etc/systemd/system/multi-user.target.wants/fail2ban.service' → '/usr/lib/systemd/system/fail2ban.service'.
Setting up libnftnl11:amd64 (1.3.1-1) ...
Setting up python3-pyasyncore (1.0.2-3build1) ...
Setting up libnftables1:amd64 (1.1.6-1) ...
Setting up nftables (1.1.6-1) ...
Setting up python3-pyinotify (0.9.6-5build1) ...
Processing triggers for libc-bin (2.43-2ubuntu2.4) ...
Scanning processes...                                                                                                                                                                                                                        
Scanning candidates...                                                                                                                                                                                                                       
Scanning linux images...                                                                                                                                                                                                                     

Running kernel seems to be up-to-date.

Restarting services...

Service restarts being deferred:
 /etc/needrestart/restart.d/dbus.service
 systemctl restart getty@tty1.service
 systemctl restart networkd-dispatcher.service
 systemctl restart systemd-logind.service
 systemctl restart unattended-upgrades.service

No containers need to be restarted.

User sessions running outdated binaries:
 root @ session #1: bash[1339], sshd-session[1291,1336]
 root @ user manager: (sd-pam)[1300]

No VM guests are running outdated hypervisor (qemu) binaries on this host.
Fail2ban installed successfully!

Configuring IP Limit...

Ip Limit jail files created with a bantime of 30 minutes.
Synchronizing state of fail2ban.service with SysV service script with /usr/lib/systemd/systemd-sysv-install.
Executing: /usr/lib/systemd/systemd-sysv-install enable fail2ban
IP Limit installed and configured successfully!

Fail2ban setup complete.
x-ui v3.8.5 installation finished, it is running now...

┌───────────────────────────────────────────────────────┐
│  x-ui control menu usages (subcommands):              │
│                                                       │
│  x-ui              - Admin Management Script          │
│  x-ui start        - Start                            │
│  x-ui stop         - Stop                             │
│  x-ui restart      - Restart                          │
│  x-ui status       - Current Status                   │
│  x-ui settings     - Current Settings                 │
│  x-ui enable       - Enable Autostart on OS Startup   │
│  x-ui disable      - Disable Autostart on OS Startup  │
│  x-ui log          - Check logs                       │
│  x-ui banlog       - Check Fail2ban ban logs          │
│  x-ui update       - Update                           │
│  x-ui legacy       - Legacy version                   │
│  x-ui install      - Install                          │
│  x-ui uninstall    - Uninstall                        │
└───────────────────────────────────────────────────────┘
root@my:~# 