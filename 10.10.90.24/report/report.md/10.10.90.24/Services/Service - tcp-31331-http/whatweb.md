```bash
whatweb --color=never --no-errors -a 3 -v http://10.10.90.24:31331 2>&1
```

[/home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_whatweb.txt](file:///home/vagan/Music/CTF/THM/10.10.32.11  UltraTech/results/10.10.90.24/scans/tcp31331/tcp_31331_http_whatweb.txt):

```
WhatWeb report for http://10.10.90.24:31331
Status    : 200 OK
Title     : UltraTech - The best of technology (AI, FinTech, Big Data)
IP        : 10.10.90.24
Country   : RESERVED, ZZ

Summary   : Apache[2.4.29], Email[ultratech@yopmail.com], HTML5, HTTPServer[Ubuntu Linux][Apache/2.4.29 (Ubuntu)], Script

Detected Plugins:
[ Apache ]
	The Apache HTTP Server Project is an effort to develop and
	maintain an open-source HTTP server for modern operating
	systems including UNIX and Windows NT. The goal of this
	project is to provide a secure, efficient and extensible
	server that provides HTTP services in sync with the current
	HTTP standards.

	Version      : 2.4.29 (from HTTP Server Header)
	Google Dorks: (3)
	Website     : http://httpd.apache.org/

[ Email ]
	Extract email addresses. Find valid email address and
	syntactically invalid email addresses from mailto: link
	tags. We match syntactically invalid links containing
	mailto: to catch anti-spam email addresses, eg. bob at
	gmail.com. This uses the simplified email regular
	expression from
	http://www.regular-expressions.info/email.html for valid
	email address matching.

	String       : ultratech@yopmail.com
	String       : ultratech@yopmail.com

[ HTML5 ]
	HTML version 5, detected by the doctype declaration


[ HTTPServer ]
	HTTP server header string. This plugin also attempts to
	identify the operating system from the server header.

	OS           : Ubuntu Linux
	String       : Apache/2.4.29 (Ubuntu) (from server string)

[ Script ]
	This plugin detects instances of script HTML elements and
	returns the script language/type.


HTTP Headers:
	HTTP/1.1 200 OK
	Date: Wed, 05 Jul 2023 03:04:00 GMT
	Server: Apache/2.4.29 (Ubuntu)
	Last-Modified: Fri, 22 Mar 2019 18:06:50 GMT
	ETag: "17cc-584b2b811ebb3-gzip"
	Accept-Ranges: bytes
	Vary: Accept-Encoding
	Content-Encoding: gzip
	Content-Length: 2264
	Connection: close
	Content-Type: text/html



```
