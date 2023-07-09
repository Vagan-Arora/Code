```bash
nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://10.10.90.24:8081 2>&1 | tee "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nikto.txt"
```

[/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nikto.txt](file:///home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nikto.txt):

```
- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          10.10.90.24
+ Target Hostname:    10.10.90.24
+ Target Port:        8081
+ Start Time:         2023-07-05 08:33:59 (GMT5.5)
---------------------------------------------------------------------------
+ Server: No banner retrieved
+ /: Retrieved x-powered-by header: Express.
+ /: Retrieved access-control-allow-origin header: *.
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ /auth/: This might be interesting.
+ /#wp-config.php#: #wp-config.php# file found. This file contains the credentials.
+ 7711 requests: 10 error(s) and 6 item(s) reported on remote host
+ End Time:           2023-07-05 08:54:32 (GMT5.5) (1233 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested

```
