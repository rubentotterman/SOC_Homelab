# SOC_Homelab

VirtualBox Settings
Create a new virtual machine.

![setting01](https://github.com/user-attachments/assets/688b2614-e28d-48e6-b0ae-5b264ed053e9)

![setting02](https://github.com/user-attachments/assets/1923b43c-304f-4bdb-bbe3-727e8317eb49)

![setting03](https://github.com/user-attachments/assets/191410c1-897e-4dae-8367-b9ae18a5291b)

![setting04](https://github.com/user-attachments/assets/5c8a361d-9098-4dc7-bf96-1ac42fbe8ca4)

![setting05](https://github.com/user-attachments/assets/4688751e-4305-484c-bf55-4712b51e4584)

![setting06](https://github.com/user-attachments/assets/f96f09aa-be6b-49c3-8ac6-0a21120189aa)

Go to the VM properties.

In Network tab, activate 3 adapters.

Making note of the MAC Addresses of each adapters will be useful for future actions. This will be the RED CARD. (external network)

![setting07](https://github.com/user-attachments/assets/e32e27b9-8748-46d3-9a78-ac318f447b7d)


This will be the GREEN CARD. (internal network)

![setting08](https://github.com/user-attachments/assets/24f9edb5-545b-4b2a-8bd7-e7beba293de0)

This will be the orange CARD. (dmz)

![setting09](https://github.com/user-attachments/assets/d84e6f0f-7042-4b3b-8516-270fb4efa644)

Launch the VM. It will ask you which ISO Virtualbox must mount on the VM, load the pfsense one.


Installation
Accept the Copyright and Trademark Notices.

![install01](https://github.com/user-attachments/assets/81ced819-e55c-402f-8af7-1f660a65827a)

Select "install".

![install02](https://github.com/user-attachments/assets/64ffc1db-e913-4487-822c-2ba70d86ce4a)

-Select your keymap

-Use the default partition (we're in a lab, we just need a firewall)

-Proceed with installation (no miror, no encrypt, nothing)

-Wait until the installation is complete

![install03](https://github.com/user-attachments/assets/e35df76a-54db-4b85-8c29-eae080fbf536)


Do not load manual configuration.

![install04](https://github.com/user-attachments/assets/0351ca1e-4d1e-41c0-9944-41ceb160d643)


Reboot on the new system.


Configuration
Now, the server is powered on with the new system. 

![conf01](https://github.com/user-attachments/assets/2e6f1556-4104-4a7e-bfbb-27a8f1b17bed)


Select 1 to configure interfaces.

![conf02](https://github.com/user-attachments/assets/2ea7f2c9-8365-4dc3-9f58-f2735b5ec322)


We can see the MAC Addresses. Remember, we recommended to make a note of the MAC addresses. It is always helpful to have/know them.

-Select the RED INTERFACE for WAN

-Select the GREEN INTERFACE for LAN

-Select the last one (ORANGE) for DMZ

![conf03](https://github.com/user-attachments/assets/eba5f76d-85ec-4e5b-a60d-4719093e61f9)

Confirm.


![conf04](https://github.com/user-attachments/assets/4b5dcddc-2ba0-4f18-80d5-b2a133b6d9d9)

- Select 2 to configure the IP address

- Leave the WAN interface as DHCP

- Select 2 to change the LAN interface

- Asssign the IP and subnet you want, the gateway must be "none" !

