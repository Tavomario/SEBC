List the cloud provider you are using (AWS, GCE, Azure, CloudCat, other): 
ANSWER: AWS
        
List your instances by IP address and DNS name (don't use /etc/hosts for this):
ANSWER:

NAME      PUBLIC IP           PRIVATE IP        PUBLIC DNS
NODO1			34.212.217.234			172.31.42.113			ec2-34-212-217-234.us-west-2.compute.amazonaws.com
NODO2			35.163.137.186			172.31.33.89			ec2-35-163-137-186.us-west-2.compute.amazonaws.com
NODO3			52.37.192.39			  172.31.45.231			ec2-52-37-192-39.us-west-2.compute.amazonaws.com
NODO4			52.88.181.34			  172.31.41.195			ec2-52-88-181-34.us-west-2.compute.amazonaws.com
 
List the Linux release you are using:
ANSWER:
[root@ip-172-31-42-113 opt]# cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.3 (Maipo)

[root@ip-172-31-33-89 ec2-user]# cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.3 (Maipo)

[root@ip-172-31-45-231 ec2-user]# cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.3 (Maipo)

[root@ip-172-31-41-195 ec2-user]# cat /etc/redhat-release
Red Hat Enterprise Linux Server release 7.3 (Maipo)

List the file system capacity for the first node:
ANSWER:
[root@ip-172-31-42-113 opt]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2      160G  982M  160G   1% /
devtmpfs         15G     0   15G   0% /dev
tmpfs            15G     0   15G   0% /dev/shm
tmpfs            15G   17M   15G   1% /run
tmpfs            15G     0   15G   0% /sys/fs/cgroup
tmpfs           3.0G     0  3.0G   0% /run/user/1000
[root@ip-172-31-42-113 opt]#

List the command and output for yum repolist enabled:
ANSWER:
[root@ip-172-31-42-113 opt]# yum repolist
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
rhui-REGION-client-config-server-7                                                                                                               | 2.9 kB  00:00:00
rhui-REGION-rhel-server-releases                                                                                                                 | 3.5 kB  00:00:00
rhui-REGION-rhel-server-rh-common                                                                                                                | 3.8 kB  00:00:00
(1/7): rhui-REGION-rhel-server-releases/7Server/x86_64/group                                                                                     | 701 kB  00:00:00
(2/7): rhui-REGION-client-config-server-7/x86_64/primary_db                                                                                      | 5.4 kB  00:00:00
(3/7): rhui-REGION-rhel-server-releases/7Server/x86_64/updateinfo                                                                                | 1.9 MB  00:00:00
(4/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/group                                                                                    |  104 B  00:00:00
(5/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/updateinfo                                                                               |  33 kB  00:00:00
(6/7): rhui-REGION-rhel-server-rh-common/7Server/x86_64/primary_db                                                                               | 118 kB  00:00:00
(7/7): rhui-REGION-rhel-server-releases/7Server/x86_64/primary_db                                                                                |  38 MB  00:00:00
repo id                                                                  repo name                                                                                status
rhui-REGION-client-config-server-7/x86_64                                Red Hat Update Infrastructure 2.0 Client Configuration Server 7                               6
rhui-REGION-rhel-server-releases/7Server/x86_64                          Red Hat Enterprise Linux Server 7 (RPMs)                                                 14,598
rhui-REGION-rhel-server-rh-common/7Server/x86_64                         Red Hat Enterprise Linux Server 7 RH Common (RPMs)                                          228
repolist: 14,832

List the /etc/passwd entries for saturn and haley
ANSWER:
saturn:x:2800:2902::/home/saturn:/bin/bash
haley:x:2900:2901::/home/haley:/bin/bash

List the /etc/group entries for comets and planets
ANSWER:
comets:x:2901:
planets:x:2902:






