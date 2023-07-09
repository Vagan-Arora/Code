```bash
feroxbuster -u http://10.10.90.24:8081/ -t 10 -w /root/.local/share/AutoRecon/wordlists/dirbuster.txt -x "txt,html,php,asp,aspx,jsp" -v -k -n -q -e -r -o "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_feroxbuster_dirbuster.txt"
```

[/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_feroxbuster_dirbuster.txt](file:///home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_feroxbuster_dirbuster.txt):

```
200      GET        1l        3w       20c http://10.10.90.24:8081/
200      GET        1l        8w       39c http://10.10.90.24:8081/auth
500      GET       10l       61w     1094c http://10.10.90.24:8081/ping
200      GET        1l        8w       39c http://10.10.90.24:8081/Auth
500      GET       10l       61w     1094c http://10.10.90.24:8081/Ping
200      GET        1l        8w       39c http://10.10.90.24:8081/AUTH

```
