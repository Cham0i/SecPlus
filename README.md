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

- Priviledge Escalation: Giving an unauthorized user more priviledges (User to Admin priviledges)
- Cross Site Scripting (XSS): The user of a clean website takes advantage of an improperly configured input, such as a comment section, to implant malicious JavaScript code

**Injections**

- SQL
- DLL
- LDAP
- XML

## 1.4 Hacking Networks

**Wireless**

**Layer 2 Attacks (Data Link)**

**DNS**

**DDos**

**Malicious code or script execution**

## 1.5 Threat vectors, Actors, and intelligence sources

**Actors and Threats**

**Attributes of actors**

**Vectors (Pathways for entry)**

**Threat Intelligence Sources**

**Research Sources**

## 1.6 Security Concerns with various types of vulnerabilities

## 1.7 Techniques used in security assesments

## 1.8 Pentesting techniques

### 2.0 ARCHITECTURE AND DESIGN

## 2.1 Security Concepts in enterprise enviroments

Will he finish uploading all of his old sec+ notes to his github? Find out in the next episode of Dragon Ball Z

R.I.P Mexico
