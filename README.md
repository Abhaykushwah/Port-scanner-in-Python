# Port Scanner in Python

This project is a Python-based port scanner using Nmap for scanning ports on a given IP address. It supports different types of scans and provides detailed information about the open ports. The script is designed to offer a simple and effective way to identify open TCP and UDP ports on a target system.

## Features

1. **SYN ACK Scan**: 
   - Scans for open TCP ports by sending SYN packets and listening for ACK responses.
   - Displays open ports on the given IP address for TCP-based services.

2. **UDP Scan**:
   - Scans for open UDP ports by sending empty UDP packets and checking for responses.
   - Displays open ports on the target machine for UDP-based services.

3. **Comprehensive Scan**:
   - Runs both SYN ACK and UDP scans to provide a full overview of open ports on the target machine.

## How to Use

1. **Install Nmap**: Make sure that Nmap is installed on your system. You can download and install Nmap from [here](https://nmap.org/download.html).
   
2. **Run the Script**:
   - Open a terminal or command prompt and navigate to the directory containing the script.
   - Execute the script by running:
     ```
     python port_scanner.py
     ```

3. **Input**:
   - The script will prompt you to enter the IP address of the machine you want to scan.
   - You can input any valid IP address (e.g., `127.0.0.1` for localhost).

4. **Choose Scan Type**:
   - The script will present three scan options:
     1. **SYN ACK Scan**
     2. **UDP Scan**
     3. **Comprehensive Scan**
   - Select the desired scan type by entering the corresponding number.

5. **Output**:
   - After the scan is complete, the script will display the status of the IP address (up/down) and the open ports found for the selected scan type.

## Example Outputs

- **SYN ACK Scan**:
  ```
  Open Ports are: [135, 137, 445, 902, 912, 1001]
  ```
  
- **UDP Scan**:
  ```
  Open Ports are: [137, 500]
  ```
  
- **Comprehensive Scan**:
  ```
  Open Ports are: [135, 137, 445, 902, 912, 1001]
  ```

## Requirements

- Python 3.x
- Nmap (installed on your system)

---
 - SYN ACK scan
```
PS C:\Users\Abhay> python -u "c:\Users\Abhay\Desktop\port scanner.py"
 This Nmap script is created by Abhay
Please Enter IP address you want to scan : 127.0.0.1
You enter the following addr to scan  127.0.0.1
 
            1) SYN ACK scan
            2) UDP scan
            3) Comprehensive scan
            ---------->>>1
you have selected : 1
<class 'int'>
NMAP version  <bound method PortScanner.nmap_version of <nmap.nmap.PortScanner object at 0x00000149A2344B00>>
<bound method PortScanner.scaninfo of <nmap.nmap.PortScanner object at 0x00000149A2344B00>>
Ip addr status :  up
['tcp']
Open Ports are :  dict_keys([135, 137, 445, 902, 912, 1001])
```
---
 - UDP scan
```
PS C:\Users\Abhay> python -u "c:\Users\Abhay\Desktop\port scanner.py"
 This Nmap script is created by Abhay
Please Enter IP address you want to scan : 127.0.0.1
You enter the following addr to scan  127.0.0.1
 
 Please enter the type of scan you want to run 
            1) SYN ACK scan
            2) UDP scan
            3) Comprehensive scan
            ---------->>>2
you have selected : 2
<class 'int'>
NMAP version  <bound method PortScanner.nmap_version of <nmap.nmap.PortScanner object at 0x000002204E5D4B00>>
<bound method PortScanner.scaninfo of <nmap.nmap.PortScanner object at 0x000002204E5D4B00>>
Ip addr status :  up
['udp']
Open Ports are :  dict_keys([137, 500])
```
---
 - Comprehensive scan
```
PS C:\Users\Abhay> python -u "c:\Users\Abhay\Desktop\port scanner.py"
 This Nmap script is created by Abhay
Please Enter IP address you want to scan : 127.0.0.1
You enter the following addr to scan  127.0.0.1

 Please enter the type of scan you want to run
            1) SYN ACK scan
            2) UDP scan
            3) Comprehensive scan
            ---------->>>3
you have selected : 3
<class 'int'>
NMAP version  <bound method PortScanner.nmap_version of <nmap.nmap.PortScanner object at 0x000002F4F7EA4B00>>
<bound method PortScanner.scaninfo of <nmap.nmap.PortScanner object at 0x000002F4F7EA4B00>>
Ip addr status :  up
['tcp']
Open Ports are :  dict_keys([135, 137, 445, 902, 912, 1001])
```
