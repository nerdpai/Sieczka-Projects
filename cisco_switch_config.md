# Cisco Catalyst 3560G Switch Configuration

This guide provides instructions on how to factory reset a Cisco Catalyst 3560G switch, configure it, and connect it to another switch using a trunk.

## Factory Reset

1. **Boot the switch**: Start the Cisco Catalyst 3560G switch.
2. **Enter the boot mode**: During the booting process, press and hold the boot button. When the LEDs on the device turn off, continue holding until they turn bright again, then release the boot button.
3. **Initialize flash**: Enter the command `flash_init`.
4. **Check the files and directories**: Use the command `dir flash:` to see which files and directories you have.
5. **Delete unnecessary files**: Delete all files except the system file (the .bin file) using the command `del [your dir]:[your file]`.
6. **Boot the switch**: Use the `boot` command to boot the switch.

For a visual guide on how to perform these steps, refer to this video tutorial.
[My Little Lan](https://www.youtube.com/watch?v=dmZPOAJ1KwE)

## Switch Configuration

Perform the following steps to configure the switch:

1. **Enter enable mode**: `Switch> enable`
2. **Enter configuration terminal**: `Switch# configure terminal`
3. **Remove enable password**: `Switch(config)# no enable password`
4. **Configure console line**: `Switch(config)# line console 0`
5. **Set console password**: `Switch(config-line)# password random_password`
6. **Enable console login**: `Switch(config-line)# login`
7. **Set hostname**: `Switch(config)# hostname random_name`
8. **Configure VLAN interface**: `Switch(config)# interface vlan random_vlan`
9. **Set IP address**: `Switch(config-if)# ip address random_ip random_mask`
10. **Enable VLAN interface**: `Switch(config-if)# no shutdown`
11. **Create VLAN**: `Switch(config)# vlan vlan_number`
12. **Name VLAN**: `Switch(config-vlan)# name vlan_name`
13. **Configure interface for trunking**: `Switch(config)# interface interface_name`
14. **Set trunk mode**: `Switch(config-if)# switchport mode trunk`
15. **Save Configuration**: `Switch(config)# copy running-config startup-config`

## Second one

Now make the similar configuration for the second one and all is done.
