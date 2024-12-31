# tcpdump-Capturing-a-packet

## Scenario
You’re a network analyst who needs to use tcpdump to capture and analyze live network traffic from a Linux virtual machine.

The lab starts with your user account, called analyst, already logged in to a Linux terminal.

Your Linux user's home directory contains a sample packet capture file that you will use at the end of the lab to answer a few questions about the network traffic that it contains.

Here’s how you’ll do this: First, you’ll identify network interfaces to capture network packet data. Second, you’ll use tcpdump to filter live network traffic. Third, you’ll capture network traffic using tcpdump. Finally, you’ll filter the captured packet data.

## **Screenshot Points with Descriptions**

1. **Identify Network Interfaces (ifconfig)**  
 ![image](https://github.com/user-attachments/assets/01717b3f-e47b-4993-9d61-58de72608426)

   - **Description:** Show all available network interfaces on the system, highlighting `eth0` as the primary interface used for packet capture.

2. **List Interfaces (tcpdump -D)**  
![image](https://github.com/user-attachments/assets/cfe6959e-625c-49e3-a0fc-308ea559d3a0)
 
   - **Description:** Show the list of interfaces recognized by tcpdump, demonstrating which interfaces are available for capturing network traffic.

3. **Inspect Live Network Traffic**  
![image](https://github.com/user-attachments/assets/e761af4d-88b6-4e1b-850c-7fde53ae0298)

   - **Description:** Display the first 5 packets captured from the `eth0` interface with verbose details, illustrating timestamps, protocols, and source/destination ports.

4. **Capture Network Traffic to a File**  
![image](https://github.com/user-attachments/assets/2e07328d-394e-4acf-80aa-360de12c5400)

   - **Description:** Show the background process capturing 9 HTTP (port 80) packets to `capture.pcap`, confirming that tcpdump is actively recording the traffic.

5. **Verify Captured File**  
![image](https://github.com/user-attachments/assets/4ff9b571-6e1c-4586-8df9-320fed82737e)

   - **Description:** Demonstrate that the `capture.pcap` file has been created and confirm its presence and size in the filesystem.

6. **Filter Captured Packets (Verbose Mode)**  
![image](https://github.com/user-attachments/assets/f5d157eb-78d1-4cf5-92cc-e6bd086e90dd)
![image](https://github.com/user-attachments/assets/bbf80183-536f-4e44-867c-8eb4406e5de2)

   - **Description:** Show verbose information of the packets from the capture file, including IP headers, TCP flags, and sequence numbers.

7. **View Hex and ASCII Output**  
![image](https://github.com/user-attachments/assets/9af5b4eb-eb83-4463-977b-c5b6029f06e5)
 
   - **Description:** Display the packets in hexadecimal and ASCII formats, highlighting how tcpdump presents deeper forensic details.







