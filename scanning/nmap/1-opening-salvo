#Opening Salvo
##Scanning -- Nmap -- Form 1

###Description
The objective of this form is to practice all of the general basics of a scanning run against a target of opportunity.

The target will be listed as <target> throughout.  Replace that with your target's IP.  (127.0.0.1 if you don't have one)

###Execution
First perform a ping scan against your target to see if they're online.
1>> **`nmap -sn <target>`**

Now assuming they were online perform a syn stealth scan to avoid triggering honeyports.
2>> **`nmap -sS <target>`**

Now you're ready to perform a full connect scan.  Let's do the first 1000 ports.
3>> **`nmap -sT  -p1-1000 <target>`**

Finally perform OS detection on your target.
4>> **`nmap -o <target>`**

###Explanation
In step one we performed a ping scan against our target to quickly determine whether or not they were online.  Obviously if the host doesn't respond to ICMP.  Or if ICMP is dropped somewhere between you and the target this won't work.

Step two has us perform an initial scan of the target host without performing a full TCP connection.  We use what is known as a "SYN scan."  This keeps us from triggering any listening honeyports.

Next in step 3 we perform a full TCP connect scan of all of the first 1000 ports on our target.  By default nmap only scans the 1000 most common ports.  Not all of the first 1000.  So if we want to be complete we might use an option like this.

Finally we perform OS detection in step four.  Nmap has a built in list of signatures for different OSes and sends specially crafted packets to the target gauging the response to determine if a match for a one of its signatures is found.
