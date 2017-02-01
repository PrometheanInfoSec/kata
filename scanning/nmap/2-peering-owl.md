#Peering Owl
##Scanning -- Nmap -- Form2

###Description
The purpose of this form is to teach how to identify who else may be on your network whether friend or foe.

The network will be listed as <###.##.#.0/24>. Replace the # with your target network. (ex. 192.168.0.0/24)

###Execution
We will first perform a scan that sends no packets to the target.
1>> **`nmap -sL <###.##.#.0/24>`**

Next we can perform a simple ping sweep that will send icmp packets but is far more reliable.
2>> **`nmap -sn <###.##.#.0/24>`**

###Explanation
In step one we perform a no packet scan that uses reverse DNS lookup to try and find different machines on the network. 

Since the scan in step one isn't always reliable we do a ping scan which will return a list of all active machines that resonded to the ping sweep.
