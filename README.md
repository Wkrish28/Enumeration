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

<img width="1917" height="1027" alt="Screenshot 2026-02-05 080849" src="https://github.com/user-attachments/assets/168efea1-368c-4f09-ae3d-a020ccc934aa" />
site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

<img width="1919" height="1022" alt="Screenshot 2026-02-05 080951" src="https://github.com/user-attachments/assets/edb6744e-8062-403c-9381-2ec78456c7d8" />
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com


<img width="1915" height="1027" alt="Screenshot 2026-02-05 081431" src="https://github.com/user-attachments/assets/4442fd5b-183d-41d5-b9c6-0df0b3290d26" />
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1919" height="1025" alt="Screenshot 2026-02-05 081556" src="https://github.com/user-attachments/assets/758c2a20-1b84-4a06-a0e5-2e3c7bea74ed" />
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img width="1919" height="1029" alt="Screenshot 2026-02-05 082026" src="https://github.com/user-attachments/assets/a5623bb9-f6cd-4e31-a991-fedea63cae86" />
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="1919" height="1022" alt="Screenshot 2026-02-05 082127" src="https://github.com/user-attachments/assets/3cc46520-a014-4aea-9fd5-6d8fdd5d2c73" />
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

<img width="1919" height="1021" alt="Screenshot 2026-02-05 082449" src="https://github.com/user-attachments/assets/5b516d6b-1e1b-4933-8ff3-eed72f056ac8" />
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="1218" height="1079" alt="Screenshot 2026-02-05 083340" src="https://github.com/user-attachments/assets/ed91cb44-a56f-4aa4-ae18-84b1a3604657" />

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
<img width="831" height="1012" alt="Screenshot 2026-02-05 093329" src="https://github.com/user-attachments/assets/cdb81b5e-1e25-4407-b8f0-175c7ad714d9" />
<img width="816" height="932" alt="Screenshot 2026-02-05 093353" src="https://github.com/user-attachments/assets/b1cd5ba0-cd83-4d5b-88e6-6b67f53fc1b0" />


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
<img width="719" height="397" alt="image" src="https://github.com/user-attachments/assets/32a41285-cab4-4ecd-81d0-70fcc4147913" />

select any username in the first column of the above file and check the same
<img width="636" height="450" alt="image" src="https://github.com/user-attachments/assets/8c69ffe6-700a-4672-b2ec-915f42ee8b0b" />


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
 <img width="638" height="608" alt="image" src="https://github.com/user-attachments/assets/97b8221e-7b28-427d-88dd-a37ebcf1bd89" />

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
<img width="955" height="197" alt="image" src="https://github.com/user-attachments/assets/f8b132cb-1864-41c0-8aad-8e1a8fd7d74a" />



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

