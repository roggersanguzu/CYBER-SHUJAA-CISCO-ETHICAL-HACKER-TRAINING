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
* This then calls for the Installations of brute hosts  module to get  sub Domains.
  

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
#
