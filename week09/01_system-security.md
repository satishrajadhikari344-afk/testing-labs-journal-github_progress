# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

(Add screenshot here)

### Questions

1.  How many users exist on the system?
2.  Which accounts appear to be system accounts?
3.  Why do operating systems create system accounts?

### Reflection

Explain why understanding system users is important for cybersecurity.

------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`?
   Process with root in the first column are running as root:
systemd
kthreadd
cron 
sshd
NetworkManager
   3. Why can processes running as root be dangerous?
  Root processes have full control over the system because there are several reason: 
 a.Access all files
b.Change system settings
c.Install or remove software
d.Create or delete user accounts
If a root process is compromised, an attacker could gain complete control of the system.
4. What could happen if a malicious program ran with root privileges?
A malicious program running as root could:
a.Steal sensitive data
b.Delete important files
c.Install malware
d.Create backdoor accounts
e.Disable security features
f.Take complete control of the computer
  ### Reflection
  what did you learn about system processes and security?
I learned that system processes keep the operating system running and many of them require special permissions. Processes running as root have powerful privileges, so it is important to monitor them and follow the principle of least privilege. Limiting root access helps improve system security and reduces the risk of attacks.

------------------------------------------------------------------------

## Task 3 --- Identify Open Network Ports

Run:

    ss -tuln

### Screenshot

(Add screenshot here)

### Questions

1.  Which ports are open?
2.  Which services appear to be listening?
3.  Why might open ports represent a security risk?

### Reflection

Explain the relationship between open ports and potential attack
surfaces.
