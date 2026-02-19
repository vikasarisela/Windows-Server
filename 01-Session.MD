How big your environment ?
Explain about infra you worked ?
Infra:
========
How many Forest 
How many Domain 
How Domain controllers
How many Sites 
How to build Trust  in  (multi domain )








Class 00
Single Forest, single domain, single site , 2 domain controllers you can manage 1000 emp, 1000 computers and 1 file server 
First 5 class 
7 servers required for the lab 
4gb ram and 2 cpu for each machine , 50gb ssd 


Class 1 

You have worked has windows desktop support and moving to next level
After this course your job would be 
System Administrator
Server Admin :
IT-support 
Operational spec:

M-Infra Ops Spec
===============================

Why we need to Learn  Windows Server OS ?


Windows admin will managing the on premises infra level 
Desktop support will be managing end users 
All users and computer must be present in AD

Two Environment IT (Any business)
Infrastructure and End user  



Infrastructure(Windows Admin)                           End user (Desktop Support will manage)
====================================================
What purpose  Server OS  ?                                                     All Employee   where they use laptop 
 To create AD -> Server OS                                           Laptop (Win10 or Win11 ) Client OS 
 DB                                                                they    Login : Domain user  (user is created in Local computer ?)
 Application				and All users and computers must be present in AD(infra)
 Printer 
File server
Windows Cluster 
DNS 
DHCP 
WSUS

After completing this course you will be managing the infrastructure like AD, DB, Application, Printer, File Server, Windows Cluster, DNS, DHCP
WSUS
 System admin should know all the infra level  
                 
As a Windows Admin We must know About server :
How you will install all the ad , db , application , printer …, there is a process called Role , if you want to install all the products you
Role 
You must install specific Role 

Every System Admin should know l1, l2, l3 AD knowledge  


A directory is a hierarchical structure that stores information about objects on the network.
 A directory service, such as Active Directory Domain Services (AD DS), provides the methods for storing directory data and making this data available to network users and administrators. For example, AD DS stores information about user accounts, such as names, passwords, phone numbers, and so on, and enables other authorized users on the same network to access this information.

From <https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview> 



From <https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview> 

Active Directory (AD) is a directory service developed by Microsoft to manage and organize network resources, such as users, computers, and other devices, in a centralized way. 
It allows administrators to control access to resources, apply security policies, and manage permissions across a network. 
AD is commonly used in enterprise environments to simplify the management of IT infrastructure.
What is Active Directory?
Active Directory (AD) is a database and set of services that connect users with the network resources they need to get their work done.
The database (or directory) contains critical information about your environment, including what users and computers there are and who’s allowed to do what. For example, the database might list 100 user accounts with details like each person’s job title, phone number and password. It will also record their permissions.
The services control much of the activity that goes on in your IT environment. In particular, they make sure each person is who they claim to be (authentication), usually by checking the user ID and password they enter, and allow them to access only the data they’re allowed to use (authorization).
Active Directory simplifies life for administrators and end users while enhancing security for organizations. Administrators enjoy centralized user and rights management, as well as centralized control over computer and user configurations through the AD Group Policy feature. Users can authenticate once and then seamlessly access any resources in the domain for which they’re authorized (single sign-on). Plus, files are stored in a central repository where they can be shared with other users to ease collaboration, and backed up properly by IT teams to ensure business continuity.



Server is empty , until you install specific role 
Server is  empty  and when you install an Active Directory DS  it becomes domain controller 
Specific role ->  
AD -> Domain controller :BNGDC01  BNGDNS01
DNS
DHCP
You should know 
1.Installation and configuration of roles on server 
2.Performing(you should know how it is performing , if something goes wrong we should have knowledge on AD, dhcp, dns ) 
3.Log 
4.basic checklist need to verify you should know to verify is it working or not step by step 
You should current IT environment OS Version  
Microsoft stopped support for 2008 OS so Microsoft will not release patches

Read day 1 PowerPoint for basic os interview questions

----------------------------------------------------------------------------------------
LAB Installation of DC1
We have deploy OS - win2019 server 
From 2016 they are using dashboard
1.Dashboad - Category you can see below 
  Events,services,BPA,roles and features 2012 features introduced
  BPA - Start BPA Scan it will check the roles is properly installed. (best practice analyzer), it will tell the best practices as per the Microsoft
recommendations
  22 Roles are in  2019 

    2. Configure this local server 
     add roles and features
     add server to manage -> you can add server to manage not to go to central server and connect rdp 
    Server group -> you can create server group like wintel- dns, dhcp and dhcp server group 
    Connect to the cloud service -> you can connect to the cloud service like azure.

2.New Features 
3.Count of Roles
4.WIll install one of The role called AD

------------------------------------------------------------
Must read active directory
https://en.wikipedia.org/wiki/Directory_service

Active Directory stores data as objects. An object is a single element, such as a user, group, application or device such as a printer. Objects are normally defined as either resources, such as printers or computers, or security principals, such as users or groups.
Its primary purpose is to provide a centralized location for managing and administering network resources, including users, computers, printers, and other network devices.

Active Directory (AD) is a directory service developed by Microsoft for Windows domain networks.
Its primary purpose is to provide a centralized location for managing and administering network resources, including users, computers, printers, and other network devices. Here are some key purposes and functionalities of Active Directory:

1. **User Authentication and Authorization**: Active Directory provides authentication and authorization services, allowing users to log in to the network using their credentials (username and password) and granting them access to resources based on their permissions.

2. **Centralized Management**: It offers a centralized and hierarchical structure for managing network resources, making it easier for administrators to control access rights, group memberships, and other configurations from a single point.

3. **Security**: Active Directory helps enforce security policies across the network, such as password policies, account lockout policies, and group policies, ensuring the security and integrity of network resources.

4. **Resource Management**: It simplifies the management of various network resources like user accounts, computers, servers, printers, and applications, by organizing them into logical containers called Organizational Units (OUs).

5. **Single Sign-On (SSO)**: Active Directory supports single sign-on functionality, allowing users to access multiple network resources with a single set of credentials, enhancing user experience and productivity.

6. **Group Policy Management**: It enables administrators to define and enforce policies across groups of computers and users, ensuring consistency and compliance with organizational standards.

7. **Directory Replication**: Active Directory replicates directory information between domain controllers, ensuring high availability and fault tolerance for directory services.

8. **Integration with Other Services**: Active Directory integrates with various Microsoft services and applications, such as Exchange Server, SharePoint, and Office 365, providing seamless access and management of these resources.

Overall, Active Directory plays a crucial role in simplifying network administration, enhancing security, and improving user productivity within Windows-based environments.





What is AD ?
Identity with secure manner (Security DB  for users and computers)
How AD Works ?
When you enter a company you need ID card or else security will stop , if user has identity then only he can enter , identity will be validated in AD 
Identity is required to login into computer ie user name and password
To run IT business we need 
Security and 
Centralized Administration means how many users and computers are there we can track 
AD is used to manage users, computers, groups , group policies , ou centrally 

For AD there is a structure way
First time when you build AD , it becomes forest and logically created name is called Domain , and the domain it creates a DC and site 



Here’s a structured learning guide on Active Directory (AD) that can be posted on GitHub:

Understanding Active Directory (AD)
What is Active Directory (AD)?
Active Directory (AD) is a directory service developed by Microsoft for Windows domain networks. It is used to manage network resources such as users, computers, groups, and other network devices in a secure and organized manner.
Key Concept:
    • Identity Management: AD acts as a security database for storing information about users, computers, and other network objects. It ensures that only authorized users and devices have access to network resources.
    • Centralized Administration: AD allows for centralized control over networked resources, making it easier to track and manage users and computers.

How Active Directory Works?
Think of Active Directory as a security checkpoint for your IT environment. Here’s a simple analogy:
    • Entering a Company: When you join a company, you need an ID card to enter the building. If you don't have the card, security will stop you. Similarly, when a user needs to log into a network, their identity must be validated to ensure they have proper access rights.
    • Validation: When you log into your computer, username and password are your credentials. These credentials are verified by AD, and if valid, you are granted access to the system.
How is this security implemented?
    • Security Database: AD acts as a secure database where user credentials (username and password) and access control information are stored.
    • Identity Management: AD ensures that users are authenticated, authorized, and assigned proper access rights to network resources.

Why Do We Need Active Directory?
To run a smooth and secure IT environment, we need two key components:
    1. Security: AD ensures that sensitive data and network resources are protected from unauthorized access.
    2. Centralized Administration: With AD, you can track and manage the number of users, computers, groups, and more, from one central location.

What Does Active Directory Manage?
Active Directory is used to centrally manage the following:
    • Users: Information about each user account, including username, password, group memberships, and permissions.
    • Computers: Information about each computer on the network, including its name, operating system, and permissions.
    • Groups: Logical collections of user accounts, which simplify the management of access permissions.
    • Group Policies: Rules for how computers and users should behave within the network (e.g., password policies, desktop settings).
    • Organizational Units (OUs): Containers that help organize users, computers, and other resources in a hierarchical structure.

Active Directory Structure
When you first build Active Directory, it follows a structured approach:
    1. Forest: The top-level container in AD. It represents the entire directory structure and can contain multiple domains.
    2. Domain: A logical container within the forest. A domain is identified by its domain name (e.g., example.com) and acts as a boundary for the management of users, computers, and other resources.
    3. Domain Controller (DC): A server that holds a copy of the Active Directory database and manages authentication requests within a domain. When a domain is created, a Domain Controller (DC) is automatically created to handle the management of that domain.
    4. Sites: Physical locations that represent network subnets, which help AD control the replication of data between domain controllers and optimize the use of network bandwidth.

How Active Directory Supports IT Business Needs
For any organization to function smoothly, it is essential to ensure:
    1. Security: AD ensures that only authenticated and authorized users can access specific resources.
    2. Centralized Administration: With AD, administrators can easily manage a large number of users and computers, assign permissions, and track resources, ensuring efficient management of IT infrastructure.




Pre-Req installing and configuring AD
================================
1.Must be configured static IP and DNS : (IP - dynamic -exception) But DNS must be configured static
2.Computer name must be renamed => DC1
3.Administrator password must be reset => by default it is disable (compmgmt.msc --> local users and groups --> Administrator enable)
4.C: drive must be NTFS format 

Configure Role
Install ADDS and DNS Role 
Server manager -- > role ->  select adds and dns , with this dependencies will be installed 
Next promote server to DC
For the first time you will be installing forest 
And it will ask for root domain name (domain name with . You have to add  for ex nee.edu)
Forest name and domain name are same 
By default there will be one forest and one domain will there 


Next  it will ask for AD functional level 
You installed OS is 2019  and AD functional level  can be select previous AD functional ie   (2008,2008R2,2012,2012R2,2016)

Two are :  read online about diff b/w forest and domain level 
Forest level -> functionality   Central govt   
So whatever the central govt assign roles It will be applicable for all the states 
Whatever the functionalities are applied at forest level , it will be applied to all the domain in a forest
Roles can define individual domain 
Domain level -> Functionality  State Govt
At state level you can define your own role 
For example 
If you selected 2008 at forest level ,whatever the AD Related functionality update  it will be updating at domain level and cannot expect new feature other than 2008 
You have 2019 OS on top of that you are building infra , now you selected forest functional level 

Interview Question 
Difference between forest and domain level functionality 

DSRM  password - whenever you want to restore ad object 
DSRM stands for Directory Services Restore Mode, which is a special boot mode in Microsoft Windows operating systems used for repairing or restoring Active Directory (AD) data or domain controllers.
The DSRM password is crucial for accessing the Directory Services Restore Mode and performing recovery tasks in scenarios such as:
1. Directory Service Restore: When restoring Active Directory from backup, you may need to boot into DSRM to perform authoritative or non-authoritative restores.
2. AD Maintenance and Repair: DSRM can be used for tasks such as offline defragmentation of Active Directory databases or repairing AD-related issues.
3. Active Directory Troubleshooting: In some troubleshooting scenarios, booting into DSRM may be necessary to diagnose and resolve directory service problems.

What is NETBios
NETBIOS (Network Basic Input/Output System) is a networking protocol suite developed by IBM in the early 1980s. It provides services for communication between applications running on different computers within a local area network (LAN).
Name Resolution: NETBIOS facilitates the resolution of computer names to their corresponding network addresses (IP addresses) within a LAN. It allows computers to identify each other by name rather than relying solely on IP addresses.
Broadcasting: NETBIOS enables broadcasting of messages within a LAN, allowing computers to send messages to all other computers on the network. This is often used for service discovery or network announcements.
NetBIOS Names: NETBIOS names are limited to 15 characters and are used to identify resources such as computers, printers, and shared folders on a network.

AD Database path  NTDS , log  and sysvol will be installed 
By default AD database is called NTDS
In production the path will be different 




Post checklist : After installing AD  (most imp services after building AD)
-----------------------------------------------
The below 2 things to do after installing ADDS
1.Check AD related Services 
 (IQ what are AD related services ?)  (go to services  and select ADDS  and check the installed services)

Netlogon
ADDS(ntds)
KDC
DNS

Check the below Services
netlogon  -> it is used to login into computer like it will establish connection b/w server and client (if this service
 stops the communication doesn’t happen)   (it is everywhere in client computer also there )
   ADDS is a display name (NTDS is a service name)  if this service stops the user will not able to login into n/w



Kerberos is a network authentication protocol designed to provide strong authentication for client/server applications by using secret-key cryptography.
It was developed by MIT and has become the default authentication protocol for many networks, including Microsoft Active Directory domains.


The Key Distribution Center (KDC) is a central component of the Kerberos authentication system. It consists of two main parts:
Authentication Server (AS): The Authentication Server is responsible for initial authentication. It verifies the identity of clients and issues Ticket Granting Tickets (TGTs) upon successful authentication.
Ticket Granting Server (TGS): The Ticket Granting Server is responsible for issuing service tickets. Clients request service tickets from the TGS to access specific services on servers.
In summary, Kerberos provides secure authentication for client/server applications by using symmetric key cryptography and a trusted third-party authentication server, known as the Key Distribution Center (KDC). The KDC consists of an Authentication Server (AS) for initial authentication and a Ticket Granting Server (TGS) for issuing service tickets.


KDC (Kerberos key distribution center)  it will manage secure channel b/w server and client
  AD  uses Kerberos authentication protocol  : 88  (authentication purpose used protocol KDC)
    AD  run the query the protocol called LDAP (ldap protocol port no is 3389)
Every query goes to ldap and port 3389
  AD works on LDAP 
Every query goes to the port number 3389 ie LDAP 
  When you run query there are 2 protocols 
GC: 389
LDAP : adsiedit.msc
Click on connect 

AD Uses Kerberos Protocol for secure authentication 

--------------------------------------------------------LDAP --------------------------------------------------------------------------
Active Directory (AD) and LDAP (Lightweight Directory Access Protocol) are closely related, but they serve different purposes and have distinct characteristics. Here's a breakdown of their relationship:
1. LDAP is a Protocol, AD is a Directory Service:
    • LDAP (Lightweight Directory Access Protocol): It is a protocol used for accessing and managing directory services over a network. LDAP defines how clients can query, search, and update directory information, which typically includes user accounts, groups, and other resources. It is a lightweight version of the Directory Access Protocol (DAP) and operates over TCP/IP.
    • Active Directory (AD): Active Directory is a directory service developed by Microsoft. It is a database and a set of services that stores and organizes information about objects in a network, such as users, groups, computers, and other resources. AD provides centralized management and security for these objects in a network, especially in a Windows environment.
2. AD Supports LDAP:
    • Active Directory uses LDAP as one of the primary protocols to allow clients to query and manipulate the directory information. Specifically, when a client makes an LDAP request to an AD server, the AD server responds based on its directory data.
    • AD also uses LDAP for various tasks like: 
        ○ User authentication and querying user information.
        ○ Searching for objects like users and groups.
        ○ Modifying directory entries.
3. Additional Protocols in AD:
    • Besides LDAP, Active Directory also uses other protocols like Kerberos for authentication and DNS for domain name resolution. While LDAP handles directory lookups and updates, Kerberos handles secure authentication.
4. LDAP as an Open Standard:
    • LDAP is an open standard and can be used to access directory services from different vendors (not just Microsoft). It is implemented by various directory services like OpenLDAP, Novell eDirectory, and others.
    • Active Directory is a proprietary service from Microsoft, but it uses LDAP as a communication protocol, allowing compatibility with other LDAP-compliant systems and applications.
5. Example of AD & LDAP Interaction:
    • When you want to search for a user in an Active Directory domain, you might use an LDAP query to locate the user's information (e.g., username, email address, group membership). The AD server will use the LDAP protocol to return the requested information.
6. Security and Permissions:
    • AD includes security features that allow fine-grained control over permissions and access to directory objects. While LDAP itself provides the mechanism for directory access, AD implements security policies, including user roles, permissions, and auditing.
In Summary:
    • LDAP is the protocol used to query and update directory information.
    • Active Directory is a directory service that uses LDAP as one of the primary communication protocols to interact with directory data.
AD's use of LDAP allows it to function as a highly scalable, queryable, and manageable directory service for large networks, particularly in Windows environments.

From <https://chatgpt.com/> 

Tools for Executing LDAP Queries:
LDAP queries can be executed using a variety of tools and libraries:
    • Command Line: Using tools like ldapsearch (on Unix/Linux) or dsquery (on Windows).
    • Programming Libraries: Most programming languages provide LDAP libraries (e.g., ldap3 in Python, JNDI in Java, or pyldap).
    • Graphical Interfaces: Tools like Apache Directory Studio or LDAP Admin offer a GUI to execute queries.
    • PowerShell: In a Windows environment, PowerShell scripts can be used to run LDAP queries against Active Directory


Of course! Imagine LDAP as a phone book for computers and other network devices. 

1. **Phone Book**: Just like a phone book helps you find people's phone numbers and addresses, LDAP helps computers find information about other computers, users, and resources on a network.

2. **Organization**: In a phone book, information is organized alphabetically by names. Similarly, LDAP organizes information in a hierarchical manner, like folders within folders, making it easy to find what you need.

3. **Search and Retrieve**: If you want to find someone's phone number in a phone book, you'd look them up by their name. Similarly, LDAP allows computers to search for specific information, like a user's login credentials or email address.

4. **Centralized Management**: Just as a phone book is a centralized place for storing contact information, LDAP provides a centralized way to manage information about users, groups, computers, and other resources on a network.

5. **Security**: LDAP ensures that only authorized users can access certain information, just like how some phone numbers may be listed as private in a phone book.

In essence, LDAP is like a smart, organized phone book for computers and network resources, making it easier for them to find and interact with each other on a network.

LDAP stands for Lightweight Directory Access Protocol
LDAP is commonly used for centralized management of user authentication, authorization, and directory services in a network environment.
Here are some key aspects of LDAP:
Directory Services: LDAP is designed for accessing and managing directory information services, which typically store information about users, groups, computers, printers, and other network resources. These directory services provide a hierarchical structure for organizing and storing data in a directory tree format.
Client-Server Architecture: LDAP follows a client-server model, where LDAP clients (applications or services) interact with LDAP servers to perform directory operations. Clients send LDAP requests to servers, which process these requests and return responses containing the requested information.

AD as an LDAP Directory: Active Directory, developed by Microsoft, is a directory service used primarily in Windows environments for managing network resources such as users, groups, computers, and printers. 
AD is built upon LDAP and implements the LDAP protocol as one of the primary means for accessing and querying directory information.

----------------------------------------------------------------------------------LDAP --------------------------------------------------------------------------------

2.Check AD tools are correctly updated 
  1. AD users and computers : dsa.msc (where you can see domain name and how many domain controllers are there  )
2.   To check how many domain controllers and sites are there in domain you can use gpmc.msc  (group policymanagment console)
  To check how many domain are there in forest (right click on domain --> show domains)
  this is how you read your infra, youll be knowing multi or single domain environment and each domain you can have multiple sites and they all are within the domain.
3.   AD sites and service  : dssite.msc
 4.  AD domain and trust : domain.msc
   AD powershell module 
   AD administrative center 

You create any object that must be replication all the DC by default within the domain 

To read infrastructure   
Run Gpmc.msc - where you can see all forest and domains. (right click and click show domains)
   ADIEDIT
   Group policy 
You can rename  default at first site to BNG ie DC1 primary DC 

3.DNS : DNS IP : its changed to 127.0.0.1 
        We need to reconfigure : 10.128.0.2 (it's is your machine IP)

4.How many Forest ? 1
   neel.edu  
  How many Domain ? 1
   neel.edu 
  How many DC1  ? 
   dc1.neel.edu 
 How many sites ? 1 (Default-first-site)

gpmc.msc => forest name 
            Expand domain => RC => show domain : 

Each domain can having multiple sites and DC :
If you multiple domains and sites all the objects needs to replicated.

Observer when you change DNS name it will change to domain name on network adapter
The above all are L2 level basics

Sites name is the place where your business runs so replace with Bangalore
For example I have another location Chennai and have no DC there and I am authentication with Bangalore dc  via WAN
What if n/w is down in Chennai location all users will not able to login and solution is build dc locally 
When you talk about new dc you need to add site.

 
Class 2
---------
BNG - Default first site 
1 DC 
5000 users 
5000 computers

What if DC is down
As per Microsoft recommendations 2 DC's are required always recommended.
Additional DC.

Recap:
=======
1.Why we need MS-windows server 
2.Infra level we need server 
3.Client OS
4.Server OS
5.Family of server OS 
6.Released date current OS details 
7.win2008,win2012,win2016 and win2019 server OS
9.Whats new (features)
10.LAB - GCP registration - build the server in Google cloud
11.Pre-req to build server in GCP (name,region,zone,hardware configuration,boot image ,allow access,http and https enable)
12.How to RDP server (external /Public IP)
13.How reset the password 
14.We have connected the server and logged in to the server 
15.Dashboad,all 5 steps : localserver,Roles and fetures,connect and manage ,Create group ,clould    connect 
16.BPA (Best practice analyser)
17.How many roles in Server 2019 (22 role)
18.what is AD, AD infra 
19.WHat is Forest,DOmain,Site and DC
19.Pre-req installing AD
20.We have installed and configured ADDS and DNS  -Forest and Domain functional
21.Post check AD
22.Service (Netlogon,ADDS-ntds,KKDC,DNS)
23.WHat is my AD infra where to check Forest and domain details (gpmc.msc)
24.How many sites ? how many DC's (dsa.msc -DC -> Dc namd Site)
25.renamed site (dssite.msc -active directry sites and service )

=============================================================================
what is infra ?
Single forest 
single domain 
SIngle site 
Single Domain controller

Default-first site - > BNG 

BNG -location 
1-DC -Down ?
5000 users 
5000 computer

Microsoft -recommendation /Best practice :
each site  must be required 2 DC
Additional domain controller 

learning
How to build Additional DC  and How its replicating to each other 
Once the additional DC is created each other should replicate by default automatically 
Very IMP: the DCs within the site or b/w the site must replicate each other within the Domain.
Why replication should be done for the DC's  within the site and b/w the sites ?
It’s the same database is shared , domain controller is the boundary 
we will create some object (users ,group in DC1)

DC1 --> 10.128.0.2
ClientPC --> 10.128.0.2
ADC --> 10.128.0.4 
CHNDC  --  10.142.0.2

Lab - 
Creating OU's within BNG OU
 create IT and Sales OU
IT - within IT OU create user bng_it_001 (domain user)
Sales- within sales OU create user bng_sales_002
Creating Groups within BNG OU
BNG_Groups
BNG_Sales
Lab - Create windows 10 client1 new OS 
How to make member of AD joining to domain.
we need configure  - DNS (Root DNS IP -10.128.0.2)
My -computer -> Properties -> domain-> azurevicky.com
After adding computer to domain azurevikas.com, you will see client1 in computers 
Join the client pc with domain user
And you can login with user created in IT and Sales OUs
You can make user to login in specific hours 
When users are added in remote desktop users security group, the user unable to logging in 
So login with admin into client1 and add users to rdp 
-> domain user has limited access.

We have created OU, Groups and Users in DC1 (users -bng_it_001 and bng_sales_001)
Exception -GCP (in Client machine - we need to those users add in Remote desktop users )
 We have logged with domain user to client machine 
we have verified -> logon to and logon hour -centrally we are managing 
You can make user to login at specific hours 
Go to user properties -> Account --->  logon hours  (logon permit and logon denied )

56:50 
What if the DC1 goes down --> we need to build additional ADC in same region

Two Objects will authenticate to DC 
Users  --> to check user which domain controller authenticated is (set l)
Computers --> nltest /dsgetdc:  (to check the computer authenticated to which DC)
Which  domain user is authenticated 
Cmd:  To check win + R set l 
Cmd :Which  domain,  computer is authenticated 
Computer :    nltest /dsgetdc:

Command  "hostname" to check device name 

Lab - Creating additional ADC    ADC name - same site ie BNG.
ADC is a backup domain controller 
    We need to build ADC -> same region 
    connect ADC server 
    change administrator password 
    configure DNS IP 
    Install and configure role -ADDS and DNS
    It will ask to replicate from then select dc1.azurevikas.com
    Add dc to existing domain. 
    
    Have to select which DC you want to replicate 
    
    Create one user in adc users-bng_it_002 then check it is replicated in dc1 
    
    Now the replication is happening in 2 way b/w dc's
    
    To see the domain controller primary or backup 
    You can type command net accounts
    
    
How to check the DC is primary or backup ?
Net accounts , if the role is backup then that is adc 
Type net accounts and check computer role for adc it shows backup
Now we have created 2 domain controllers dc1 and adc

--------------------------------------------------DC and ADC finished creating within a site BNG  ------------------------------------

1:36
Now think your business is expanded and you're in other location Chennai but the problem is while authenticating via 
WAN to Bangalore site there is latency. So with
We will build new DC in chennai location 
To do that we can create multiple sites in a domain 
AD infra 
to create a site it  must require Subnet (Network address -CHN) 
10.130.10.0/24
Bangalore subnet is 10.128.0.0/24
Apart from Any new site created(ie 
Default-first-site - BNG  ) , 
 we must create Subnet :

What we will learn ?
we will build new server - in different region -> 
How to create new site 
how to create new subnet 
how replicating happens  between the sites


Replication 
----------------
there are two type of replications 
1. Intra site => Replication happening within site (between Domain controller's)
                 Replication time interval - immediate 3 sec
2. Inter site => Replication happening between the sites (Between two or more site - in existing domain)          
                 Replication time interval -default 180 min (3hrs) you can set it to min 15min


IMP in Production  Class 2 time 1:36
------------------------ LAB
Building new dc for chennai region chndc where user can authenticate locally avoiding 
Authentication with Bangalore dc via WAN
Within a domain we can create multiple site
To create site it must require subnet because Chennai site different n/w 
How you will be knowing dc belongs to different n/w -> you have to refer to subnet
Other than default first site(BNG) we must create subnet.

1. Build new VM - in different region 
2.go to Rootdc ie DC1 -DC: dssite.msc
   2 Important Points
 => create site(CHN)(right click on site and new site) and select "DEFAULTSITELINK"
Defaultsitelink by default given by microsoft to link sites and communicate
 =>(1:47) create subnet (right click on subnet and give 10.142.0.2 (Subnet -10.142.0.0/24), it is given based on topology given by network admins) and select created CHN Site
BNG and CHN are 2 diff n/w's , how he knows this dc belongs to chennai, he refer to the subnet
Default site link is to connect b/w two site bng and Chennai site
Any new site when creating --> we must create subnet 
By default microsoft has given default site link, with this you are going to communicate b/w BNG and CHN
Create a default site Link b/w bng and chn, it is to communicate b/w bng and chn 
Default site link uses rpc over tcp/ip, where active sites going to transfer the data 
Create subnet for created site expect the default site.
Right click on the new site and give CHN




4.go to chndc -> login -> reset administrator password
5.configure root DNS IP (10.128.0.2) 
6. Make a member of this server (my computer -properties -> domain)
7.Login domain administrator 
8.Install and configure ADDS and DNS 
9.While configure this CHNDC - belongs to CHN
10.Once Deployment completed 
11.Veryfy all object must replicated (compare with DC1 to CHNDC)

Create one OU in chndc and other OU called IT 


Time replication like 15 mins 
How to check my replication is happening b/w chennai and Bangalore  site
Go to dc1 -> dscsite.msc -> inter site transports -> IP -> defaultipsitelink -> replicate every 15 mins you can change and you can schedule replication




You can do manual replication as will if you don’t want to wait for 15 mins
Manual replication : dssite.msc in chndc-> site-> server->NTDS settings -> click automatic generated->Right Click - replicate now


DC1,ADC and CHNDC
DC1 -BNG 
ADc - BNG
CHNDC - CHN

To check replication status :
repadmin /syncall
repadmin /replsummary
repadmin /showrepl
dcdiag /test:replications



1-Forest
1 -Domain
2 Sites
BNG and CHN
Three - dc1,ADC and CHNDC




NTFS permissions provide a powerful mechanism for controlling access to files and folders on Windows systems, ensuring security and data integrity in both local and networked environments.

Multiple Permission Types: NTFS permissions include various permission types, such as:
    • Read: Allows users to view the contents of files and folders.
    • Write: Allows users to create, modify, and delete files and folders.
    • Modify: Combines the permissions of Read and Write, plus allows users to delete subfolders and files, even if they do not have explicit permissions for those items.
    • Full Control: Grants all available permissions, including the ability to change permissions and take ownership of files and folders.
Inheritance: NTFS permissions can be inherited from parent folders, meaning that permissions set on a parent folder are automatically applied to its subfolders and files. This simplifies permission management by allowing administrators to set permissions at higher levels in the folder hierarchy.

Active Directory
Windows Active Directory is the overarching concept and technology for managing users, groups, and resources in a Windows network environment
ADDS
Active Directory Domain Services (AD DS) is a specific service or feature within Windows Server that implements the directory services functionality, handling tasks such as user authentication, authorization, and resource management within a domain-based network
Active Directory Domain Services is a critical part of the Windows Active Directory system, providing the core functionality for managing domains and their associated objects.





AD made of no.of  below partitions 



Trusts 



Role of DC within the forest 
Host the ADDS ( ntds.dit)  that lives on the file systems of all the DC's
DC are use to distribute Group Policy settings and preferences to the client computers 




AD is designed to be multi master what that means is you can make a change to any object  for ex. If I want to change a user properties . I can connect to any DC .i can make change 
No single point of failure 






You can manage AD by no.of tools   (AD Management Tools)




1.2 Deploying and managing ADDS Domain Controller 

Whenever you create DC additional DNS server records are created for the DC . These records determines which services running on the DC
GC, kerberos , ldap records 
DC in contoso.com domain has records stored in contoso.com  zone in DNS . So when a client computer wants to authenticate it query DNS speicifcally for the contoso.com zone and locate records that are relevant to that client computers for authentication and authorization .
If you configured sites in your org called Bangalore then computer based on its ipaddress can determine nearest DC 






Adding additional DC is for high availability of authentication and authorization services provided by DC

To create new forest install ADDS Role


After installation of ADDS Role
Promote the machine as DC


Child tree in an existing tree or as a new tree 

Deploy RODC 
The idea behind ROD if your physical DC were compromised or stolen then malicious person might get access to passwords possibly by removing hardisk
2 protections you can do 
Apply bitlocker
Replication policy




You can select record determine which host is offering the service  kerberos record and host contoso-dc-contoso.com offering the kerberos on port 88 
Priority and weight determines which dc is selected if there are several providing the same service and on what tcp port 


You can make your machine as global catalog
Member computers such as servers and workstations determine their site membership based on their ipaddress and setup configured by admin interms of subnet object and its relationship to a site 

Deploying DC to Azure 



FSMO Roles

When you are creating a new DC that you are aware of which DC hold which particular role 
For example 
Schema master is usually assigned along with the domain naming master to the first DC in the forest , you can transfer the role 




