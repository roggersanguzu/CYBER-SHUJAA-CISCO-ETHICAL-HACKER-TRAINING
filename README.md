# CYBER-SHUJAA-CISCO-ETHICAL-HACKER-TRAINING

The First Steps of Ethical Hacking include the following:
First and foremost is having a conversation with the Client and Clearly Knowing the scope of operation during the Process.
Then Signing a caontract and also clearly stating the Forms of Payment.
Clearly Stating the Means of communication.

# INFORMATION GATHERING.
There are various ways of information gathering. The main reason of information gathering is to know the version of 
systems that are being Used , to know the operating System of the Systems that are being used, to know the level or 
Extent of Vulnerabilities of the System.
The various ways of Information gathering are:
1. Using the OSINT Framework to gather information  (https://osintframework.com/) .
2. Using SpiderFoot. {spiderfoot -l 127.0.0.1:5001}// This is used to start the Spiderfoot and then it is opened in the Web.
3. Usinf the Recon-ng Information Gathering tool
        {
          It can be started using the Recon-ng Application or the "recon-ng" command.
          N:B ctrl + Shift +T is used to open a ne command Screen while "back" is used to go back to the terminal.
          Double tap the Tab to get more options and help or descriptions about the recon-ng.
   
         workspace save ........workspacename........
         workspace remove ........workspacename........
         workspace open/load ........workspacename........
         db schema //CHECKS on the schema of the recon-ng Database.
        }

# MARKET PLACE COMMANDS.
marketplace search // Checking available modules for usage in the recon-ng.
marketplace install .........needed module(Full domain)..........
marketplace info ......modulename......


# SOME OF THE BEST MODULES FOR DOMAIN/IP ADDRESS GATHERING.
hackertarget
Brute_host.


# Steps of Recon-ng Usage.
* install a given module.
* modules load ......modulename.....//Loads the required module.
* options unset SOURCE.
* options set SOURCE ........domainnameOVconcentration(Target).......
* input command// Checks whether the Source Domain has been Set.
* show hosts//Gives hosts.
* This then calls for the Installations of brute hosts  module to get  sub Domain.
* dnsrecon -d h4cker.org // this used to provide a detailed information about a Domain.
* Incase all the modules need to be installed, (marketplace install recon)
* Inorder to be be able to get infomation about a given recon-ng File(options list)
  

# RECON-NG RESULTS MANIPULATION.
* Donot forget the marketplace intall reporting/ ( This command is used to install the reporting module)
* options set CREATOR Roggers.// it is a must to have a creator
* options set CUSTOMER Coders.// It is a must to heave Customer.
* use the options list commmand to find the Locaton of the file because it is hidden in most Cases.
* Everytime Load the module first before using it.(Example options load reporting/html)
  
  
# DNS LOOKUP
* dnsrecon -d h4cker.org(This command is used to provide all the details about the Given Domain name.).
* dig h4cker.org ( The dig command is used to get more information aabout a Domain name); But remember that the
  same work has been solved by spiderfoot, recon-ng tool.
* nslookup command.
* dig h4cker.org mx (Used to Get information about Email Servers).
*N.B Many of these tools are here https://github.com/The-Art-of-Hacking/h4cker/tree/master/osint

# Finding Domain Name Servers For a given Domain.
# //Option one.
* step 1: nslookup
* step 2: set type=ns
* step 3: cisco.com (The Domain name of Concentration)
* server n1.cisco.com // This will then give the Details of the Second Name server.
* set type=any // This will give all the necessary information the needed Domain.
# //Option Two
*step 1: nslookup
* step 2: set type=ns
* step 3: cisco.com (The Domain name of Concentration)
# Other Options.
* Occasionally it is desirable to use a different DNS server to perform lookups. This may be necessary if the local DNS server
  is unable to resolve an address or resolves the host name to an internal private address and you need to obtain the internet accessible address of the host.
* nslookup skillsforall 8.8.8.8 ( nslookup ....prefered Domain name.... and then Google ip address).
* // Whois cisco.com (This command is mainly used to obtain information about the Domain registration information).

# Use whois to determine IP address registration information.
![image](https://github.com/RoggersAnguzu/CYBER-SHUJAA-CISCO-ETHICAL-HACKER-TRAINING/assets/141458053/5762637b-de87-4f46-aca4-4d7492b1ab22)

# Digging More information about Domain.
* dig strichat.com ns
* dig -x 172.268.0.34 // This is the Exact opposite of DNS, it aims at getting the associanted DNS other than the ip address
# Employee Intelligence Gathering.
* This involves the Social media and many more others.
# Site Certificates.
* Informations about an organization can also be got via the Site Certificates.(Normally Looks like the PadLock ON the Browser).
* The command netstat -tunap is used to display information about network connections, routing tables, and network interfaces on a Unix-like operating system. Here's what each option means:

*-t: Show TCP connections. // For Example netstat -tunap
*-u: Show UDP connections.//For Example netstat -uunap
*-n: Show numerical addresses instead of resolving hostnames.
*-a: Show all connections and listening ports.
*-p: Show the process ID (PID) and name of the program to which each socket belongs..

# Vulnerability Scans.
* nmap -sV --script vulners --script-args mincvss=4 h4cker.org

# SearchSpoilt.
* After doing a thorough search, then the searchsploit ..........The Vulnerability Website........... // This givens all the Sources of understanding the Vulnerability.
* enum4linux .......IPaddress/Domain Name..........// This command is is used to provide information about the users, groups , privileges and password strength on the
* Target machine.

# PACKET CAPTURE.
sudo tcpdump -i eth0 -s 0 -w capture.pcap // This captures Files and then them in a file with .pcap extension.

# GVM.(GREEN BONE VULNERABILITY MANAGEMENT).
* sudo gvm-check-setup.
* * nmap -sV --script vulners --script-args mincvss=4 h4cker.org
* sudo gvm-start
* Web UI (Greenbone Security Assistant): https://127.0.0.1:9392
* sudo gvm-stop.

* Username: admin //By Default it has been built in the Cisco Environment.
* Password: kali // By Default in the CISCO Environment.
* Simple Challenge. 10.6.6.23 or gravemind.vm.

  # Scocial Engineering.
  * setoolkit // Mainly For Fishing.
  * Zphisher // Clones Various Account to Collect Login Credentials.

* # Sofar
* I can Clone Various Social Media Accounts as a way to Show my Knowledge is Social Engineering.                                                                                                                                                                                                                                           
* [01] Facebook      [11] Twitch       [21] DeviantArt                                                                                                                                                                                       
* [02] Instagram     [12] Pinterest    [22] Badoo                                                                                                                                                                                            
* [03] Google        [13] Snapchat     [23] Origin                                                                                                                                                                                           
* [04] Microsoft     [14] Linkedin     [24] DropBox                                                                                                                                                                                          
* [05] Netflix       [15] Ebay         [25] Yahoo                                                                                                                                                                                            
* [06] Paypal        [16] Quora        [26] Wordpress                                                                                                                                                                                        
* [07] Steam         [17] Protonmail   [27] Yandex                                                                                                                                                                                           
* [08] Twitter       [18] Spotify      [28] StackoverFlow                                                                                                                                                                                    
* [09] Playstation   [19] Reddit       [29] Vk                                                                                                                                                                                               
* [10] Tiktok        [20] Adobe        [30] XBOX                                                                                                                                                                                             
* [31] Mediafire     [32] Gitlab       [33] Github                                                                                                                                                                                           
* [34] Discord       [35] Roblox

# XSS This is the attack that is normally known as Cross Site Scripting.
* It is mainly Done Using the BEef Software.
* The Software can be got from any of the Links Below.
* https://github.com/beefproject/beef and  https://beefproject.com/
* The Software is Launched by the Command:
*sudo beef-xss.
* username: beef.
* passwd: ------ the one for Logging into the VM.             
# To  Fasten Social Media Looking for Some.
* We can Use Sherlock
 * python3 sherlock user1  // To look for a single user.
 * python3 sherlock user1, user2 // To Look for Many People.


 * # clone the repo
$ git clone https://github.com/sherlock-project/sherlock.git

# change the working directory to sherlock
$ cd sherlock

# install the requirements
$ python3 -m pip install -r requirements.txt

# SMS ATTACK.
* A link can actiually be embedded in the Messsage Text to Gather a Target's Information.

# NETWORK ATTACKS AND VULNERABILIITIES.
The include the Following.
* Windows name resolution-based attacks and exploits
* DNS cache poisoning attacks
* Attacks and exploits against Server Message Block (SMB) implementations
* Simple Network Management Protocol (SNMP) vulnerabilities and exploits
* Simple Mail Transfer Protocol (SMTP) vulnerabilities and exploits
* File Transfer Protocol (FTP) vulnerabilities and exploits
* Pass-the-hash attacks
* On-path attacks (previously known as man-in-the-middle [MITM] attacks)
* SSL stripping attacks
* Denial-of-service (DoS) and distributed denial-of-service (DDoS) attacks
* Network access control (NAC) bypass
* Virtual local area network (VLAN) hopping attacks
* Network Basic In and Out put knowledge is needed /(NetBIOs). // This is mainly needed to acquire information about the

  # NETBIOS.
  * Taking over the NetBios involves having knowledeg about what is really Does.
  * TCP port 135: Remote Proceedure Call.
  * UDP port 137: NetBIOS Name Service.
  * UDP port 138: NetBIOS Datagram Service.
  * TCP port 139: NetBIOS Session Service
  * TCP port 445: SMB protocol, used for sharing files between different operating systems, including Windows and Unix-based systems.
  * Main Idea is to take control over the NetBios.
  * LLMR For mainly for Logical. N.B: It is important to Turn off the NetBios Ports in the Network Services.
  * Spoofing refers the Process of imitating the machines on a network.
  * The command that works here is:
  * searchsploit smb. //
  * Use the nmap -sN command to find the services available on hosts in the 172.17.0.0 virtual network.
  * ┌──(root㉿kali)-[/home/kali]
*└─# nmap -sN 172.17.0.0/24

*Performing an Enumeration on the Target.
* -U find configured users

* -S get a list of file shares

* -G get a list of the groups and their members

* -P list the password policies

* -i get a list of printers

* enum4linux scan on target 172.17.0.2.

* Enum4linux takes the advantages of smb weaknesses making it advantageous for the PenTestese.

//*  List the file shares available on 172.17.0.2 using the enum4linux -S command. Use the verbose option to see the Samba tools that are used to obtain the information.
*┌──(root㉿kali)-[/home/kali]
*└─# enum4linux -Sv 172.17.0.2

* enum4linux -a 172.17.0.2 // This is used to find out all the Potential Information about a Given Server.

* It is not a good Idea to use the Same machine to do various Task for Example ftp service and the Backend Usage Purposes.

* ![image](https://github.com/RoggersAnguzu/CYBER-SHUJAA-CISCO-ETHICAL-HACKER-TRAINING/assets/141458053/10b79ba6-6920-42d5-ab56-af606378ad5a)
* ![image](https://github.com/RoggersAnguzu/CYBER-SHUJAA-CISCO-ETHICAL-HACKER-TRAINING/assets/141458053/3092ef16-2be8-42d0-ab48-9a0ee837c861)
* ![image](https://github.com/RoggersAnguzu/CYBER-SHUJAA-CISCO-ETHICAL-HACKER-TRAINING/assets/141458053/465e5882-f85f-431a-9cf5-08b78bd97428)

* enum4linux -Sv 172.17.0.2    // This is used to check the Files that are really Sharable.
* smbclient -L 172.17.0.2 to Check on the Status of the Anonymous Login.
* smbclient //172.17.0.2/tmp

  
# WEB VULNERABILITIES AND EXPLOITATION.
* The method: In this example, the method is an HTTP GET, although it could be any of the following:
* GET: Retrieves information from the server
* HEAD: Basically the same as GET but returns only HTTP headers and no document body
* POST: Sends data to the server (typically using HTML forms, API requests, and so on)
* TRACE: Does a message loopback test along the path to the target resource
* PUT: Uploads a representation of the specified URI
* DELETE: Deletes the specified resource
* OPTIONS: Returns the HTTP methods that the server supports
* CONNECT: Converts the request connection to a transparent TCP/IP tunnel.
* The URI and the path-to-resource field: This represents the path portion of the requested URL.
* The request version-number field: This specifies the version of HTTP used by the client.
* The user agent: In this example, Chrome was used to access the website. In the packet capture you see the following:
* User-Agent: 





