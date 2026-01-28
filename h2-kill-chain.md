# h2 Kill Chain 
## x) Hutchins et al. 2011 - intrusion Kill Chain 
- Intrusion kill chain is an integrated, structured mode of attack where a single faliure in any steps interrupts the entire operations.
- It is borrowed from the military targeting doctrine (F2T2EA), which is a model that treats a intrusion as a chain of dependent steps.
- There are seven phases in this model.
- By proper analysis of the attacks through this phases, defender can identify vulunerable points and also secure those weak points at a multiple stages.
- This article showcases the modern cyber attacks which are properly planned and analyzed and not a random attack, which enables the cybersecurity professionals to understand the behavior and thought patterns of attackers. 
  
### Seven phases of intrusion kill chain: 
1. Reconnaissance:
- Searching and selecting the targets for example via publicly available emails and social informations.
2. Weaponization:
- In this phase attackers start with weaponizing their attacks usually by creating a exploit and malwares/viruses.
- Making an exploit with a backdoor into a deliverable payload for e.g. malicious files.
3. Delivery:
- In this phase, Delivery of the weapon is initiated to the victim.
- Usually target receives this delivery via emial, Phising websites, USB stick etc.
4. Exploitation:
- The execution of the intruder malicious code/attack occurs inside the victims systems.
- The system is exploited and the attacker could target many vulnerablities.
5. Installation:
- Installation occurs in this phase, the persistent backdoor of somesorts like remote access trojen.
6. Command and Control (C2):
- Infected system of the victim connects to attacker controlled infrastructures.
- This also Enables remote control (“hands on keyboard”) for the attacker.
7. Action on objectives
- Completing the original objectives, such as data theft, lateral movement, espionage, or system disruption.

### My Thought about this article - Intrusion Kill Chain
- This was really interesting and insightful read for me as it describes the actual kill chain concept which helps defenders on a cyber attack to predict analyze and adapt the step by step process used in an specific attack. By breaking down like this, securtiy teams and professionals can focus on each steps and prevent or defend from a kill chain. 

## a) Tactics, tools and procedures
### Tactics 
- A tactic is the attackers goal and represents "the why" of an attack.
- Tactics represents it is not a particular approach, but rather a stage of adversarial purpose.
- Example of a specific tactics would be an adversary may want to achieve credential access.
- 
### Technique 
- Technique is the method to achieve a specific tactic.
- A Technique is "How" the general method will or can be used to achieve a tactic.
- Example of a technique: an adversary may dump credentials to achieve credential access.

### Sub-technique 
- Sub-technique is more specific description of a technique.
- Example of a sub-technique : an adversary may dump credentials by accessing the Local Security Authority (LSA) Secrets.

### Procedure
- Procedure are the specific implementation of a technique or sub-technique that adversory uses.
- A procedure are catagorized as the observed in the wild implementation or instance of an attack.
- Example of procedure could be an adversary using PowerShell to inject into lsass.exe to dump credentials by scraping LSASS memory on a victim.

### MITRE ATT&CK key insights
- The FAQ section of the website makes it clear about all the procedures techniques and tactics behind a attack. I learned real life examples from the website and also real-life ATT&CK stories which made me aware about different sorts of tools and process used while attacking a victim.

## c) Voluntary Bonus: Attack Story



# Sources 

- Karvinen 2024: Information Security Course. URL: https://terokarvinen.com/information-security/
- Hutchins et al. 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains. URL:  https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf 
- MITRE 2024: ATT&CK Matrix for Enterprise. URL: https://attack.mitre.org/
- MITRE 2024: MITRE ATT&CK FAQ. URL: https://attack.mitre.org/resources/faq/

