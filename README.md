# Configure DHCP on Wireless Router
Lab: Configure DHCP on a Wireless Router using Packet Tracer

![Packet Tracer - Configure DHCP on a Wireless Router](https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/ae60e0d2-708f-47bf-b2bb-a38f414ae1bb)


## Objective:
The objective is to connect PCs to the router, change DHCP settings, and enable clients to obtain their IP addresses automatically. I'll be using Packet Tracer software, three generic PCs, a wireless router, and Ethernet cables. Let's dive in and explore the world of network configuration, automation, and seamless connectivity. 

Prerequisites:
- Packet Tracer software
- Three generic PCs
- One wireless router
- Straight-through Ethernet cables

Instructions:
<details>
  
<summary> 
  
  ### Part 1: Set up the network topology

</summary>  

1. Open Packet Tracer and create a new network topology.
2. Add three generic PCs to the workspace.
3. Connect each PC to an Ethernet port on the wireless router using straight-through cables.

- ![Select Straight Through Cable](https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/b838bce9-8908-4116-9d9e-046b12fa4f8b)


</details>

#

<details>

  <summary>
    
### Part 2: Observe the default DHCP settings
  </summary>
  
1. Wait for the amber lights on the devices to turn green.
- <img width="350" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/742ee137-4586-4652-a0cc-c05012caf4dc"/>

3. Click on PC0, then click on the Desktop tab and select IP Configuration.
- <img width="500" alt="Select IP Configuration (PC0)" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/8c887fe6-a8a7-4ea9-993b-ecf30dc157bb"/>

5. Choose DHCP to receive an IP address from the DHCP-enabled router.
- <img width="900" alt="Configure DHCP Wireless Router (PC0)" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/d85b63af-3d33-40ac-baed-ecbc818769fe"/>

7. Record the IP address of the default gateway (picture here `192.168.0.1`).
8. Close the IP Configuration window.
  - You can close the window by selecting the `X` button to the right of IP Configuration.
10. Open a web browser on PC0.
    - <img width="500" alt="Select Web Browser PC0" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/2d090e92-e4ec-4ccc-bb60-788b59896e8e"/>

11. Enter the recorded IP address of the default gateway into the URL field.
    - <img width="500" alt="image" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/cc7afa69-ec9a-45a7-9825-02b3fa8c8502"/>

13. When prompted, enter the username "admin" and password "admin".
    - <img width="500" alt="Login to router with default credentials (PC0)" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/89ec063e-f127-45e3-af26-6add9aa8deed"/>

15. Scroll through the Basic Setup page to view the default settings, including the default IP address of the wireless router.
16. Notice that DHCP is enabled, the starting address of the DHCP range, and the range of addresses available to clients.
    >**Note**: The starting IP address here is 192.168.0.100

</details>

#

<details>
  <summary>
    
  ### Part 3: Change the default IP address of the wireless router
</summary>

1. Within the Router IP Settings section, change the IP address to 192.168.5.1.
   - <img width="500" alt="Change router ip address" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/8087ec93-42d2-4e50-b1bd-fa44f5d7946a"/>

3. Scroll to the bottom of the page and click Save Settings.
4. If done correctly, the web page will display an error message. Close the web browser.
   - <img width="500" alt="Request timeout after changing default ip address" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/324d4455-00fc-44f6-a272-d7b44834c34f"/>

6. Click IP Configuration on PC0 to renew the assigned IP address. (Recall this from Part 2)
7. Click Static, then click DHCP to receive new IP address information from the wireless router.
   - <img width="700" alt="DHCP update after start IP change" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/92162ba7-5ebf-4556-9580-14acdff6fe92"/>

9. Open the web browser again and enter the IP address 192.168.5.1 in the URL field.
10. When prompted, enter the username "admin" and password "admin".
</details>

#

<details>
<summary>

### Part 4: Change the default DHCP range of addresses
</summary>

1. Notice that the DHCP Server Start IP Address is updated to the same network as the Router IP.
2. Change the Starting IP Address from 192.168.5.100 to 192.168.5.126.
   - Change the Maximum Number of Users to 75. 
   - <img width="600" alt="Change start ip address" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/f9812566-9482-4587-a125-4834b770bdfc"/>


5. Scroll to the bottom of the page and click Save Settings. Close the web browser.
6. Click IP Configuration on PC0 to renew the assigned IP address.
7. Click Static, then click DHCP to receive new IP address information from the wireless router.
8. Select Command Prompt on PC0 and enter "ipconfig".
   - <img width="500" alt="IPConfig PC0" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/1dee329b-0606-4cae-86a7-3c0ef095f447"/>


  >**Note**: Record the IP address for PC0.
</details>

#

<details>
  <summary>
    
### Part 5: Enable DHCP on the other PCs
</summary>

1. Click on PC1.
2. Select the Desktop tab.
3. Select IP Configuration.
4. Click DHCP.
   - <img width="600" alt="DHCP PC1" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/7594356b-a72a-4524-9ca1-4610a6d89958"/>


  >**Note**: Record the IP address for PC1.

5. Close the configuration window.
6. Enable DHCP on PC2 following the same steps as for PC1.
   - <img width="600" alt="DHCP PC2" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/8009706e-f373-4d2f-bb04-2813accb32c4"/>

</details>

#

<details>
<summary>
  
### Part 6: Verify connectivity
</summary>

1. Click on PC2 and select the Desktop tab.
2. Select Command Prompt.
3. Enter "ipconfig" at the prompt to view the IP configuration.
   - <img width="675" alt="IPConfig PC2" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/111f2a9f-cc09-4a60-abe6-d4b4b21fae72"/>

5. At the prompt, enter "ping 192.168.5.1" to ping the wireless router.
6. Enter "ping 192.168.5.126" to ping PC0.
7. At the prompt, enter "ping 192.168.5.127" to ping PC1.
8. The pings to all devices should be successful.
   - <img width="500" alt="Ping other devices from PC2" src="https://github.com/0xbythesecond/Configure-DHCP-on-Wireless-Router/assets/23303634/e35b4948-b9de-4b39-8fd4-1f9c4207f236"/>

</details>

## Conclusion:
I have successfully configured DHCP on a wireless router using Packet Tracer. I've learned how to connect PCs to the router, change the DHCP settings, and configure clients to obtain IP addresses automatically. DHCP simplifies network configuration by assigning IP addresses dynamically, ensuring efficient and automatic network connectivity. By using DHCP, it removes human error when entering the IP addresses manually to end devices. On the other hand, there are some devices that one would like to enter the IP address manually so that they remain static and unchanged such as routers, printers, FTP servers, and DHCP servers. This lab was part of Cisco's Networking Academy Networking Basics through the Skills for All curriculum and you can learn more [here](https://skillsforall.com/).
