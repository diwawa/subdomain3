Subdomain3

![language](https://img.shields.io/badge/version-2.0-green.svg)  ![[stars](https://img.shields.io/github/stars/yanxiu0614/subdomain3.svg) ![[forks](https://img.shields.io/github/forks/yanxiu0614/subdomain3.svg)  ![language](https://img.shields.io/badge/language-python2%2B-green.svg) ![language](https://img.shields.io/badge/language-python3%2B-green.svg)

Subdomain3 is a new generation of tool , It helps penetration testers to discover more information  in a shorter time than other tools.The  information includes subdomains, IP, CDN, and so on. Please enjoy it.

##Screenshot
medium pattern for speed
![](screenshot.png)

##Features
* More quick
Three patterns for speed. User can modify the configuration(/lib/config.py) file to speed-up.
* CDN support
Determines whether the subdomain  uses CDN storage by searching list of CDN severs.
* RFC CIDR
Sorting ip and report CIDR(example 1.1.1.1/24)
* Multi-level subdomain support
Discover more subdomains,example:admin.test.xx.com
* Big dict support
Million of subs support
* Less resource consumption
1 CPU/1GB Memory/1Mbps bandwidth

###Getting started

```
sudo apt install git
git clone https://github.com/yanxiu0614/subdomain3.git
pip install -r requirement.txt
```
### Usage

Short Form    | Long Form     | Description
------------- | ------------- |-------------
-d            | --domain      | domain name,for example:baidu.com
-s            | --bruteforce  | Enable the subbrute bruteforce module
-l            | --level       | example: 2:baidu.com; 3:world.baidu.com;
-f            | --file        | The list of domain

###change log:

2017-10-11:Rebuild part of the code; api support; result is more readable；update cdn-severs；faster

2017-6-17: delete universal parse opthon(-p t/f);add a file of config;optimze strategy for universal parse

2017-5-2: add a module(validate the domain),please modify "result_name" in the validate_domain.py if you will use it;fix universal bug;update cdn-servers,etc

2017-4-21: optimze strategy for generating subname，improve the speed

2017-3-23: add universal parse opthon(-p t/f)

2017-3-17: big dict support(for example: two million)

2017-3-10: read several domains from file support(-f domains) support;update cdn-servers

2017-2-26: multilevel domain support(no upper limit);big dict support;take up about a third to a quarter as much memory; faster

2017-2-24: mac support