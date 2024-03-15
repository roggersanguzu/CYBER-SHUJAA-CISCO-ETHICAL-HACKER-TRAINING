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
*-p: Show the process ID (PID) and name of the program to which each socket belongs.

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




