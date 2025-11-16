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


## OUTPUT:

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

![2](https://github.com/user-attachments/assets/4487db40-a71c-4fc6-a828-d0731fbaff21)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

![1](https://github.com/user-attachments/assets/0c4bab79-1915-4973-9f88-05d3f72da808)




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![10](https://github.com/user-attachments/assets/0c8a6e4e-93ad-4a73-a217-553d07e9496b)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![4](https://github.com/user-attachments/assets/04d2583d-51ee-4740-af20-af9b6a0b791b)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![6](https://github.com/user-attachments/assets/ac443ab1-a0a0-4cdb-b21b-d85c549f812c)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![7](https://github.com/user-attachments/assets/b568dffd-3d55-4d05-bf73-f94ba1e2d284)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![8](https://github.com/user-attachments/assets/4464ab03-aad2-4a2e-91cc-6ff29359fba0)



## DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![ss1](https://github.com/user-attachments/assets/15da5c4b-9d04-4a34-905d-18005002ff45)


![ss2](https://github.com/user-attachments/assets/b61d177d-43e8-4100-8e9c-32e543c24e83)


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

![ss3](https://github.com/user-attachments/assets/4baef516-0c41-4d8a-9581-632fe138e533)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

## OUTPUT:

<img width="939" height="474" alt="Screenshot 2025-11-16 163612" src="https://github.com/user-attachments/assets/408417cc-0fff-4d8e-bbda-64a78771b689" />

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

## OUTPUT:

<img width="723" height="266" alt="image" src="https://github.com/user-attachments/assets/2aedc145-cb11-4c9f-9310-55b1ea905709" />

select any username in the first column of the above file and check the same

## OUTPUT:

<img width="966" height="492" alt="image" src="https://github.com/user-attachments/assets/0cb0ad54-9b46-4644-9183-d7cd3e7f81d1" />

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## OUTPUT:

<img width="967" height="383" alt="image" src="https://github.com/user-attachments/assets/8e3ba183-b498-4e23-8cc7-bf4221dab885" />
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

<img width="637" height="171" alt="image" src="https://github.com/user-attachments/assets/052e7636-1476-4fce-916d-94f1b4b892bb" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
