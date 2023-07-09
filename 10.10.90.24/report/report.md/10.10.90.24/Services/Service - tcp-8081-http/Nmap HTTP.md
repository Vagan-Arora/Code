```bash
nmap -vv --reason -Pn -T4 -sV -p 8081 --script="banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/xml/tcp_8081_http_nmap.xml" 10.10.90.24
```

[/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nmap.txt](file:///home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nmap.txt):

```
# Nmap 7.94 scan initiated Wed Jul  5 08:33:57 2023 as: nmap -vv --reason -Pn -T4 -sV -p 8081 "--script=banner,(http* or ssl*) and not (brute or broadcast or dos or external or http-slowloris* or fuzzer)" -oN "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/tcp_8081_http_nmap.txt" -oX "/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp8081/xml/tcp_8081_http_nmap.xml" 10.10.90.24
Nmap scan report for 10.10.90.24
Host is up, received user-set (0.16s latency).
Scanned at 2023-07-05 08:33:58 IST for 30s

Bug in http-security-headers: no string output.
PORT     STATE SERVICE REASON         VERSION
8081/tcp open  http    syn-ack ttl 60 Node.js Express framework
|_http-stored-xss: Couldn't find any stored XSS vulnerabilities.
|_http-date: Wed, 05 Jul 2023 03:04:11 GMT; 0s from local time.
| http-headers: 
|   X-Powered-By: Express
|   Access-Control-Allow-Origin: *
|   Content-Type: text/html; charset=utf-8
|   Content-Length: 20
|   ETag: W/"14-tVlBr0s73mf41Pi7C/1PMqiyXRc"
|   Date: Wed, 05 Jul 2023 03:04:10 GMT
|   Connection: close
|   
|_  (Request type: HEAD)
|_http-malware-host: Host appears to be clean
|_http-title: Site doesn't have a title (text/html; charset=utf-8).
|_http-jsonp-detection: Couldn't find any JSONP endpoints.
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-fetch: Please enter the complete path of the directory to save data in.
|_http-config-backup: ERROR: Script execution failed (use -d to debug)
|_http-aspnet-debug: ERROR: Script execution failed (use -d to debug)
|_http-wordpress-users: [Error] Wordpress installation was not found. We couldn't find wp-login.php
|_http-chrono: Request times for /; avg: 379.54ms; min: 343.31ms; max: 421.71ms
|_http-referer-checker: Couldn't find any cross-domain scripts.
|_http-wordpress-enum: Nothing found amongst the top 100 resources,use --script-args search-limit=<number|all> for deeper analysis)
|_http-csrf: Couldn't find any CSRF vulnerabilities.
| http-php-version: Logo query returned unknown hash 7a0764cca649f98ed5fedb60db4db182
|_Credits query returned unknown hash 7a0764cca649f98ed5fedb60db4db182
|_http-cors: HEAD GET POST PUT DELETE PATCH
| http-vhosts: 
|_128 names had status 200
|_http-dombased-xss: Couldn't find any DOM based XSS.
|_http-comments-displayer: Couldn't find any comments.
|_http-feed: Couldn't find any feeds.
|_http-devframework: Express detected. Found Express in X-Powered-By Header
|_http-mobileversion-checker: No mobile version detected.
| http-sitemap-generator: 
|   Directory structure:
|     /
|       Other: 1
|   Longest directory structure:
|     Depth: 0
|     Dir: /
|   Total files found (by extension):
|_    Other: 1
|_http-errors: Couldn't find any error pages.
|_http-drupal-enum: Nothing found amongst the top 100 resources,use --script-args number=<number|all> for deeper analysis)
| http-useragent-tester: 
|   Status for browser useragent: 200
|   Allowed User Agents: 
|     Mozilla/5.0 (compatible; Nmap Scripting Engine; https://nmap.org/book/nse.html)
|     libwww
|     lwp-trivial
|     libcurl-agent/1.0
|     PHP/
|     Python-urllib/2.5
|     GT::WWW
|     Snoopy
|     MFC_Tear_Sample
|     HTTP::Lite
|     PHPCrawl
|     URI::Fetch
|     Zend_Http_Client
|     http client
|     PECL::HTTP
|     Wget/1.13.4 (linux-gnu)
|_    WWW-Mechanize/1.34

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Wed Jul  5 08:34:28 2023 -- 1 IP address (1 host up) scanned in 30.80 seconds

```
