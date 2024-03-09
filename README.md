CompTIA Sec + is a memory test. The concepts are really easy, too easy some might say, but you need to know the correct termanology in order to pass this test.

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
- Pre-texting: Formulating a fake scenario to trick a target into thinking a request is legitimate, or gain sympathy to bend rules. [Example](https://youtu.be/lc7scxvKQOo?si=9eP6g3n60LvsQP1m&t=47)

Influence Campaigns use hybrid warefare, which is the use of politics, culture, social media, cyberspace, etc. in war

**Principles of effective social engineering**

- Authority: Appears to be coming from superordinate or legitimate business, coworker, etc with authorization.
- Intimidation: Invokes a fear of punishment or responsibility of a major loss
- Consensus/ social proof: Comforts to a popular verdict (sheeple. beheheheheh)
- Scarcity: Invokes a fear of missing out on a rewarding opportunity
- Urgency: Pressures the victim into taking action due to a closing time frame
- Familiarity/ Liking: Friendship or bond building using a victims sense of humor, hobbies, tastes, etc.
- Trust: Comforts the victim into thinking he/she is safe

## 1.2 Malware Types

- Ransomware: The encrpytion of a victims files which the hacker promises to decrypt once the ransom is payed. Well atleast according to the hackers...(PSA. Never give them money. Always have backups)
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
- Dictionary attack: Using commonly used words or phrases to guess passwords. [See example here](https://en.wikipedia.org/wiki/List_of_the_most_common_passwords)
- Brute Force: Trying a myriad of keys until a password is randomly guessed. This attack is easily countered by enabling a max number of password attempts within a given time frame. (This is only feasable for keys of up to 128 bits. Any password longer than 256 bits would take 14 billion years for any computer to guess)
- Rainbow Table: Using a table of hashes derived from passwords to compare against a ciphered password. [Please look at this example](https://youtu.be/icBD5PiyoyI?si=d1saS-j5J7_UvYiM&t=1758)

Its important to note the difference between offline and online attacks. Offline compares the results against a ciphertext or hash, so that the hacker isn't actually attempting to login. Online is the opposite; the hacker is not comparing its guess to any key. Online attacks are application dependant. (Will explain better in some other time)

**Physical Attacks** (Not like assualt and battery fyi)

- Malicious USB: Acts as an input device to infect a machine
- Card cloning: Copies the magnetic strips from cards. Fine here's a whole fucken video! [Example](https://youtu.be/ZDstCHYlj0U?si=ZbKyvRH1D-nDu7WH)
- Skimmers: Fake card readers placed on top of real ones to collect your credit card information. (PSA. Wiggle the card reader before each use)

**Adversarial Artificial Intelligence**

- Tainted Training Data: Data that isn't categorized properly and thus misguides the machine learning process. (Editor's Note; This is a hard concept to understand if you don't know how AI works. Might have to explain how machine learning works in future update)
- Security of ML Algorithims: Basically keep your code hidden

Supply Chain Attack: Malware is placed during the manufacturing or shipping of a product or one of its components. See [Stuxnet](https://youtu.be/djUHvCyPYhY?si=gDbZ9jFaNuArEFjM&t=167)
  
Physical vulnerabilities don't exist in a cloud based network (atleast for Sec+ purposes. In theory, someone could WatchDogs_2 their way into a Google server farm)

**Cryptographic Attacks**

- Birthday: Hash collisions. Same hash, different password
- Downgrade/ Bidding down/ Version rollback Attack: Forcing a downgrade on a encryption method to then hack that weaker version

## 1.3 Hacking Applications

Priviledge Escalation: Giving an unauthorized user more priviledges (User to Admin priviledges)

**Injections**

Injections take advantage of the following computer languages in order to do something malicious via the misuse of user input. 

- SQL (Structured Query Language): SQL is a relational database structure; think of it as Excel spreadsheets. Injecting malicious SQL queries will allow a hacker to delete, change, or add data to that database strucute.
- DLL (Dynamic Link Library): DLL is shared based code that is used in memory. A malware can rewrite DLLs so that programs that rely on that DLL are maliciously altered. Have you ever wanted to create your own gaming cheat engine? 
- LDAP (Lightweight Directory Access Protocol): Its like a phonebook for internet users. 
- XML (Extensible Markup Language): Used for the transmission of data between two points; this data can intercepted and altered with injections.
- XSS (Cross Site Scripting): The implementation of malicious JavaScript code. JS is the underlying code that runs allows HTML websites to do logical tasks.

- Pointer/ Object Deference: A pointer (AKA the piece of code that tells an OS where to find the rest of the information on a hardrive) can point to the wrong location and cause a crash
- Directory Traversal: Inspecting directories (AKA the folders on your PC) to plan out a potential attack or espionage
- Error Handling: The way in which an application handles a error. For example, if the user types a letter where numbers are expected its better for an app to say something like "Error: Passcode may only contain numbers" instead of simply crashing.
- Impropert Input Handling: The flawed acceptance of incorrect values or formatting. This is what allows injections to happen.
- Buffer Overflow: When a buffer (or section of memory reserved for a specific purpose) receives too much data that it overflows to other pars of the RAM; and thus corrupting the data in the neighboring buffer.
- Race Conditions: When two different processes run simultenously, but must finish in specific orders. If the secondary processes finishes their tasks before the expected first process, a problem can occur. A common example of this is Time of Check and Time of Use race conditions. Imagine two people that want to buy the same anime figure on ebay. Suppose that when someone purchases the figure, it will change its status to "Sold"; and it only checks for the availability of the product when its added to checkout cart. If Bob and Albert both have the same figure in their cart, but Bob buys the figure first; Albert might also incorrectly purchase that same figure that in reality is sold out. So what's the race condition here? The check of availibility from Albert races the Purchase (or Use) from Bob. This is why its best practice to have your checks and uses of resources as close as possible. In real life, ebay would have checked the availibility of the anime figure right before purchase instead of when it was placed on the cart, thus minimizing the possibility of a race condition.
- Replay Attack: Resending legitimate info for a fradulent response. For example, [I clone your car keys using the same signal that your legitimate car keys send to unlock your car.](https://www.youtube.com/watch?v=uxzm_6SYBFo) (PSA. Don't try this at home and also consider buying a Faraday cage.) (but if you do want to hack a car, remember that rolling codes exist and you really need to capture the signal out of reach. See [Spider-man stole that guy's pizza (using a FlipperZero)](https://github.com/Cham0i))
  - Session Replay: A session ID is reset to a server from a hacker to obtian access to the target's session
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

- Evil Twin: Fradulent copycat of a WAP
- Rouge Access Point: A sketchy WAP. vague SSID, location is odd, sus.
- BlueSnarfing: Hacker connects to unsecured bluetooth connection for contact, notification, data. etc.
- BlueJacking: Connecting without pairing/ authentication. This is an old vulnerability, most modern bluetooth devices require pairing.
- RFID: Radio Frequency Identification. The tech used in NFC
- NFC: Near Field Communications. Tap to pay. Security Badges.
- IV: Initialization Vector: Piece of keystream used per session (frame). (Will be explained better some other day)
- On-Path/ Man-in-the-middle Attack: Routing data through a hacker's machine so that the data is viewed.

**Layer 2 Attacks (Data Link)**

- ARP (Address Resolution Protocol): You should know this by now (See [this](https://github.com/Cham0i/Netacad?tab=readme-ov-file#encapsulation-address-resolution-protocol-arp-mac-address-table-and-routing-tables))
  - ARP Poisining: Spoofing a fake MAC so that the ARP cache is inaccurate
  - MAC Flooding: Registering an overwhelming amount of new MACs to the MAC table to force the switch to act as a hub
  - MAC Cloning: Using someone else's MAC

**DNS**

- Domain Hijacking: Taking control over a domain
- URL Redirection: Redirecting from a URL to another site
- DNS Poisining: Adding spoofed DNS cache to be spread by other DNS servers
- Domain Reputation: Maliciously blacklisting domains can hurt their potential views on the web.

**DDos**

- Distributed Denial of Service: Multiple bots send multiple requests to strain an app, server, network, operational tech, etc.

**Malicious code or script execution**

Powershell, Python, Bash, Macros, VBA, can all change file permissions, NTFS permisions, change IP addresses, names, manipulate files etc. Execution policies, constrained language mode and even the complete deletion of these tools can provide better security.

## 1.5 Threat vectors, Actors, and intelligence sources

**Actors and Threats**

- APT (Advanced Persistent Threats): Hackers that will always attempt to hack you
- Insider Threats: Threats within your organization. Either traitors or incompetent people
- State Actors: Government sponsored hackers (China, Russia, North Korea)
- Hacktivists: Hackers motivated by politics
- Script Kiddies: Noob hackers that use other people's scripts
- Criminal syndicates: Hackers for illegal profits
- Shadow IT: Unauthorized modifiers of apps and policies
- Competitors: Business rivals

**Attributes of actors**

1. Internal or External
2. Sophistication level/ Capabilities
3. Resources and funding
4. Intent and motivation

**Vectors (Pathways for entry)**

- Direct Access: Coming through the router
- Wireless: WAP, Bluetooth, cell
- Email
- Supply Chain Attack
- Social Media (Social Engineering)
- Removable Media (Bad USB)
- Cloud

**Threat Intelligence Sources**

- OSINT (Open Source Intelligence): Free, public, information
- Closed/ Proprietary: Paid, closed off from the general public
- Vulnerability databases: Databases of known vulnerabilities

ISAC (Information Sharing and Analysis Center) Established after 9/11. ISAC ensures that public and private forums communicate with each other using AIS (Automated Indicator Sharing).

Darkweb: The .onion sites. Illegal activity.

- IoCs (Indicators of Compromise): Evidence to believe a hack occured
- STIX/ TAXII: DHS specifications for cybersecurity sharing
- Predictive Analysis: Anticipation of incident, often using AI to guess hardware failures or network overload.
- Threat Maps: Geographic representations of past attacks
- File/ Code repositories: Storage area for data/ code (Hello, you currently viewing this repository for Sec+ right now)

**Research Sources**

## 1.6 Security Concerns with various types of vulnerabilities

## 1.7 Techniques used in security assesments

## 1.8 Pentesting techniques

### 2.0 ARCHITECTURE AND DESIGN

## 2.1 Security Concepts in enterprise enviroments

Will he finish uploading all of his old sec+ notes to his github? Find out in the next episode of Dragon Ball Z

R.I.P Mexico
