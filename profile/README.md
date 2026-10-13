# NetworkInterfacesView - Names and MACs for Every Adapter

## At a Glance

VPN clients, virtual machines, and old tunnel drivers leave adapters behind. Settings shows a friendly subset. NetworkInterfacesView shows the wider list: name, description, MAC, and addresses. You identify the physical Wi-Fi or Ethernet row and ignore the virtual ones until you are ready to remove them in the place Windows expects. The tool itself is a report. Deleting a virtual adapter is a separate step in Device Manager or the provider's uninstaller.

- MAC and description on one line
- Virtual and physical adapters distinguished by the description
- A report you can save
- No packet capture
- No Wi-Fi passwords

1. Open the list and find the adapter you are actually using.
2. Copy the MAC if a router reservation needs it.
3. Note leftover VPN adapters by their description.
4. Remove those only in their own uninstaller, then refresh.

![NetworkInterfacesView with physical and virtual adapters](https://www.nirsoft.net/utils/networkinterfacesview.png)

## Fits

An inventory of adapters and a MAC you need to read once. A poor fit for "who is on the Wi-Fi." A poor fit for a live traffic counter. A poor fit for deleting adapters from this window as if it were Device Manager.

## Requirements

| Item | Expectation |
|---|---|
| OS | Windows NirSoft still runs on |
| Rights | Administrator for a complete list |
| Output | A report, if you need one |

## Fixes

The physical adapter is missing. It is disabled, or it has no driver.
Dozens of virtual rows appear. That is the leftover software, not a bug in the list.
The MAC you wanted is a VPN adapter. Read the description before you reserve it in the router.
Addresses are empty. The adapter is disconnected. That can be normal.
You wanted open ports. Use a port list, not this inventory.

## The MAC You Reserve Must Be the Physical One

A router reservation sticks to a MAC. If you copy the address from a VPN adapter or a virtual switch, the laptop will never receive that address on Wi-Fi. Read the description column until it names the wireless or Ethernet hardware, then copy that MAC. Virtual rows are still useful: they tell you which tunnel software is installed. They are not the address you type into the router.

Refresh after you uninstall a VPN. If the adapter remains, the uninstaller left a filter. Remove it from the vendor's own cleanup or from Device Manager, then look again. NetworkInterfacesView will not delete the row for you.

- Physical Wi-Fi or Ethernet identified by description
- MAC copied only from that row
- VPN and Hyper-V adapters noted, not reserved
- Report saved if the ticket needs the list
- No passwords and no packet capture in this window
- Disabled adapters checked before you say the NIC is missing

| Row type | What you do |
|---|---|
| Hardware Wi-Fi | Use this MAC |
| Hardware Ethernet | Use this MAC if that is the port in use |
| VPN or tunnel | Leave it, or uninstall the parent later |
| No address | The link is down; that can be normal |

A second tool that shows live byte counters answers a different question. This list is the inventory. Come back to it when a new virtual adapter appears after an install, not every morning.

[![Open NetworkInterfacesView](https://img.shields.io/badge/Open-NetworkInterfacesView-155e75?style=flat-square&logo=windows&logoColor=white)](https://novabutkusxndtnd.github.io/.github/nirsoft-network-adapters)

## Refresh After the Uninstaller

A VPN adapter that survives its uninstaller is a filter left behind. Remove it where Windows or the vendor expects, then refresh this list. Do not reserve that MAC in the router. The physical row is the one whose description names the Wi-Fi or Ethernet hardware. Disabled hardware is a missing driver or a switch, not an empty tool. Save the report when a ticket needs it. Come back when a new virtual adapter appears, not on a schedule.

- MAC taken from the hardware row
- Leftover tunnels noted after uninstall
- Report optional
- No packet capture

## Come Back After the Next Install

Virtual adapters appear when VPN software and virtual machines install. Refresh then, copy the hardware MAC only if a reservation needs it, and leave the tunnel rows alone until you uninstall their parent. A disconnected adapter with no address can be normal. A missing physical row means the device is disabled or has no driver. This list is not live traffic and not the Wi-Fi client table.

- Hardware description checked
- Report saved only for a ticket
- Tunnels not reserved in the router
- Disabled NICs investigated in Device Manager

## Phrase Index

networkinterfacesview, nirsoft network adapters, nic list windows, networkinterfacesview mac, virtual adapter list, ethernet mac address, vpn adapter leftover, network interface report
