# TryHackMe--Nmap Quiz
![nmap](https://user-images.githubusercontent.com/52219676/87219391-391e4b80-c378-11ea-8675-be474497683e.png)

Network scanning is an important thing to knows about victim or target, such as what kinds of services runs on the background from the target?, what kinds of open ports on the target?.

Nmap is a famous open-source tool to grabbing and gathering information about network’s services. This room is very usefull for a beginner to know about Nmap, and how use Nmap to gathers network’s services from the target.

## Task 2 - Nmap Quiz
For Task 2, all of answers in Nmap’s description and we can see options summary on Nmap documentation https://nmap.org/book/man-briefoptions.html

# Question #1
First, how do you access the help menu?

ANS: -h

# Question #2
Often referred to as a stealth scan, what is the first switch listed for a ‘Syn Scan’?

ANS: -sS

# Question #3 
Not quite as useful but how about a ‘UDP Scan’?

ANS:-sU

# Question #4
What about operating system detection?

ANS: -O

# Question #5
How about service version detection?

ANS: -sV

# Question #6
Most people like to see some output to know that their scan is actually doing things, what is the verbosity flag?
ANS: -v

# Question #7
What about ‘very verbose’? (A personal favorite)
ANS: -vv

# Question #8
Sometimes saving output in a common document format can be really handy for reporting, how do we save output in xml format?

ANS: -oX

# Question #9
Aggressive scans can be nice when other scans just aren’t getting the output that you want and you really don’t care how ‘loud’ you are, what is the switch for enabling this?

HINT: This is listed under the misc section and enables pretty much everything

ANS: -A

# Question #10
How do I set the timing to the max level, sometimes called ‘Insane’?
HINT: The template names are paranoid (0), sneaky (1), polite (2), normal (3), aggressive (4), and insane (5)

ANS: -T5

# Question #11
What about if I want to scan a specific port?
ANS: -p

# Question #12
How about if I want to scan every port?
Omit beginning and end numbers to scan the whole range (excluding zero). read Port Scanning Options
 
ANS: -p-
 
# Question #13
What if I want to enable using a script from the nmap scripting engine? For this, just include the first part of the switch without the specification of what script to run.

ANS: --script

# Question #14
What if I want to run all scripts out of the vulnerability category?

HINT: The vulnerability category is referenced as ‘vuln’ in this case

ANS: --script vuln

# Question #15
What switch should I include if I don’t want to ping the host?

ANS: -Pn


## Task 3 - Nmap Scanning

# Question #1
Let’s go ahead and start with the basics and perform a syn scan on the box provided. What will this command be without the host IP address?

ANS: nmap -sS

# Question #2
After scanning this, how many ports do we find open under 1000?

ANS: 2

# Question #3
What communication protocol is given for these ports following the port number?

HINT: tcp or udp

ANS: tcp

# Question #4
Perform a service version detection scan, what is the version of the software running on port 22?

HINT: This will start with the number 6

ANS: 6.6.1p1

# Question #5
Perform an aggressive scan, what flag isn’t set under the results for port 80?

HINT: The answer here will start with an h

ANS: httponly

# Question #6
Perform a script scan of vulnerabilities associated with this box, what denial of service (DOS) attack is this box susceptible to? Answer with the name for the vulnerability that is given as the section title in the scan output. A vuln scan can take a while to complete. In case you get stuck, the answer for this question has been provided in the hint, however, it’s good to still run this scan and get used to using it as it can be invaluable.

HINT: This can be slightly misleading as this is referred to as a check in the output. In case you get stuck, here’s the solution: http-slowloris-check

ANS: http-slowloris-check




 
