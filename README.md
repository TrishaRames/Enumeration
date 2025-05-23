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

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/user-attachments/assets/4f9f5fa8-c88b-413e-ae79-fd1e0bebb90e)

![image](https://github.com/user-attachments/assets/f1d69ce3-8c48-4aaa-ba01-5f353c8cc3ac)


![image](https://github.com/user-attachments/assets/da9f1d95-8140-45ee-9a63-9e5aceaf6e4e)

![image](https://github.com/user-attachments/assets/7ca9e60f-9498-4fa6-b7fc-87608e2996b2)

![image](https://github.com/user-attachments/assets/1c8b8ad9-72dc-451f-9164-841131c7d371)

![image](https://github.com/user-attachments/assets/48286c59-8b71-4a70-a663-17d73554f292)

![image](https://github.com/user-attachments/assets/30bd6bc8-5e15-46ba-8250-e7aa288b81bd)

##dnsenum
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
![image](https://github.com/user-attachments/assets/ef2f0650-3ae2-4a38-aabb-acbc48016f9a)

![image](https://github.com/user-attachments/assets/fba5bd1d-d855-46fb-8841-872e15c153e7)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
![image](https://github.com/user-attachments/assets/9fb05bb0-fbcb-4ae4-9c8e-be1e52191452)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  ![image](https://github.com/user-attachments/assets/f30a68ff-081a-44d7-8ed7-dcfd3f9b10d0)

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/user-attachments/assets/97d79817-b6ac-49f5-974a-0670b70dbaa9)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

