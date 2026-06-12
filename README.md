# Basic Network Scanning with Nmap

## Demo Video

The demonstration video for this task is included in this repository.

Link: https://drive.google.com/file/d/1cBZpzSyGF-8W-u5G-ObhNG7aWKLjwxcs/view?usp=drive_link 

## Objective

The objective of this task was to perform a basic network scan using Nmap to identify open ports and services running on a target machine.

## Tools Used

* Nmap (Zenmap)
* Windows 11

## Target

localhost (127.0.0.1)

## Scan Results

The scan identified the following open ports:

| Port | Service            |
| ---- | ------------------ |
| 135  | Microsoft RPC      |
| 445  | Microsoft-DS (SMB) |

## Port Analysis

### Port 135 (MSRPC)

Port 135 is used by Microsoft Remote Procedure Call (RPC). This service allows Windows applications and services to communicate with each other across a network.

**Security Significance:**

* Supports Windows administrative functions.
* May reveal information about system services.
* Should be monitored and secured.

### Port 445 (Microsoft-DS)

Port 445 is used by the Server Message Block (SMB) protocol.

**Security Significance:**

* Used for file and printer sharing.
* Has historically been targeted by malware and ransomware attacks.
* Should be protected through proper configuration and updates.

## Operating System Detection

Nmap detected the operating system as Microsoft Windows 11.

## Conclusion

The Nmap scan successfully identified active services running on the local machine. Regular network scanning helps identify exposed services and potential security risks.
