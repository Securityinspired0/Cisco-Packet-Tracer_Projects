#  Cisco Packet Tracer Projects

DHCP (Dynamic Host Configuration Protocol) is a network protocol that enables a device, such as a computer or router, to automatically obtain its IP address and other network configuration information from a DHCP server

# List of steps to configure a DHCP Server
1. Create a network configuration where a DHCP server allocates IP addresses. In this project, include 7 PCs, a switch, and a server.
2. Establish physical connections using wires between all the networking devices in this setup.
3. Commence the configuration process for the DHCP Server

# Configure the DHCP Server settings.

  1. Navigate to DHCP Server > Services > DHCP. Choose the IP range for this server; let's opt for the Network ID 192.168.1.0.

     Here are the specified IP parameters for the network configuration: Network ID: 192.168.1.0 - Default Gateway: 192.168.1.1 - Subnet Mask: 255.255.255.0 - IP Address Range: 192.168.1.0 - 192.168.1.255 -       
     Usable IP Address Range: 192.168.1.1 - 192.168.1.254 - Total Hosts: 256 - Usable Hosts: 254

  3. Now that we've collected the necessary information for DHCP Server configuration, proceed with the followng steps.

     * Within the DHCP tab, locate the Pool Name field and input the preferred pool name.
     * Moving forward, in the Default Gateway field, input the value 192.168.1.1.
     * Following that, for the DNS Server entry, use the IP address of the server itself, which is 192.168.1.1. Note that in this scenario, the default gateway and the server's IP address are identical.
     * Continuing with the configuration, set the Starting IP address to 192.168.1.2.
     * Proceeding to the Subnet Mask configuration, enter 255.255.255.0, which is the default subnet mask for a Class C IP address.
     * Moving on to the Maximum Users setting, input the desired value based on your requirements; for instance, you can fill in 50 as an example.
     * Select the "Add" option to incorporate this IP range into the Server's IP Pool.
    
  # Test the DHCP Server
    * To assess the DHCP Server's functionality, navigate to the configuration settings of each PC. Within the "Interface" section, specifically in the "IP Configuration" block, switch from the static option DHCP       for the FastEthernet0 interface. This adjustment enables the PCs to dynamically obtain IP addresses from the DHCP Server.
    * Indeed, with the DHCP configuration in place, the DHCP server will automatically select an available IP address and assign it to the respective PC or any network device that requests an IP address. This   
      dynamic allocation simplifies the network setup process and helps prevent IP address conflicts.






    
