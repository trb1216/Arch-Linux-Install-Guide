# Arch Linux Install Guide
[ArchWiki](https://wiki.archlinux.org/title/Installation_guide)

## Connect to the internet

```shell
# iwctl
```
### get the "device 'name'"
```shell
[iwd]# device list
```
### get the "station 'name'" aka available networks
```shell
[iwd]# station 'name' get-networks
```
### connect to the network. 
```shell
[iwd]# station "device 'name'" connect "station 'name'" 
```
### verify
#### look for "inet" ip usually 192.something.
```shell
# ip a
```
#### ping an 'address' e.g. archlinux.org or google.com 5 times
```shell
# ping -c5 'address'
```
