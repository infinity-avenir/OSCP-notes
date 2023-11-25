Notes

Host and Port Scanning
============================================
Nmap Scan the TCP Top port 2000 and save the result as file.
nmap -v -Pn --top-ports 2000 192.168.1.1 --open -oG nmap_topport_2000.txt

Nmap Scan the UDP Top port 2000
nmap -v -Pn -sU --top-ports 2000 192.168.1.1 --open

nmap -sV -sT -sC 192.168.1.1

nmap host & OS detection
nmap -v -A 192.168.1.1

nmap port scan, all port 1-65535
nmap -p 1-65535 192.168.1.1

nmapAutomator scan everything to the target IP
./nmapAutomator.sh --host 192.168.1.1 --type All
https://github.com/21y4d/nmapAutomator

nmap reference book :
https://www.amazon.com/dp/0979958717
============================================

Web Server Scanning
nikto -host http://192.168.1.1:8080/
dirb http://192.168.1.1:8080/
