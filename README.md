___
#  Basic Network Sniffer 

This project is an advanced network sniffer built using Python and the `scapy` library. It captures, analyzes, and logs network traffic, offering insights into the flow of data within a network.

## Features

- **Protocol Filtering**: Captures only IP, TCP, UDP, and ICMP packets.
- **Packet Parsing**: Extracts and displays source and destination IP addresses, ports, and protocol type.
- **Live Summary**: Prints a real-time summary of captured packets to the console.
- **File Logging**: Logs captured packet details with timestamps to a file (`captured_packets.log`) for later analysis.

## Prerequisites

Before running the network sniffer, ensure you have the following installed:

- **Python 3.x**: The script is written in Python 3, so you'll need Python installed on your machine.
- **Scapy**: Scapy is a powerful Python library used for network packet manipulation. It can be installed via pip.

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/codealpha_Networksniffer.git
   cd codealpha_Networksniffer
   ```

2. **Install Dependencies**:

   Install the required Python libraries using pip:

   ```bash
   pip install scapy
   ```

## Usage

 **Run the Sniffer**:

   The network sniffer needs to be run with administrator privileges because packet sniffing requires elevated permissions. Run the script using:

   ```bash
   sudo python3 networksniffer.py
   ```


## Logging

The `captured_packets.log` file stores the following details for each captured packet:

- **Timestamp**: The exact date and time the packet was captured.
- **Protocol**: The protocol type (TCP, UDP, ICMP).
- **Source**: The source IP address and port number.
- **Destination**: The destination IP address and port number.

This log file is useful for reviewing the captured packets at a later time, making it suitable for network monitoring and forensic analysis.

## Further Enhancements

This basic network sniffer can be expanded with additional features:

- **PCAP File Saving**: Save captured packets to a `.pcap` file for in-depth analysis using tools like Wireshark.
- **Email Alerts**: Automatically send alerts via email when specific types of packets are detected.
- **GUI Integration**: Develop a graphical user interface to visualize network traffic in real-time and provide user-friendly controls.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

