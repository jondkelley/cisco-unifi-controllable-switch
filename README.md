# Integrating a Cisco switch with a UniFi controller

The UniFi controller provides integration for Ubiquiti's UniFi hardware. However, they don't really support anything but their overpriced switches. This project aims to add basic read-only support to the UnifiController using SNMP v2 and v3 from Cisco devices.

This project borrows from the similarly named project unifi-controllable-switch which was a custom TOUGHswitch firmware. Unfortunately, unlike the TOUGHswitch project, Cisco devices do not run a Linux based OS. You will need a Windows or Linux computer to run against your switches to poll SNMP and send the UniFi announcements to your UniFi controller.

## Links

* UniFi protocol
 - [Help: What protocol does the controller use to communicate with the UAP?](https://help.ubnt.com/hc/en-us/articles/204976094-UniFi-What-protocol-does-the-controller-use-to-communicate-with-the-UAP-)
 - [jk-5/unifi-inform-protocol](https://github.com/jk-5/unifi-inform-protocol)
 - [fxkr/unifi-protocol-reverse-engineering](https://github.com/fxkr/unifi-protocol-reverse-engineering)
 - [nutefood/python-ubnt-discovery](https://github.com/nitefood/python-ubnt-discovery)
 - [job/ubbnut](https://github.com/jof/ubbnut)
 - [Ubiquiti inform protocol](https://github.com/mcrute/ubntmfi/blob/master/inform_protocol.md)
 - [model identifiers](https://community.ubnt.com/ubnt/attachments/ubnt/UniFi/194506/1/bundles.json.txt)
* UniFi controller docker image at [jacobalberti/unifi](https://hub.docker.com/r/jacobalberty/unifi/)
* [finish06/unifi-api](https://github.com/finish06/unifi-api) - utitilies to manage a UniFi controller
* [sol1/icinga-ubiquiti-mfi](https://github.com/sol1/icinga-ubiquiti-mfi) - parser for mFi `mca-dump`'s json output
* [mcrute/ubntmfi](https://github.com/mcrute/ubntmfi) - web controller for mFi hardware
* OpenWRT on [UniFi AP AC](https://wiki.openwrt.org/toh/ubiquiti/unifiac)
* [TOUGHswitch@wikidevi](https://wikidevi.com/wiki/Ubiquiti_Networks_TOUGHSwitch_PoE_Pro)
