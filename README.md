# Port-scanner-in-Python
SYN ACK scan
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
UDP scan
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
Comprehensive scan
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
