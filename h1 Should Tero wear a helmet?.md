# Threat Modeling  Manifesto - Summary 

## What is threat modeling?
- Threat modeling is the process of analyzing representations of systems to draw attention towards the security and privacy characteristics and concerns before they can be exploited.
- At the very top level, when we do threat modeling we ask four key question that are:
-  What are we working on, what can go wrong, what are you going to do about it, and did we do a good enough job?
  
## Why do we do threat modeling and who should threat model? 
- Threat modeling allows to pinpoint design and implementation issues, we do the threat modeling to understand what might go wrong with the system.
- Everyone who feels concerened about their privacy, security and saftey of their system.
  
## How to use Threat modeling manifesto 
- Threat modeling manifesto is a guide to develop or refine a methodology that leads to best and effective security practices of our systems.
- Threat modeling manifesto follows a similar format to that of agile manifesto which is Using frameworks of values and principles.
- "Values" in threat modeling is something that has more of a importance and relatively of more worth than others, focusing on what brings more merit or value.
- Principles outlines fundamentals truth of threat modeling, in threat modeling there are three types principles which are fundamental truths, recommended patterns, and anti-patterns to avoid.
  
## Adam Shostack Threat Modeling videos - Short summary 
- We threat model to anticipate problems before anything else is done like coding or building any infrastructures.
- Data flow diagrams are heavily associated with threat modeling because threats tends to follow with the data. Five elements make up the data flow diagram are external entities, processes, data stores, data Flows, boundaries.
- The Most important key question at the heart of threat modeling is What could go wrong?. After asking this question we should come up with the answers and specially pay attention to the conclusive answer to these questions.
  
## Infosec scene - Darknet Diaries - episode 137 - Predetor 
- This episode explains about the global mercenary spyware industry, especially showcasing Predator spyware.
- Predator is a high-end mobile surveillance tool capable of fully exploiting cellphones.
- Developed and sold by a network of private companies led by Tal Dilion.
- Spyware was sold to governments and entities with poor human-rights records.
  The Predator spyware is used to target journalists, politicians, and civil society, amongst others.
- Infections relied on phishing links and browser exploits, leaving little to no traces.
- This showcases how attackers exploit software vulnerabilities and phishing techniques to gain covert access to smartphones
  
# a) Security Hygiene 

## What basic security practices should everyone follow?
- Be cautious to unknown links, attachment, emails from unknown sender/origin.
- Use strong passwords and unique ones in every different websites that we log in.
- Enable multi-factor authentication.
- Lock devices and update devices drivers and operating systems.
- Regularly backup important data.

## What security practices should every companies follow?
- Perform regular threat modeling to identify, prioritize, and manage security risks.
- Use firewalls, and regular security sweeps in the system.
- Use encryption methods to protect the data.
- Implementation of regular backup system, and protect internal system throughly.
- Strictly mandating the Multi-factor authentication (MFA) for all the employees, administrators of the companies.
- Employees should be made aware of the security risks and should be trained on many aspects of security hazards in real life like phising or spam emails.

# b) Make-belief boogie-man - Threat Model for Imaginary Company

**Company name:** Ease Wallet Oy   
- Ease Wallet Oy is a Finnish Fintech company which provides its customers with a very easy to use digital wallet and mobile payment platform system. Ease wallet allows users to transfer money from any bank in the world to their wallet system with no charge policy, make payments and exchange currency in good exchange rates. 

**Business requirements:** The Ease Wallet Oy service must be fast, easy to use, reliable, and available so customers keep using it. As this is a financial tech company it should be heavily secure and customers should feel at ease that they can do secure transactions everytime. One error or a flaw can be detrimental for this company. Therefore 
Cyber Security Professionals (Technical specalists) must support and secure the business by ensuring the platform is secure, stable, and compliant 24/7.

## 1) What are we working on?
### Our Assets 
- Customer funds stored in our digital wallets
- Customer personal and financial information
- Transaction data and payment history
- Mobile application and backend services
- company goodwill and trust

* Customers funds and their transfers, exchanges and transactions are the most critical assests to our company. Security supports the business by protecting the funds, prevention of any kinds of frauds and maintaining clients trust. 

- Customer is the king, so to serve our customers well and to keep our company business thriving, we have to make our financial wallet system secure, easy to use, fast funds transfers/exchange, better exchange rate and 24/7 uptime. 
- The customer interacts with Ease wallet through Mobile Apps, currancy exchange, sending and recieving money, viewing wallet balance etc.

## 2) What can go wrong?
### Threat Modeling approach 
The stride and CIA model are used 

### Examples of some identified risks
- Fradulent transactions (Tampering, Integrity)
- Stolen Credentials (Spoofing, Confidentiality)
- Breach of personal or financial data (Information disclosure)
- Service delay or outages (Denial of service, Availability)

### Prioritized risks 
- Financial fraud leading to direct financial loss 
- Data breach damaging customer trust and causing regulatory issues
- Service downtime & delay in service, impacting customers directly (bad user experience) and business continuity

### Threat actors
- Cybercriminals targeting usually to major fintech services for financial or reputation gain
- Organized fraud groups using phishing
- Opportunistic attackers exploiting exposed APIs

### Known TTPs
- Phishing and social engineering
- Credential stuffing
- Abuse of weaker security systems and authentication mechanism 

### Capability, Opportunity, Intent - COI
- Capability: Common tools and skills are widely available
- Opportunity: Online payment services
- Intent: Direct financial benefit

### Business continuity
- The Fintech services provided by Ease wallet must continue to do it. 
- Trust is a very critical factor as our customers expect their money to be safe, relaible and transfers/exchanges to be fast. Loss of trust would seriously impact the business.

## (3) What are we going to do about it?

### Attack surface reduction 
- Disabling vulnerable and unnecessary ports. (entrypoints)
- mitigating software vulnerabilities.
- best security practices for cloud infrastructure
- removing inactive accounts or temporary banning them until Know your customer (KYC) update.
- limit external access to only necessary APIs and endpoints.

### Risk handling (META)
**Mitigate:**  
  - Strong authentication and mandatory MFA  
  - Encryption of sensitive data  
  - Monitoring and flagging fraudulent transactions
  - flagging the suspicious activity and devices
 **Eliminate:**  
  - Remove unused accounts
  - ban the devices with wrong intentions
  - banning the fradulent devices and reporting it to the authorities
    
**Transfer:**  
  - Use trusted third-party payment providers  
  - Cyber insurance to cover risks
    
 **Accept:**  
  - Acknowledge the Low-impact risks that doesn't pose immediate risk, we do accept minor downtimes on our main servers which will be covered by our backup servers.
  -  



## (4) Did we do a good enough job?

- Perform regular security audits and assessments
- Conduct penetration testing when we change our systems or have major updates and upgrades. 
- Continuously update the threat modeling procedures as the business evolves
- Review incidents and improve controls

**Threat modeling is an ongoing process and its not a one time job, so we need to keep on doing it, It never ends!**








