## Security Threats and Countermeasures

Types of security threats to operating systems
- Intruders
- Malicious Software
- Buffer Overflow

**Intruders**
- Intruders are hackers who poise threats to the OS
- Three classes of intruders:
  - Masquerader (Usually Outsider) - one who breaks the system's access controls to impersonate as a legitimate user
  - Misfeasor (Usually Insider) - a user who misuses his or her privileges or access resources which he/she doesn't have the authorisation
  - Clandestine (Insider/Outsider) - one who gets root control of the system and bypasses access control

**Malicious Software**
- Two groups
  - **Independent** - referred to as self-contained programs, and can be run by the OS. (e.g. worm)
  - **Need a host program** - referred to as parasitic, and they need to attach to another program (e.g. virus)
- Can cause disaster, such as destroying files and bypass access control

**Buffer Overflow**
- Can occur due to programming error when a process attempts to overwrite adjacent memory location
- Can result in attacker able to gain control in the program
- Attacker can use Metasploit against unpatched system (that is vulnerable to buffer overflow) and get a shell remotely

**Countermeasures**
- Authentication
- Access Control
- Buffer Overflow Countermeasures

**Authentication**
- To identify and verify that the users are who they claim to be
- Methods that OS can use to authenticate:
  - Something you know (e.g. username and password)
  - Something you have (e.g. ATM card, Access Card)
  - Something you are (e.g. biometrics such as fingerprint, iris)
- To enhance the security, two or more factors can be implemented

**Access Control**
- Access Control system works hand in hand with the authentication system
- After the system authenticates who you are, the system can then give you the correct access rights

**Buffer Overflow Countermeasures**
Two broad categories:
- **Compile-time Defence** - aims to resist the attacks by hardening the programs
- **Runtime Defence** - aims to detect and stop attacks in executing programs

## Operating Systems Hardening
Operating system hardening is the process of securing an OS by reducing its attack surface. This involves disabling or removing unnecessary services, applications, and open ports, since leaving them enabled can introduce vulnerabilities or weaknesses that attackers may exploit to compromise the system.

- Steps of hardening OS:
  - OS installation and patching
  - Remove unnecessary services, applications, and protocols
  - Configure user, groups and permissions
  - Install and configure additional security controls
  - Test the system security

**OS installation and patching**
- Proper planning in installing an OS is important




















































