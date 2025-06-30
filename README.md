# raghava00-Capturing-and-Analyzing-Network-Traffic-Using-Wireshark-Task-5

📡 Live Network Packet Capture with Wireshark:

Capturing live network packets using Wireshark and identifying common protocols like HTTP, DNS, and TCP.

✅ Prerequisites
A computer with Wireshark installed.

Administrative/root permissions to capture packets.

An active internet connection (to generate real traffic).

🚀 Steps to Capture Packets
Launch Wireshark
Open Wireshark with administrator/root privileges.

Select the Network Interface

Go to the main Wireshark window.

Choose the network interface connected to the internet (e.g., eth0, wlan0, or Wi-Fi).

Click the Start capturing packets (the blue shark fin button).

Generate Traffic

Open a web browser and visit websites (to generate HTTP/HTTPS traffic).

Use the command prompt/terminal to ping or use nslookup (to generate DNS queries).

Any other network activity will generate TCP traffic.

Stop the Capture
After you’ve generated enough traffic, click the red square Stop button in Wireshark.

🔍 Identifying Protocols
HTTP Traffic

Filter: http

Shows web traffic over port 80.

Look for GET/POST requests in the packet details.

DNS Traffic

Filter: dns

Shows DNS queries (UDP/53) and responses.

Check for Standard query and Standard query response.

TCP Traffic

Filter: tcp

Shows all TCP segments (including HTTP, HTTPS, SSH, etc.).

Look for SYN, ACK, FIN flags to understand TCP handshakes and closures.

🛠️ Useful Wireshark Filters
Protocol	Display Filter	Description
HTTP	http	Only HTTP requests/responses
DNS	dns	Only DNS queries/responses
TCP	tcp	All TCP traffic

📑 Tips
Right-click a packet ➔ Follow ➔ TCP Stream to see the full conversation.

Use Statistics ➔ Protocol Hierarchy to see a breakdown of captured protocols.

Save your capture for later analysis with File ➔ Save As.

