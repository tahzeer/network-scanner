# Network Scanner

This repository contains a simple network scanner script written in Python using the Scapy library. The script allows you to scan a range of target IP addresses and retrieve their corresponding MAC addresses.

## Prerequisites

- Python 3.x
- Scapy library (`pip install scapy`)
- [Npcap](https://npcap.com/#download): Nmap Project's packet capture (and sending) library for Microsoft Windows.

## Usage

1. Clone the repository using Git or download the script file.

2. Open a terminal or command prompt and navigate to the directory containing the script.

3. Run the script using the following command:

   ```bash
   python network_scanner.py -t <target IP range>
   ```

   Replace `<target IP range>` with the range of IP addresses you want to scan. For example, `192.168.1.1/24` or `10.0.0.1-20`.

4. The script will send ARP requests to the specified IP range and display the IP addresses and MAC addresses of the discovered devices.

## Example

```bash
python network_scanner.py -t 192.168.1.1/24
```

Output:
```
IP                MAC Address
-------------------------------------------
192.168.1.1       00:11:22:33:44:55
192.168.1.2       11:22:33:44:55:66
192.168.1.3       22:33:44:55:66:77
...
```

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute the code for personal or educational purposes.
