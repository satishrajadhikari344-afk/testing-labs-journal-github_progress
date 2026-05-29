# Exploring Your System's Security

## Task 1 --- List System Users

Run:

    cat /etc/passwd

### Screenshot

(Add screenshot here)

1.  How many users exist on the system?
There are 35 users on the system.
3.  Which accounts appear to be system accounts?
   root
   daemon
   bin
   sys
   nobody
   www-data
   systemd-network
   systmed-timesys

5.  Why do operating systems create system accounts?
   Operating systems create system accounts do :
Run background services securely
Seperate permissions between services
Protect the system from unauthorized access
Manage system processes automatically

### Reflection

Explain why understanding system users is important for cybersecurity.
Understanding system users is important for cybersecurity because it helps identityfy who can access the system and what permissions thry have. System accounts allow services to run safely with limited acess, reducing security risks. Monitoring user accounts also helps detect unauthorized access and protect sensitive data.

------------------------------------------------------------------------

## Task 2 --- Inspect Running Processes

Run:

    ps aux

### Screenshot

(Add screenshot here)

### Questions

1.  Which processes are running as `root`?
2.  Why can processes running as root be dangerous?
3.  What could happen if a malicious program ran with root privileges?

### Reflection

What did you learn about system processes and security?

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
