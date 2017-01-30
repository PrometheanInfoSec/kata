#Eye of the Oracle
##Scanning -- Nmap -- Form 3

###Description
This form teaches a few more advanced scanning techniques that can be used in a practical environment.

Replace <target> with the IP of your target machine.

###Execution
First perform a ping scan against your target to see if it's online.
1>> **`nmap -sn <target>`**

Perform a full syn stealth scan with verbose output and OS + Version detection.
2>> **`nmap -v -A -sS -T4 <target>`**

Use nmap to find and display a Netbios name from your target (assuming it is running gsuch a service).
3>> **`nmap -sU --script nbstat.nse -p 137 <target>`**

Scan only the top ten most common ports outputting to xml.
4>> **`nmap --top-ports "10" -oX top10.xml <target>`**

##Explanation
In step one we perform a ping scan against our target to see if it is online.

In step two we use -v for verbose output, -A for OS and version detection, -sS for a SYN stealth scan, and -T4 for aggressive timing.  This is a complete scan command.  Something that can get you everything you need.

In step three we use a script to detect the netbios name of our target (assuming they are a windows device running netbios).

In step four we show a simple and easy scan of only the top ten most commonly used ports for our target, outputting the scan to a file in XML format.
