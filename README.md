Hello. Use this to learn and practise for your CompTIA Security + exam.

![alt text](https://github.com/Cham0i/SecPlus/blob/main/SecPics/goal.jpg)

# CompTIA Security+ Objectives

1) [THREATS, ATTACKS AND VULNERABILITIES](https://github.com/Cham0i/SecPlus/blob/main/README.md#1-threats-attacks-and-vulnerabilities)
   - 1.1 Types of Social Engineering Techniques
   - 1.2 Types of Attacks
   - 1.3 Application Attacks
   - 1.4 Network Attacks
   - 1.5 [Threat Actors, Vectors and Intelligence Sources](https://github.com/Cham0i/SecPlus/blob/main/README.md#15-threat-vectors-actors-and-intelligence-sources)
   - 1.6 Vulnerabilities
   - 1.7 Techniques used in Security Assesments
   - 1.8 Techniques used in Penetration Testing
2) [ARCHITECTURE AND DESIGN](https://github.com/Cham0i/SecPlus/blob/main/README.md#2-architecture-and-design)
   - 2.1 Security Concepts in an Enterpise Enviroment
   - 2.2 Virtualization and Cloud Computing Concepts
   - 2.3 Secure Application Development, Deployment, and Automation Concepts
   - 2.4 Authentication and Authorization Design Concepts
   - 2.5 Cybersecurity Resilience
   - 2.6 Security Implications of Embedded and Specialized Systems
   - 2.7 Physical Security Controls
   - 2.8 Cryptographic Concepts
3) [IMPLEMENTATION](https://github.com/Cham0i/SecPlus/blob/main/README.md#3-implementation)
   - 3.1 Secure Protocols
   - 3.2 Host or Application Security Solutions
   - 3.3 Secure Network Designs
   - 3.4 Wireless Security Settings
   - 3.5 Secure Mobile Solutions
   - 3.6 Cybersecurity Solutions to the Cloud
   - 3.7 Identity and Account Management Controls
   - 3.8 Authentication and Authorization Solutions
   - 3.9 Public Key Infastructure
4) [OPERATIONS AND INCIDENT RESPONSE]()
   - Will be added soon
   - I promise
5) [GOVERNANCE, RISK AND COMPLIENCE]()
   - Same with
   - this one...


# 1 THREATS, ATTACKS AND VULNERABILITIES

## 1.1 Social Engineering

**Ways to get manipulated**

- Phishing: Fake/ scam emails
  - Spear phishing: Tailored to catch a specific person. "Hello Robert from Echo Co. 148!"
  - Whaling: Spear phishing a high-ranking authorized user "Dear Joe Biden...send nuke codes"
- Smishing: Fake/ scam texts. Named derived from SMS
- Vishing: Fake/ scam calls. "Here to reach you about you car's extended warranty"
- Spam: Annoying, unsolicited email
- SPIM: Annoying, unsolicited text

**Tactics**

- Shoulder surfing: Watching or peaking a person's monitor/ screen for sensitive information
- Dumpster diving: Literally going through their trash for information
- Pharming: Using DNS to route a domain to a phishing site
- Tailgating: Following someone with authority to locations that are unauthorized for you. Like holding a door open after someone else scans their badge to enter.
- Eliciting Information: Use of small talk to obtain sensitive information "Yeah, the commander and I are going to be attending the graduation ceremony for the upcoming class" (Perfect time for a hacker to walk into their office and scrape some data off his computer. Thanks for the info sucka!!!!)
- Prepending: Modifying a file to look like another file. For example, FamilyPhoto.jpg vs FamilyPhoto.exe (PSA. Don't run .exe files you don't know)
- Identity fraud: Its not a joke Jim
- Invoice scams: Invoices or bills from scammers pretending to be a good/ service that the victim trusts.
- Credential Harvesting: Stealing credentials. (PSA. Don't lose your CAC. Don't leave a sticky note with your passwords next to your computer)
- Reconnaissance: Gaining information of victim or target. Maybe through OSINT (covered later)? Maybe using one of the above methods.
- Hoax: Non-threatning attack that appears threatning
- Impersonation: Pretending to be someone else (See "Catch me if you can" the 2002 movie)
- Watering Hole Attack: Legitimate website that target victim visits often which is infected with malware by hacker
- Typosquatting/ URL Hijacking: Making a URL similar to a legitimate website to trick a victim into a fake website. For example, Amazon.com vs Amaz0n.com
- Pre-texting: Formulating a fake scenario to trick a target into thinking a request is legitimate, or gain sympathy to bend rules. [Watch this hacker pretend to be the target's wife](https://youtu.be/lc7scxvKQOo?si=9eP6g3n60LvsQP1m&t=47)

Influence Campaigns use hybrid warefare, which is the use of politics, culture, social media, cyberspace, etc. in war

**Principles of effective social engineering**

- Authority: Appears to be coming from superordinate or legitimate business, coworker, etc with authorization.
- Intimidation: Invokes a fear of punishment or responsibility of a major loss
- Consensus/ social proof: Comforts to a popular verdict ("Everyone else is doing it, why aren't you?")
- Scarcity: Invokes a fear of missing out on a rewarding opportunity
- Urgency: Pressures the victim into taking action due to a closing time frame
- Familiarity/ Liking: Friendship or bond building using a victims sense of humor, hobbies, tastes, etc.
- Trust: Comforts the victim into thinking he/she is safe

## 1.2 Malware Types

- Ransomware: The encrpytion of a victims files which the hacker promises to decrypt once the ransom is payed. Well atleast according to the hackers...(PSA. Never give them money. Always have backups for this reason)
- Trojans: Software that a victim wants and installs with hidden malware
  - RAT (Remote Access Trojan): A trojan which includes some sort of spyware or remote access to the victim's computer
- Virus: Malware that requires user action to spread
  - Fileless Virus: Virus that is embedded within memory/ RAM
- Worm: Malware that spreads on its own. No user action needed.
- PUP (Potentially Unwanted Program)/ Bloatware: Unwanted apps that come with a product that you can't get rid of. Microsoft Edge, Apple Music, etc.
- C2 (Command and Control): Not necessarly a malware, more like a term used to describe a hacker's ability to do something post exploitation
- Bots: Computer's under a hacker's control
- Cryptomalware: Malware that secretely mines crypto currency for the hacker on the victims computer without knowledge
- Logic Bomb: Malware that only activates after a certain condition is met. Usually time related. For example, I recon March 22nd will be an intresting day at the computer lab...
- Spyware: Malware that is used to gather information from the victim. For example, Keyloggers
- Rootkit: Malware that infects BIOS or Root Kernal. It is undetectable within the infected OS, thus the hardrive must be scanned and fixed using specialized tools. (Basically you're done. Destroy the computer. Get a new one. You ain't reimaging this one chief)
- Backdoor: Unprotected access to administrative control. Sometimes these are purposefully placed by the developers of an app to quickly make changes or to comply with the feds' coercion for accessing data. Other times, they are created by hackers post hack to make sure they have access to a computer even if the victim's volnerability is patched.

**Password Attacks**

- Spraying: Trying one password for multiple accounts. It helps a hacker avoid being locked out of any one account. For example, guessing "Password123" for Jenny's, Robert's, and Jose's account. One of them has to be stupid...
- Dictionary attack: Using commonly used words or phrases to guess passwords. [Here is a list of the most commonly used passwords](https://en.wikipedia.org/wiki/List_of_the_most_common_passwords)
- Brute Force: Trying a myriad of keys until a password is randomly guessed. This attack is easily countered by enabling a max number of password attempts within a given time frame. (This is only feasable for keys of up to 128 bits. Any password longer than 256 bits would take 14 billion years for any computer to guess)
- Rainbow Table: Using a table of hashes derived from passwords to compare against a ciphered password. [Please look at this real life hacking example](https://youtu.be/icBD5PiyoyI?si=d1saS-j5J7_UvYiM&t=1758)

Its important to note the difference between offline and online attacks. Offline compares the results against a ciphertext or hash, so that the hacker isn't actually attempting to login. Online is the opposite; the hacker is not comparing its guess to any key. Online attacks are application dependant. (Will explain better in some other time)

**Physical Attacks** (Not like assualt and battery fyi)

- Malicious USB: Acts as an input device to infect a machine
- Card cloning: Copies the magnetic strips from cards. [Here is a whole video about it](https://youtu.be/ZDstCHYlj0U?si=ZbKyvRH1D-nDu7WH)
- Skimmers: Fake card readers placed on top of real ones to collect your credit card information. [PSA. Wiggle the card reader before each use or you'll end up like her](https://youtu.be/nBF5wTqyW-k?si=-2V7rWqycnTkub4t))

**Adversarial Artificial Intelligence**

- Tainted Training Data: Data that isn't categorized properly, weighted incorrectly, or otherwise trains the AI away from its intended purpose. [Machine learning algorithims are built on well sorted data](https://youtu.be/PeMlggyqz0Y?si=zgDLG95Q0zn8OiNW)
- Security of Machine Learning Algorithims: Keep the categorization, the weighting, and other ways your AI interprets training data hidden to avoid someone purposefully feeding the AI with powerfull tainted training data.

Supply Chain Attack: Malware is placed during the manufacturing or shipping of a product or one of its components. [This is how the Stuxnet worm was smuggled into Iran's nuclear facility](https://youtu.be/djUHvCyPYhY?si=gDbZ9jFaNuArEFjM&t=170)
  
Physical vulnerabilities "don't exist" in a cloud based network (atleast for Sec+ purposes. [In theory, someone could Watch_Dogs_2 their way into a Google server farm](https://youtu.be/meERzyzBTIo?si=kyIu2KoHm4uUNm15))

**Cryptographic Attacks**

- Birthday: Hash collisions. Same hash, different password. Named after the birthday paradox; which states that in a room of 23 people there is a 50% chance that 2 people share a birthday; and 99.9% chance that 2 people share a birthday after 75 people or more are present. The principle applies here by replacing people with passwords and birthdays with hashes. The statistical probability that two passwords produce the same hash is extremely more rare than the original birthday paradox, but since the possibility exists, this attack method exists also. [Here is a link to the website of the researchers who proved this was possible with SHA-1 encryption.](https://shattered.io/) (Which is why we don't use it anymore)
- Downgrade/ Bidding down/ Version rollback Attack: Forcing a downgrade on a encryption method to then hack that weaker version. [Video here](https://youtu.be/fBeShEMXcfU?si=IX4-iRu9jnTPnaed)

## 1.3 Hacking Applications

Priviledge Escalation: A unauthorized user gaining more priviledges. For example, the [DirtyCOW exploit](https://nvd.nist.gov/vuln/detail/CVE-2016-5195); in which a linux user could write priviledges faster than the computer could verify that the user had the authority to write to that file. Which is also an example of a race condition (see below).

**Injections**

Injections take advantage of the following computer languages in order to do something malicious via the misuse of user input. 

- SQL (Structured Query Language): SQL is a relational database structure; think of it as Excel spreadsheets. Injecting malicious SQL queries will allow a hacker to delete, change, or add data to that database strucute.
- DLL (Dynamic Link Library): DLL is shared based code that is used in memory. A malware can rewrite DLLs so that programs that rely on that DLL are maliciously altered. Have you ever wanted to create your own gaming cheat engine? This is how
- LDAP (Lightweight Directory Access Protocol): Its like a phonebook for internet users. 
- XML (Extensible Markup Language): Used for the transmission of data between two points; this data can intercepted and altered with injections.
- XSS (Cross Site Scripting): The implementation of malicious JavaScript code. JS is the underlying code that runs allows HTML websites to do logical tasks.

[Click here for an example of this in practice](https://youtu.be/KnQIbyK779I?si=BcPJQpxn29i2ShBn&t=227) 

- Pointer/ Object Deference: A pointer (AKA the piece of code that tells an OS where to find the rest of the information on a hardrive) can point to the wrong location and cause a crash. [Perphaps this CS50 video can dumb it down](https://youtu.be/qPI9a2N9s74?si=RpIjMQC0pLkAR8z1)
- Directory Traversal: Inspecting directories (AKA the folders on your PC) to plan out a potential attack or espionage
- Error Handling: The way in which an application handles an error. For example, if the user types a letter where numbers are expected its better for an app to say something like "Error: Passcode may only contain numbers" instead of simply crashing.
- Impropert Input Handling: The flawed acceptance of incorrect values or formatting. This is what allows injections to happen.
- Buffer Overflow: When a buffer (or section of memory reserved for a specific purpose) receives too much data that it overflows to other pars of the RAM; and thus corrupting the data in the neighboring buffer.
- Race Conditions: When two different processes run simultenously, but must finish in a specific orders. If the secondary processes finishes their tasks before the expected first process, a problem can occur. A common example of this is Time of Check and Time of Use race conditions. Imagine two people that want to buy the same anime figure on ebay. Suppose that when someone purchases the figure, it will change its status to "Sold"; and it only checks for the availability of the product when its added to checkout cart. If Bob and Albert both have the same figure in their cart, but Bob buys the figure first; Albert might also incorrectly purchase that same figure that in reality is sold out. So what's the race condition here? The check of availibility from Albert races the Purchase (or Use) from Bob. This is why its best practice to have your checks and uses of resources as close as possible. In real life, ebay would have checked the availibility of the anime figure right before purchase instead of when it was placed on the cart, thus minimizing the possibility of a race condition.

![alt text](https://github.com/Cham0i/SecPlus/blob/main/SecPics/racecon.webp)

- Replay Attack: Resending legitimate info for a fradulent response. For example, [I clone your car keys using the same signal that your legitimate car keys send to unlock your car.](https://www.youtube.com/watch?v=uxzm_6SYBFo) (PSA. Don't try this at home and also consider buying a Faraday cage.) (but if you do want to hack a car, remember that rolling codes exist and thus need to capture the signal out of reach)
  - Session Replay: A type of replay attack where a victim's session ID is resent to the server from the hacker in order to obtian access to the victim's session
- Integer Overflow: If a number gets too big and does not have access to more bits to represent that number, the value resets back to 0 once the max value is reached.

**Request Forgery**
- CSRF (Cross site): Using session cookies on a victim's computer to send legitimate requests to a server. (See [this](https://github.com/Cham0i/Cybersec-101?tab=readme-ov-file#html-cookies-and-cross-site-request-forgery-csrf-attacks))
- SSRF (Server Side): Using HTTP request to query a website's server

- API (Application Programming Interface): API essentially translates code amongst code. A hacker can misuse API to control an app
- Resource Exhaustion: The overuse of RAM or other component to disrupt a service
- Memory leak: Unused memory which is not released and thus denied to other apps that may need it
- SSL Stripping: Taking a victim to the HTTP (as opposed to HTTPS) version of a website. (See [this](https://github.com/Cham0i/Cybersec-101?tab=readme-ov-file#http-vs-https))
- Driver Manipulation: Using drivers to hack
  - Shimming: Adding extra inputs to drivers to cause misuse
  - Refactoring: Adding extra malicious output to drivers
- Pass the Hash: Old vulnerability where a hash can be used for authentication instead of the password (before its converted to hash)

## 1.4 Hacking Networks

**Wireless**

- Evil Twin: A fradulent copycat of a legitimate Wireless Access Point (WAP) which uses its identical SSID to trick clients into connecting to it.
- Rouge Access Point: A WAP that was not authorized to be installed on the network. Most likely done by someone who is not a part of the IT department wanting wifi in their area and thus unintentionally compromising security... what a jerk...
- BlueSnarfing: Hacker connects to unsecured bluetooth connection for contact, notification, data. etc.
- BlueJacking: Connecting without pairing/ authentication. This is an old vulnerability, most modern bluetooth devices require pairing.
- Radio Frequency Identification (RFID): The tech used in NFC
- Near Field Communications (NFC): Tap to pay. Security Badges.
- Initialization Vector (IV): Piece of keystream used per session (frame). (Will be explained better some other day)
- On-Path/ Man-in-the-middle Attack: Routing data through a hacker's device so that the data is viewed. [A common example is using a Evil Twin to redirect traffic with the hacker also being able to view the data going thru it](https://youtu.be/1OVTmrXGHyU?si=SWWwf0NBZgAOhUNh)

**Layer 2 Attacks (Data Link)**

- Address Resolution Protocol (ARP): You should know this by now (See [this](https://github.com/Cham0i/Netacad?tab=readme-ov-file#encapsulation-address-resolution-protocol-arp-mac-address-table-and-routing-tables))
  - ARP Poisining: Spoofing (AKA pretending to be legitimate) a fake MAC so that the ARP cache is inaccurate
  - MAC Flooding: Registering an overwhelming amount of new MACs to the MAC table to force the switch to act as a hub
  - MAC Cloning: Using someone else's MAC

**DNS**

- Domain Hijacking: Taking control over a domain
- URL Redirection: Redirecting from a URL to another site/ IP
- DNS Poisining: Adding spoofed DNS cache to be spread by other DNS servers
- Domain Reputation: Maliciously blacklisting domains can hurt their potential views on the web.

**DDos**

- Distributed Denial of Service: Multiple bots send multiple requests to strain an app, server, network, operational tech, etc. This is different from a normal Denial of Service attack, because with DDos the attacks come from various sources. Therefore a server isn't able to simply block a single IP from making an excessive amount of requests but must rather contend with multiple IPs collectively sending a myriad of requests (of which a server will most likely be unable to decern if they are legitimate).

**Malicious code or script execution**

Powershell, Python, Bash, Macros, VBA, can all change file permissions, NTFS permisions, change IP addresses, names, manipulate files etc. Execution policies, constrained language mode and even the complete deletion of these tools can provide better security.

## 1.5 Threat vectors, Actors, and intelligence sources

**Actors and Threats**

- Advanced Persistent Threats (APT): Hackers that will always attempt to hack you. "The opps that are always around the block"
- Insider Threats: Threats within your organization. Either traitors or incompetent people (like Dave, the guy that set up that Rouge Access Point without your permission... what a jerk...)
- State Actors: Government sponsored hackers (China, Russia, North Korea, and yours truly)
- Hacktivists: Hackers motivated by politics [Wake the fuck up, Samurai...](https://youtu.be/bN1tW2o23Qk?si=Ld851BTIqXFhjiji)
- Script Kiddies: Noob hackers that use other people's scripts to hack. They probably don't have a deep understand of what is going on underneath the hood with the code they utilize. 
- Criminal syndicates: Hackers for illegal profits. Fun fact: hackers target your medical records more often than your actual financial accounts.
- Shadow IT: Unauthorized modifiers of application or policies. (Akin to how the lizard people control the U.S government)
- Competitors: Business rivals (Arasaka vs Militech in Cyberpunk)

**Attributes of actors**

1. Internal or External (Is it Dave, from sales department, or is it a hacker from Russia?)
2. Sophistication level/ Capabilities (Is he a script kiddie or or a Watch_Dogs protagonist?)
3. Resources and funding (Does he have a single laptop to attack you or a gigantic botnet?)
4. Intent and motivation
![alt text](https://github.com/Cham0i/SecPlus/blob/main/SecPics/why.jpg)

**Vectors (Pathways for entry)**

- Direct Access: Coming through the router
- Wireless: WAP, Bluetooth, cell
- Email
- Supply Chain Attack
- Social Media (Social Engineering)
- Removable Media (Bad USB)
- Cloud

**Threat Intelligence Sources**

- Open Source Intelligence (OSINT): Free, public, information. [Here is a list of various OSINT tools you can try out](https://osintframework.com/) You probably won't know how to use any of them...patience young padawan (look up youtube tutorials)
- Closed/ Proprietary: Paid, closed off from the general public
- Vulnerability databases: Databases of known vulnerabilities 

Information Sharing and Analysis Center (ISAC): Established after 9/11. ISAC ensures that public and private forums communicate with each other using Automated Indicator Sharing (AIS).

Darkweb: The .onion sites. Illegal activity sometimes, but mostly FBI honey pots pretending to be illegal websites.

- Indicators of Compromise (IoCs): Evidence to believe a hack occured
- Structured Threat Information Expression/ Trusted Automated Exchange of Intelligence Information (STIX/ TAXII): Made by the Department of Homeland Security to easily share cyber threat intelligence (CTI). Think of them as the NFPA 704 hazard symbols of the cybesecurity field. [Here is a list of STIX objects](https://oasis-open.github.io/cti-documentation/stix/intro). TAXII is often also mentioned when STIX is brought up because TAXII is the protocol in which people commonly communicate STIX objects. However, STIX objects are what is most important here and don't necessarly have to be transmitted using TAXII.

![alt text](https://github.com/Cham0i/SecPlus/blob/main/SecPics/stix.webp)

- Predictive Analysis: Anticipation of incident, often using AI to guess hardware failures or network overload.
- Threat Maps: Geographic representations of past attacks. Its what you see prompt up in the "command room" in a lot of movies. [Here is a website that displays a live threat map](https://threatmap.checkpoint.com/) 
- File/ Code repositories: Storage area for data/ code (Hello, you are currently viewing this repository for Sec+ right now. Typically code is shared in these files, but im using as my own website)

**Research Sources**

- Vendor Websites: Website of product's vendor (Dell, [Apple](https://support.apple.com/en-us/HT201222), [Cisco](https://sec.cloudapps.cisco.com/security/center/resources/vex-cvr-faqs), etc.)
- Vulnerability Feeds: Newsletters, RSS Feeds, Content creators, etc. EXAMPLES: https://cyberprotection-magazine.com/ https://www.esecurityplanet.com/ https://jetpatch.com/blog/ 
- Conferences: [DEFCON](https://www.youtube.com/@DEFCONConference/videos), [Blackhat](https://www.blackhat.com/us-24/), etc.
- Academic Journals: Often theoretical without practibility. College papers.
- Request For Comment (RFC): Documents maintained by the IETF. They are the "laws" of the internet, essentially creating the standard for computer communication across all layers (of the OSI model). [You may find the entire RFC collection here](https://www.rfc-editor.org/search/rfc_search_detail.php?sortkey=Number&sorting=DESC&page=All&pubstatus%5B%5D=Standards%20Track&std_trk=Internet%20Standard)
- Local Industrial Groups: Based on industry (issa.org ????)
- Social Media: Reddit, twitter, youtube.etc
- Threat Feeds: Real time data streams recognizing threats

![alt text](https://github.com/Cham0i/SecPlus/blob/main/SecPics/threatmap.jpg)

- Advesary Tactics, Techniques, and Procedures (TTP): The actions of threat actors to gain access. Goal (Tactic) How (Technique) specific way/ variables (procedures)

## 1.6 Security Concerns with various types of vulnerabilities

And here I come to assert to you again, that in comparing a Cloud network vs on-premise network, Cloud networks do not have phyiscal vulnerabilities (for purposes of the Sec+ test).

Zero Day: Vulnerability that was previously unknown upon release. Comes from the fact that the vulnerability was present on day zero.

**Weak Configurations**

1) Open permissions
2) Errors
3) Unsecure Protocols
4) Unsecure Root Accounts
5) Weak Encryption
6) Default Settings
7) Open Ports and Services

**Third Part Risks**

- Vender Management: Vendor negotiating, contracts, termination. Essentially, make sure your organization has the money and diplomacy to rely on the vendor.
- System integration: Although merging organizations might increase productivity it also increases the attack surface for any potential hacker. 
- Lack of vendor support: Not communicating nor providing End of Life (EOL) and End of Service Life (EOSL) support to products might mean that once the vendor is done with a product/ service continuing to use the product/ service may expose your organization to threats which the vendor will not be able to help with.
- Outsourced code developement: Your organization doesn't known for sure what is inside a given piece of code if its produced elsewhere.
- Data Storage: The 3rd party vendor must be trustworthy enough to keep your organazations' data secure.
- Improper/ Weak path management: To ensure that the product/ service is compatible with your organization its important to centralize the patches and test them prior deploying them to the network.
- Legacy Platforms: EOSL that doesn't get security updates

Impacts the following:

1) Financial. In the form of delayed sales, overtime, fines, quantitive loss of money
2) Reputation. Data Breach = Your security sucks, which implies you suck and your products suck
3) Availibility loss. Unavailible data and angry customers.
4) Data Loss (gone/deleted) Data Breach (viewed by unauthorized people) or Data exfiltration (stolen data)

Identity theft: Impersonation with documents

## 1.7 Techniques used in security assesments

- Threat Hunting: Actively locating and mitigating cyber attacks
- Intelligence Fusion: The good guys share Computer Threat Intelligence (CTI)
- Threat feeds: RSS Feeds, podcasts, blogs, etc. [See Research Sources](https://github.com/Cham0i/SecPlus/blob/main/README.md#15-threat-vectors-actors-and-intelligence-sources)
- Advisories and Bulletins: Announcement by organizations. See Research Sources (link above)
- Manuever between these different techniques

**Vulnerability Scans**

This is called a $Confusion Matrix$

![alt text](https://github.com/Cham0i/SecPlus/blob/main/SecPics/confusion.png)

It lays out the options for a machine learning algorithim (or any form of decision making) to categorize its outputs. Using the example of COVID-19 testing, we could say that a TP is when a COVID carrier tests positive. A TN would be when a non-carrier tests negative for COVID. Both of these are True, and thus the desired outcomes. Yet, sometimes FP and FN may occur in AI algorithims. In our COVID example, this would be as if a non carrier test positive or when a carrier tests negative. Its important to make good criterias for training AI or making network administration policies so that hackers are deterred and legitimate employees remain undisturbed.  

- Log Reviews: Looking for signs of attack using logs
- Credentialed vs not: Valid authentication (admin priviledges)
- intrusive vs non-intrusive: Affects perfomance, may restart as opposed to background scan
- Common Vulnerabilities Exposure/ Common Vulnerabilities Scoring System (CVE/CVSS): Databases and scoring of vulnerabilities. [Video Explanation Here](https://youtu.be/SYio0CH6-Mo?si=RofMiMLz1h23-E78)

**Security Information and Event Manager (SIEM)**

A unified collection of data for real time analysis. [A much more detailed explanation of SIEM](https://youtu.be/zrgBrpv4azs?si=FA-Zi7W4DjI6RhPj)

- Review Reports: Results of success rate of SIEM/time period
- Packet Capture: Collecting packets of data
- Data Input: Data that goes into SIEM such as
  - Log Collectors: Tools for recording network events and SNMP inputs
  - User Behaiviour: How users behave (Login times)
  - Sentiment Analysis: What people are discussing (Bomb threats?)
  - Security Monitoring: Watch and record network activity
  - Log Aggregation: Oraganized labeling and collection of logs
- Security Orchestration, Automation and Response (SOAR): Toolset to react to threats. Think of it as a playbook (automated) runbook (conditional)

## 1.8 Pentesting techniques

- Known (white) Unknown (black) partial (gray box) enviroments
- Rules of Engagement: How, what, when pentesters can do within availible network
- Lateral Movement: Actions within avalible network to gain deeper access
- Persistence: Perpetual access (backdoor)
- Priviledge Escalation: Gaining deeper access
- Clean up: Deleting logs, folders, registries, etc to avoid detection that a pentester was present
- Bug Bounty: Payment for discovery and report of vulnerabilities
- Pivoting (PC to Router to Target PC, etc.)

**Passive and Active Recon**

War [anything] Searching for wireless networkds. Footprinting is collecting as much info on the target.

**Exercise and Types**

Red (ATTCK) Blue (DEF) White (Referees) Purple (ATTK and DEF/ Coach coms)

# 2 ARCHITECTURE AND DESIGN

## 2.1 Security Concepts in enterprise enviroments

**Configuration Management**

The following image depicts a network created by some random person online.

![alt text}(https://github.com/Cham0i/SecPlus/blob/main/SecPics/netdiawhite.png)

In a professional setting, the Standard Naming Convention should be short, but precise. For example, instead of naming a switch "dumb switch" you might opt to name it S1 (for Switch 1). For much larger organizations, you may have to add additional information like the floor that the device is on and which building its located in. Example: ES3-E4 could be your organizations' way of referring to the ExchangeServer #3 located in the East building on the 4th floor. Whatever naming convention your organization adopts, it has to be uniform accross all devices and should adhere to a short, but precise principle. Just like the names of devices, the devices' IPs should also be neat, organized and uniform. In the image above, we can see that IP cameras use IP addresses from 10.10.3.2 - 10.10.3.10. PCs and servers seem to take IPs 10.10.2.50 - 10.10.2.255. Again, whatever IP Schema your organization uses, ensure that its easy to understand so that identifying computers whilst troubleshooting is easiest. 

The image above was an example of a logical network topology. Meaning that it shows devices and its connections to other devices as they are located within the various networks and subnets. The image below is a physical network topology. Its purpose is to show where the devices are located in terms of geogpraphy. 

![alt text]()

Both are diagrams/ topologies, but serve different purposes. If you want to know where a device is, use physical; if you want to know what its connected to; use logical.

- Baseline Configuration: Baseline Performance
- Data Sovereignty: Under which government is data under the jurisdiction of?

**Data Protection**

- Data Loss Protection (DLP): An umbrella term for methods and products intended to keep data from being lost. USB Blocking, backup verification, data monitoring, etc
- Masking: Censoring of data. (xxx) xxx-1234. SSN: *** - ** - 1234
- Tokenization: An arbitrary number or string that is tied to sensitive information elsewhere. Student ID: 1602851, Patient #: 159ST3, Traffic Ticket Violation: WMG16-195MFGAP6LT 
- Digital Rights Management (DRM): Technologies aimed at stoping piracy of their products
- Geographical considerations: Consider under which legal jurisdiction your server will operate under, possible threats to that site, and lag caused by the distance of your servers to your customers. 
- Response and Recovery Controls: The thing Control Incident Responce people do
- SSL/ TLS Inspection: Grabing, decyphering and reencrypting packets
- Hashing: Integrity checks can be done using asymetric key encryption
- API considerations: Never fully trust code your organization didn't write. 

**Site Resiliency**

You know how doomsday prepares have bunkers in case their homes are destroyed? Well organizations have hot, warm, and cold sites in case of emergencies (like the California wildfires).

- Hot: Basically the main site. It might effectively be another branch or store that operates nearly identical to your original site.
- Warm: May have some utilities, older hardware, overall the site has an insufficient amount of resources for maximum productivity (as compared to your original site). Imagine having 1 port-a-potty for 40 people...
- Cold: No or few utilities, basically only servers, open space mostly.

**Deception and Disruption**

"Honey" + [anything] is a trap! They are meant to lure attackers into triggering an alarm or away from the real deal. "Honeyyyy, he's just a friend" -My EX, Summer of 2019

- Honeyfile: Fake files that bait attackers to click on or interact with. They usually send an alarm to the defense team
- HoneyPot: A term used to describe the collective honeynet and honeyfiles used to bait hackers. Usually in refrence to websites. "David, c'mon buddy... hire-a-hitman.com is obviously a FBI honeypot"
- Honeynet: An entire fake network designed to distract a hacker away from the real network
- Fake telemetry: If a wise attacker were to see a router that isn't routing anything, he might deduce that it is looking at a device within a honeynet. However, if you were to implement fake serverloads, RAM consumption, packet transfers, etc...the hacker might believe the network is legitimate. 
- DNS sinkholes: A DNS server that ignores requests for known malicious websites "Sorry Timmy, we can't let you access NoScamFreeRobux.com. They already gave Dave's PC internet STDS"

## 2.2 Virtualization and Cloud Computing concepts

**Cloud Models**

- Infastructure as a service: Azure, AWS
- Platform as a service: Web app server, database server, etc.
- Software as a service: Apps like Google Drive, docs, excel, etc
- Anything as a service (Xaas): Monitoring (Maas) Desktop (Daas)
- Public Cloud: Azure AWS, etc
- Hybrid: Combination of any of the above. DMZ reasons
- Managed Service Provider/ Security Provider (MSP/MSSP): Offshored IT/Sec and monitoring usually by CSP
- Fog Computing: Local processing. Pre-sync
- Edge Computing: Local processing and data sotrage (normal net)
- Containers/ App Cells: allow cloud usage of apps
- Microservices/ API: Distributed cloud cloud code; such as user logins, database, Xaas,; tiny cloud services
- Infastructure as Code: Use preset definition files as opposed to being manually set up
- Software Defined Network (SDN): Centralized routing and switching configurations
- Software Defined Visibility (SDV): Centralized viewing of network devices
- Serverless Architecture: CSP provides services directly to endpoint (AWS Lambda)
- Service Integration: Combining all cloud services into a single source (or just use one CSP).
- Resource Policies: Permissions given to a resource
- Transit Gateway: On-premise to cloud gateway (VPN)
- VM Sprwal avoidance: Limit permissions to create VMs, enact policies, monitor, keep good inventory, audit
- VM Escape Protection: Same as physical machine (harden, snapshots, sandbox, test, scan, etc.)

## 2.3 Secure App development, deployment and automation

**Enviroment (Dev)**

- Resource vs Security (more code = more bugs)
- Scalibilitiy (Meeting increased demand)
- Elasticity (Scale up or down as demand changes)
- SDK (JavaOKD, .NET) vs APIs

**Testing**

Code quality, debugging, use IDE (static code analysis) fuzzing (random inputs

[REDO THIS SECTION]

**Secure Coding Techniques**

- Normalization: Store and organize data so its not rpreated unnecessarly
- Stored procedures: Custom code for custome query format to avoid injections
- Obfuscation/ camoflage: Difficult to read code, but not encrypted ( to avoid lag) JS minifying
- Code Reuse/ Dead code: Use SDK and libraries to get rid of code that does nothing
- Data Exposure/ encryption: Use HTTPS, AES, or attempt obfuscation/ camoflage (see above)
- Open Web Application Security Project (OWASP.org)
- Software Diversity: Different executables for same process to confuse hackers

**Automation/ Scripting (Things done automatically)**

- Continous monitoring: Monitor functioning of application itself
- Continous Validation: Code running as expected
- Continous Integration: Different parts are working together properly
- Continous Delivery: Deploy latest version to customers
- Continous Deployment: Process that make continous delivery happen (AKA automatic updates)
- Version Control: Management of changes

## 2.4 Authentication and Authorization concepts

- Directory: A network with a Domain Controler and its respective Client Computers
- Federation: Essentially Active Directories' Forest. Its made up of multiple Directories. Can access other directory using your directories credentials
- Attestation: Hardware use for verfication

**Technologies**

- Time-Based One Time Password (TOTP): Changes password every couple of seconds. Requires synconization of keys and lock
- HOTP: HMAC uses hasj counter to generate a new key each time a key is used to unlock. U2F key
- Token Key: 3rd Party password generator that syncs key with lock phyiscal (U2F) software (QR, Authentication Apps)
- Static Code: PIN codes (dont' change)
- Smart Card Authentication: NFC card, magnetic strip
- Personal Identity Verification Card (PIV): Essentially a smart card with an ID (CAC)

**Biometrics**

- Fingerprint (cheap), Retina/Iris (Expensive), Facial (Uses infrared tech), vain matching (accurate), voice (inaccurate), gait analysis (AKA walking analysis. its 75% accurate)
- False Rejection Rate (Type 1 error), False Acceptance Rate (Type 2 error), and Crossover Error Rate (sweet spot).

[ADD GRAPH]

**Multifactor Authentication (MFA)**

- Factors: Known (password), Have (Physical key), Are (biometrics)
- Attributes: Somewhere you are (office, geofencing), something you can do (action, gestures, pattern), someone you know, something you exhibit (neurological, as in speech)

## 2.5 Implement Cybersecurity Resilience

- Geographical Dispersal: Synced copies around the world to avoid natural disasters or "peacefull protests"
- Redundant Array of Independant Disks

[EXPLAIN RAID 1, 0, 10, 5, 6 and Parity using XOR]

- Multipath: More than one way of accessing data
- Load Balancers: Provide efficient division of loads. Helps with peak demand resource exhaustion.
- NIC Teaming: Multiple NICs per machine to ensure connectivity if one fails
- Uninterruptable Power Supply (UPS): Emergency battery provides enough power to safely shut down
- Power Distribution Units (PDU): Power strips but smart
- Storage Area Network (SAN): Centralized storage that is detached from any one machine client. Cloud
- Master Image: OS Image that all other VMs copy/ patch from

**Backup Types**

- Full (whole) Incremental (Changes from last) Differential (All changes from previous full save??)
- Tape: Magnetic strip
- Disk: Magnetic disk
- Network Attached Storage (NAS): Centralized storage that is attached to LAN and shared locally

## 2.6 Security Implications of Embedded and Special System

- Raspberry Pi: SoC, DNS Pihole, VPN, etc
- Field Programmable Gate Array (FPGA): ICs reprogrammable for hardware corrections
- Arduino: For robotics
- Supervisory Control and Data Aquisition (SCADA/ICS): For utilities, HVAC, industrial control systems, etc
- Internet of Things (IoT): Smart devices, wearables with sensorts, multifunction devices. These devices' default settings typically aim for ease of use rather than security
- Facility Automation: Heating and cooling automation

**Specialized**

- Medical Systems: HIPPA and "wireless injuries"
- Vehicles: Bluetooth, wifi, cell vulnerabilites
- Aircraft and Drones: (UAV, autopilot, embedded cameras, wifi)
- Smart Meter: Monitoring of water, electricity,etc
- Surveilance System: SoC, cell, wifi, cloud storage privacy concerns
- Voice over IP (VOIP): Dos, spoofing, harrasment
- Mobile System: IoC vulnerabilities keep updated
- Real Time OS (RTOS): Responds to input in real time

**Communication Considerations**

- 5G: cell
- Narrowband (NBIoT) Only 200khz band. Max battery life
- Zigbee: low power radio providing personal network
- Baseband Radio: Near 0 frequency radio

## 2.7 Physical security controls

- Barricades
- Alarms
- Badges
- Cameras (motion, object detection)
- Access Control Vestibules (manholes and mantraps)
- CCTV + industrial camoflage (AKA hide them)
- Robot Sentries
- Human Guards
- Reception with sign in procedure
- Two-person integrity/ control
- Locks (bio, electric, physical, cable)
- USB data blocker
- Good lighting
- Fencing
- Faraday Cages
- Air Gap (physical seperation of secure and unsecure networks)
- Screened subnet/ DMZ
- Hot/ cold aisles (good airflow???)
- Burning, shredding, pulping (soak in water to recycle), pulzerizing (smash), degaussing (electromagnetic wiping), 3rd party (software DBAN, Hillary Clinton used BleachBit)

## 2.8 Basic Cryptographic Concepts

- Digital Signatures: AES from both client and host
- Key length/ size: # of bits
- Key stretching: Using key derivations functions that slow down deriviations (PBKDF2, bcrypt)
- Salting: Adding extra string to plain password. The salt value also has to be stored by system
- Hashing: Value that represents integrity
- Key Exchange: In symetric encryption a key can be exchange in-band (using same communications as message) or out of band (in person [USB] or independant channels)
- Elliptic: Curve cryptography??? (ECC) Asymetric, low resource cost, used in phones. Still fairly hard to crack.
- Perfect Foward secrecy: Use a key only once so that its hash isn't found elsewhere
- Quantum Cryptography: Using qubits (0, 1, and superposition) a quantum computer could crack any encryption up to date. While the theory is sound, its implementation has yet to be widespread. Fun fact: The FBI stores many encrypted messages from bad guys in hopes that they may be decrypted once quantum decryption arrives. New post-quantum crpytography will have to be developed for public use to withstand quantum decrpytion.
- Ephemeral: Temporary key used once (session key?)
- Modes of operation: DES uses 5 blocks
- Electronic Code Book (ECB): 64 bit plain directly to cyphertext. Identical ciphertext will have identical messages
- Cipher Block Chaining (CBC): Encryption has to be sequential. One chain error can corrupt the rest of the data.
- Counter Mode (CTR): using nounce/ counter. Uses XOR to decrpyt?
- Authentication Encryption (AE): Encrypts message and authenticates it
- Blockchain: Uses public ledger as a decentralized way to record transactions within the blockchain of computers using the crypto currency
- Cipher Suites: Group of algorithms used to secure connections
- Stream: Bit-by-bit encryption
- Block: Chunks of bits encryption
- Symmetric (one key) vs Asymetric (public and private key)
- Steganography: Hiding data in other data (audio, video, image)
- Homomorphic Encryption: Modifying encrpyted data which applies its changes once decrpyted

[USE DIAGRAMS HERE]

Common use cases 

- For low power consumption use ECC
- For low latency use Symmetric cryptography
- For high resilience use AES (until quantum makes its global debut)

The best cryptosystem makes data obfuscating (unclear) with integrity (no change), authentication (correct source) checking features and...
- Non repudiation: Inability to deny action (used private key to sign)
- Confidentiality: Only intended viewer can view

Limitations:

Longevity; as in how long a system is secure given current tech ($quantummmmm$) Entropy; the pseudorandomness of a number

# 3 IMPLEMENTATION

## 3.1 Implement Secure Protocols

- DNSSEC: Digitally signs every zone file for every domain in DNS to prevent cache poisining
- SSH: Replaced Telnet as a secure way to send commands to remote machines (Port 22)
- S/MINE: Encrypts email attachments (Port ??)
- SRTP: Voice and audio encryption (UDP 5004)
- SFTP (FTP + SSH): Encrypted file upload and download (Port 22)
- SFTPS (FTP + SSL/TLS): Same as above but using public-private key encryption of SSL/TLS (TCP 990)
- LDAPS: Allows already authenticated directory users to browse and locate objects (TCP 636)
- SNMPv3: Device monitoring (UDP 161 and 162)
- HTTPS (HTTP + SSL/TLS): (TCP 443)
- IPSec: Authentication and encryption for IP
  - Authentication Header (AH): Integrity and authentication
  - Encapsulating Security Protocol (ESP): Encryption
  - Tunnel/ Transport: Tunnel mode doesn't use AH but does encrypt using ESP (because some devices can't read AH).
- POP: Receives email and promptly deletes it off the server once it's downloaded from it
- IMAP: Receives email, but keeps a original copy of the email in the server. Also supports multiple connections (TCP 143)
- NTP: Network Time Protocol is the time sync protocol

## 3.2 Host or application security solutions

**Endpoint protection**

The Following are present in most NGFW:

- Antivirus
- Antimalware
- Host firewall
- Data Loss Prevention (DLP)
- Host Intrusion Detection System (HIDS)
- Host Intrusion Prevention System (HIPS)
- Detect and Response (EDR)

**Boot Integrity**

- UEFI: Secure Boot
  - Boot attestation: Report to remote trusted system
  - Measured Boot: Verify integrity of bootfiles over a network (win10) stops root kits
Databases can salt, tokenize, and hash data

**Application Security**

- Input Validation: Rejects possible injections
- Secure cookies: Cookies that deny sending info unless they are secured
- HTTP Headers: Provide browser with critical information
- Code Signing: Integrity signature on code
- Firewall
- Static Code Analysis (IDE)
- Fuzzing: Input testing
- Dynamic code analysis: IDE but done live
- Hardening: Close unused ports, disk encryption, OS patches, lock access to harmfull registries, password for admin/root access
- Self Encrypted Drive (SED) or...
- Full Disk Encryption (FDE)
- Hardware root of trust
- Sandboxing
- Trusted Platform Module (TPM)

## 3.3 Secure Network Designs

- Load Balencing: Efficient workload share. active/active; which splits the workload. active/passive; where one server takes the majority of the workload and the other takes the excess.
- Scheduling: Which devices gets the request
- Virtual IP: IP of load balancer. Like public IP???
- Persistance: Service always availble

**Network Segmentation**

VLAN segmentation to organize and avoid lateral movement
- DMZ/ screened subnet
- East west traffic: Server to server within LAN
- North South traffic: Internet leaves LAN
- Intranet: Local LAN
- Extranet: Local LAN with external access to LAN for customers, clients, students, etc.
- Internet: WorldWideWeb. Everyone
- Zero Trust: Exclude traffic untill its verified or health checked


VPN segmentation
- Always-on: VPN concentrators for remote of site-to-site access
- Split Tunnel (only LAN traffic) vs Full tunnel (from another company LAN)
- Remote (outside company LAN) vs Site-to-site (from another company LAN)??
- L2TP: Microsoft and Cisco product. Slowly being replaced by IPSec, SSL/TLS VPNs.

DNS Segmentation
- Network Access Control (NAC): Prohibits connection to join network untill health check or verification
- Agent-based: Battleye, anticheat, any other fine tunned monitoring
- Out-of-band Management: Admin access to downed server, offline access, AUX and Console

**Port Security**

- Broadcast Storm Prevention: DDos flood guard
- BPDU Guard: Protects from accidental routing loops
- DHCP snooping: Blocks any other DHCP server not in the whitelist

**Network Applianeces**

- Jump server: Used in DMZ
- Foward Proxy: Outward traffic. Used often to regulate content monitoring
- NIDS and HIPS: Detection (passive) and Active (inline) control. Respectively
- Detection Types:
  - Signature; Database of known patterns
  - Rule; Ruleset, policy threshold
  - Heuristic; Signature + Rule combination. Creates rules based on a signature for that specific server
- Hardware Security Module (HSM): Hardware specific to reduce cryptography processsing
- Sensor: Monitors packets in NIDS/ HIPS
- Collectors/ Aggregator: Takes in data

**Firewalls**

- Web Application Firewall (WAF): Dedicated hardware box
  - Statefull; group
  - stateless; packet per packet
- Unified Threat Management (UTM): Multiple security application and devices
- NAT Gateway: Gives private IP to devices under single public IP
- Content/ RL Filter: Content URL block
- Host; Software on workstation vs. Virtual; within VM
- Access Control List (ACL): Criteria/ rules for a firewall. Discriminates on IP, port, time, etc.
- Route Security: Routers must be trustworthy
- Quality of Service (QoS): Bandwidth maximum or minimum on certain protocols???
- IPv6: Consider a NGFW for IPv6 Firewalls
- Port mirroring/ spanning: Monitors data fo copying passive data (in n out)
- Network Tap/ Port tap: Steals some packets to test them
- Monitoring services: Baseline to real-time monitoring
- File Integrity Monitors (FIM): ?:???

## 3.4 Wireless Security Settings


- WPA2: AES, 8-63 characters, pre-shared key
- WPA3: same, but diffie-hellman
- Counter Mode Cipther Block Protocol (CCMP): 128 bit key and 128 block size. 48 bit IV? (initialization vector???)
- Simultaneous Auth
