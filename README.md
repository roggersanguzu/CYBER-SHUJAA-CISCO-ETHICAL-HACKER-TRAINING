# CYBER-SHUJAA-CISCO-ETHICAL-HACKER-TRAINING
{
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
install a given module.
modules load ......modulename.....//Loads the required module.
options unset SOURCE.
options set SOURCE ........domainnameOVconcentration(Target).......
input command// Checks whether the Source Domain has been Set.
show hosts//Gives hosts.
This then calls for the Installations of brute hosts  module to get  sub Domains.

dnsrecon -d h4cker.org // this used to provide a detailed information about a Domain.
}
