LEVEL 0 : Log into the game using ssh.

Host: bandit.labs.overthewire.org
port: 2220
user: bandit0
commands given: ssh 


command for this mission: ssh -p port_number user@IP 
Like we do not have the IP. The game given us just the hostname and that ssh accepts both, "IP addres" and the "Hostname".
The computer will handle the translation automatically via DNS.
So our command will be: ssh -p 2220 bandit0@bandit.labs.overthewire.org
