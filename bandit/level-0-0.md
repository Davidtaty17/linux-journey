# LEVEL 0  : Log into the game using ssh

Host: bandit.labs.overthewire.org
port: 2220
user: bandit0
commands given: ssh 

**Useful commands**: ssh

## How to solve this level?


=> Log into the game using ssh command, " **ssh -p port_number user@IP**"  

=> Log out with **CTRL + D** or **exit**.

## Observations 


1. **ssh** (Secure Shell) is an encrypted protocol used to connect and control a remote computer over a network securely.

   *-p* here means the port is the argument
   
2. I learned that a host can be an IP address or a hostname.
  IP address -> Numerical, not user-friendly
  Hostname -> Human friendly name
   
3. **DNS** (Domain Name System) is a system that translates human-readable hostnames into numerical IP addresses. 
