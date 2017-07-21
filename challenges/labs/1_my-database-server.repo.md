Installation of mariadb and mariadb-server used the repo file redhat-rhui.repo and the repository rhui-REGION-rhel-server-releases.
 
The definition for rhui-REGION-rhel-server-releases  is 
[rhui-REGION-rhel-server-releases]
name=Red Hat Enterprise Linux Server 7 (RPMs)
mirrorlist=https://rhui2-cds01.REGION.aws.ce.redhat.com/pulp/mirror/content/dist/rhel/rhui/server/7/$releasever/$basearch/os
enabled=1
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-redhat-release
sslverify=1
sslclientkey=/etc/pki/rhui/content-rhel7.key
sslclientcert=/etc/pki/rhui/product/content-rhel7.crt
sslcacert=/etc/pki/rhui/cdn.redhat.com-chain.crt
