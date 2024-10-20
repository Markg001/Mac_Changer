# Mac_Changer
**A simple Mac_changer**
**Description**
This script is designed to change the MAC (Media Access Control) address of a specified network interface on a Linux system. It allows users to easily alter the MAC address for privacy, security, or testing purposes.

**Features:**
Change the MAC address of any network interface on the system.
Retrieve and display the current MAC address before and after making changes.
Input validation to ensure necessary options are provided.

**Benefits of This Script**
  [1]Privacy & Security: Changing your MAC address can help improve privacy when connecting to public Wi-Fi networks. By changing the MAC address, you can prevent tracking and improve anonymity, since the MAC address is often used by networks to     
     identify devices.

  [2]Network Testing: In network penetration testing, changing your MAC address can help bypass MAC filtering (a security measure used by some networks) or test network behavior with different devices.

  [3]Bypassing Network Restrictions: In some cases, networks or ISPs (Internet Service Providers) may restrict devices based on their MAC addresses. Changing the MAC address can sometimes help bypass these restrictions and reconnect to the network.

**Prerequisites**
This script is designed to run on Linux-based systems with the ifconfig tool installed. Ensure that you have administrative (root) privileges to run it, as changing the MAC address requires elevated permissions.

To run the script, use:

sudo python3 mac_changer.py -i <interface> -m <new_mac_address>

**Example Usage**

sudo python3 mac_changer.py -i wlan0 -m 00:11:22:33:44:55
wlan0 is the network interface to change.
00:11:22:33:44:55 is the new MAC address to assign.
Output:

[+] Changing MAC address for wlan0 to 00:11:22:33:44:55
Current MAC = 11:22:33:44:55:66
[-] MAC address was successfully changed to 00:11:22:33:44:55
