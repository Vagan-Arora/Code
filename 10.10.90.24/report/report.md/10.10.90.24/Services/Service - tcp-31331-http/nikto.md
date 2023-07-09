```bash
nikto -ask=no -Tuning=x4567890ac -nointeractive -host http://10.10.90.24:31331 2>&1 | tee "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_nikto.txt"
```

[/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_nikto.txt](file:///home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_nikto.txt):

```
- Nikto v2.5.0
---------------------------------------------------------------------------
+ Target IP:          10.10.90.24
+ Target Hostname:    10.10.90.24
+ Target Port:        31331
+ Start Time:         2023-07-05 08:33:59 (GMT5.5)
---------------------------------------------------------------------------
+ Server: Apache/2.4.29 (Ubuntu)
+ /: The anti-clickjacking X-Frame-Options header is not present. See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options
+ /: The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type. See: https://www.netsparker.com/web-vulnerability-scanner/vulnerabilities/missing-content-type-header/
+ No CGI Directories found (use '-C all' to force check all possible dirs)
+ /robots.txt: contains 1 entry which should be manually viewed. See: https://developer.mozilla.org/en-US/docs/Glossary/Robots.txt
+ Apache/2.4.29 appears to be outdated (current is at least Apache/2.4.54). Apache 2.2.34 is the EOL for the 2.x branch.
+ /: Server may leak inodes via ETags, header found with file /, inode: 17cc, size: 584b2b811ebb3, mtime: gzip. See: http://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2003-1418
+ OPTIONS: Allowed HTTP Methods: POST, OPTIONS, HEAD, GET .
+ /css/: Directory indexing found.
+ /css/: This might be interesting.
+ /images/: Directory indexing found.
+ /icons/README: Apache default file found. See: https://www.vntweb.co.uk/apache-restricting-access-to-iconsreadme/
+ 7702 requests: 0 error(s) and 10 item(s) reported on remote host
+ End Time:           2023-07-05 08:55:10 (GMT5.5) (1271 seconds)
---------------------------------------------------------------------------
+ 1 host(s) tested

```
