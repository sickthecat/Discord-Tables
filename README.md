# Discord-Tables
Let's confuse the phuck out of nmap.

# These rules:

Set the default policies to DROP, meaning that all incoming and outgoing traffic is dropped unless it matches a specific rule.
Allow established connections to continue.
Allow incoming connections on two non-standard ports that are unlikely to be open on most systems.
Allow outgoing connections on common ports to ensure that basic internet connectivity is not affected.
Drop packets with invalid TCP flags or unusual combinations of flags.
Limit the rate of incoming SYN packets to make it harder for a scanner to detect open ports.
Randomize TCP sequence numbers to make it harder to predict what ports are open.
Implement a stealth DROP for some TCP ports, meaning that the connection is immediately dropped without sending a response, which can make it harder to determine whether the port is open or closed.
