# firewalls (ufw)
#STEPS FOLLOWED:

Installed UFW (Uncomplicated Firewall) in my pc. </br>
Run: sudo apt install ufw

1.Enable UFW: sudo ufw enable</br>
2.Check status: sudo ufw status verbose sudo ufw status numbered </br>
3.Block inbound traffic on port 23: sudo ufw deny 23 </br>
4.Tested the block rule using telnet: telnet localhost 23 It shows: Unable to connect to remote host: Connection refused </br>
5.Allow SSH traffic port 22: sudo ufw allow 22 </br>
6.Remove the test block rule to restore original state: sudo ufw delete </br>

#SUMMARY: </br>
In thi task, I confiured firewall rules on my PC using kali linux. I listed the current rules, then created a new rule to block inbound traffic on port 23 (telnet) and tested that it worked. I also added an allow rule for SSH (port 22) to ensure remote connection remained possible. Finally, I removed the test blockk rule to restore the firewall to its original state. The process helped me understand how firewall rules filter network traffic and how to manage firewall configuration effectively.
