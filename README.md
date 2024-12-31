# **tcpdump: Capturing and Analyzing Network Packets**

## **Scenario**
You are a network analyst tasked with capturing and analyzing live network traffic using `tcpdump` on a Linux virtual machine.

- Your lab environment starts with the `analyst` user already logged into the Linux terminal.
- A sample packet capture file is provided in your home directory for analysis.

### **Lab Objectives**
1. Identify network interfaces available for packet capture.
2. Use `tcpdump` to inspect live network traffic.
3. Capture network traffic to a file for further analysis.
4. Analyze and filter captured data using `tcpdump`.

---

## **Screenshot Points with Descriptions**

### **1. Identify Network Interfaces (ifconfig)**  
![Identify Network Interfaces](https://github.com/user-attachments/assets/01717b3f-e47b-4993-9d61-58de72608426)

- **Description:** Display all available network interfaces using the `ifconfig` command. Highlight the `eth0` interface, which will be used for packet capture.

---

### **2. List Interfaces (tcpdump -D)**  
![List Interfaces](https://github.com/user-attachments/assets/cfe6959e-625c-49e3-a0fc-308ea559d3a0)

- **Description:** Show the list of available interfaces recognized by `tcpdump` using the `tcpdump -D` command. This confirms which interfaces are available for capturing traffic.

---

### **3. Inspect Live Network Traffic**  
![Inspect Live Traffic](https://github.com/user-attachments/assets/e761af4d-88b6-4e1b-850c-7fde53ae0298)

- **Description:** Use `tcpdump` to capture and display the first 5 packets from the `eth0` interface in verbose mode. Highlight timestamps, protocols, source/destination ports, and other packet details.

---

### **4. Capture Network Traffic to a File**  
![Capture Traffic to File](https://github.com/user-attachments/assets/2e07328d-394e-4acf-80aa-360de12c5400)

- **Description:** Run `tcpdump` in the background to capture 9 HTTP packets (port 80) from the `eth0` interface and save them to a file named `capture.pcap`. This demonstrates the ability to save traffic for later analysis.

---

### **5. Verify Captured File**  
![Verify Captured File](https://github.com/user-attachments/assets/4ff9b571-6e1c-4586-8df9-320fed82737e)

- **Description:** Use the `ls -l` command to verify the presence of the `capture.pcap` file and its size in the filesystem. This confirms successful packet capture.

---

### **6. Filter Captured Packets (Verbose Mode)**  
![Filter Packets - Verbose Mode 1](https://github.com/user-attachments/assets/f5d157eb-78d1-4cf5-92cc-e6bd086e90dd)  
![Filter Packets - Verbose Mode 2](https://github.com/user-attachments/assets/bbf80183-536f-4e44-867c-8eb4406e5de2)

- **Description:** Use `tcpdump` to read the `capture.pcap` file in verbose mode. Highlight key details such as IP headers, TCP flags, and sequence numbers for deeper packet inspection.

---

### **7. View Hexadecimal and ASCII Output**  
![View Hex and ASCII Output](https://github.com/user-attachments/assets/9af5b4eb-eb83-4463-977b-c5b6029f06e5)

- **Description:** Display packets from the `capture.pcap` file in hexadecimal and ASCII formats using `tcpdump`. This output provides deeper forensic insights for detecting patterns or anomalies.

