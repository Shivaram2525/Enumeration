# NAME: SHIVARAM M.
# REG. NO: 212223040195
# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## OUTPUT:

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/90446958-be01-4f8b-aeda-c65f2b4bfbba)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## OUTPUT:

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/1f13ab3a-cbf8-4e72-92d0-4dfb2d2e3430)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## OUTPUT:

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/9f4a4d49-1b3e-440d-8b8d-7c91d8bb30f6)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## OUTPUT:

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/cc956e79-3d86-400a-bab8-064f155a9ab2)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## OUTPUT:
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/7cb576e7-5c94-4c58-beb3-367e5b7bffd0)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## OUTPUT:
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/d179c0dc-864e-410e-b4a3-d317c96d348d)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT:
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/59b709f0-6f94-414d-87a6-b9f655b6b97f)
 
# DNS Enumeration
## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/b53b2d1e-1a39-4b15-97d8-9e0b238f0d42)

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/b4f2a600-78e2-4605-b51f-9cf39786c7ed)


## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT:

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/3c737672-4643-423a-b41b-0bfa2262ebb4)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
## OUTPUT:

![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/c07b5298-9a16-41d8-805e-b6b751d0eda7)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/d6b3c192-6b97-41e8-a677-61b9cfc8f1a0)

select any username in the first column of the above file and check the same
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/6034435c-b383-491b-b814-f1a6b7e4548c)

# TELNET for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  ![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/b9dc406a-5fad-4d9c-9b83-66198a836fd2)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/Shivaram2525/Enumeration/assets/144226303/09441a1b-5281-4dd3-8ae3-f375af9be43e)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

