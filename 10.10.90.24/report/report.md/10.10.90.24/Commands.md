```bash
nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/_quick_tcp_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/xml/_quick_tcp_nmap.xml" 10.10.90.24

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/_full_tcp_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/xml/_full_tcp_nmap.xml" 10.10.90.24

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/_quick_tcp_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/xml/_quick_tcp_nmap.xml" 10.10.90.24

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/_full_tcp_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/xml/_full_tcp_nmap.xml" 10.10.90.24

nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/_top_100_udp_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/xml/_top_100_udp_nmap.xml" 10.10.90.24

feroxbuster -u http://10.10.90.24:8081/ -t 10 -w /root/.local/share/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -r -o "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_feroxbuster_dirbuster.txt"

curl -sSikf http://10.10.90.24:8081/.well-known/security.txt

curl -sSikf http://10.10.90.24:8081/robots.txt

curl -sSik http://10.10.90.24:8081/

nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://10.10.90.24:8081 2>&1 | tee "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nikto.txt"

nmap -vv --reason -Pn -T4 -sV -p 8081 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/xml/tcp_8081_http_nmap.xml" 10.10.90.24

whatweb --color=never --no-errors -a 3 -v http://10.10.90.24:8081 2>&1

wkhtmltoimage --format png http://10.10.90.24:8081/ /home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_screenshot.png

feroxbuster -u http://10.10.90.24:31331/ -t 10 -w /root/.local/share/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -r -o "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_feroxbuster_dirbuster.txt"

curl -sSikf http://10.10.90.24:31331/.well-known/security.txt

curl -sSikf http://10.10.90.24:31331/robots.txt

curl -sSik http://10.10.90.24:31331/

nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://10.10.90.24:31331 2>&1 | tee "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_nikto.txt"

nmap -vv --reason -Pn -T4 -sV -p 31331 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/xml/tcp_31331_http_nmap.xml" 10.10.90.24

whatweb --color=never --no-errors -a 3 -v http://10.10.90.24:31331 2>&1

wkhtmltoimage --format png http://10.10.90.24:31331/ /home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_screenshot.png


```