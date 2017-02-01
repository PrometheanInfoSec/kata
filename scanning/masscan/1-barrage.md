#Barrage
##Scanning -- Masscan -- Form 1

###Description
This simple form shows how to use masscan to quickly scan an entire portion of the internet.

###Execution
Scan an entire sector of the internet for an ssh server on port 22.

Replace <base_ip> with something like 10.0.0.0 and <cidr> with something like /8 (or /16, /24, etc).  Google "CIDR Notion" to learn more.

1>> **`masscan <base_ip>/<cidr> -p 22`**

###Explanation
Masscan is an incredibly fast scanning tool.  It can scan at speeds far in excess of what nmap is capable of.

In step one we scanned an entire section of the internet for ssh servers.


