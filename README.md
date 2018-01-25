# oracledb_network_config
Network prerequisites for Oracle 12c database installation.

* hostnamectl set-hostname
* /etc/resolv.conf
* /etc/sysconfig/network
* Public Network
    * ifcfg
    * DNS
* SCAN address in DNS
* Virtual IP address in DNS
* Private Network
    * ifcfg
    * Jumbo frames
    * multicast
    * Reverse path filtering
* /etc/hosts
* Network Time Protocol
    * /etc/ntp.conf
    * /etc/sysconfig/ntpd
    * VMware disable time sync
* Firewall
    * Public network = public zone
    * Private network = trusted zone
* ssh equivalency

## References

* [Grid Infrastructure Startup During Patching, Install or Upgrade May Fail Due to Multicasting Requirement (Doc ID 1212703.1)](https://support.oracle.com/epmos/faces/DocumentDisplay?_afrLoop=433587474287187&id=1212703.1&_afrWindowMode=0&_adf.ctrl-state=i43gabkvh_4)
* [mcasttest.pl](https://support.oracle.com/epmos/main/downloadattachmentprocessor?parent=DOCUMENT&sourceId=1212703.1&attachid=1212703.1:MCASTTEST&clickstream=yes)
