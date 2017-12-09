# week9
Time spent: 16 hours spent in total

This week we set up honeypots on the cloud to *lure* attackers to try and attack our machines in order to learn what kind of techniques they use, what their ultimate goals are, and hopefully capture some malware samples.


## Which Honeypot(s) you deployed
I deployed two honeypots, dionaea - a low interaction honeypots whose goal is to get malware exploiting vulnerabilities exposed by services exposed to a network   
and p0f - which attempts to fingerprint various attributes of the attackers machine. 

## Any issues you encountered
At first I was not able to create firewall rules from the command line, because the Compute Engine API was not enabled in the project settings. That made the firewall creation process appear to take an infinite amount of time. Upon enabling it, firewall rules were created within a few seconds. Inclusion of this step in the tutorials would have saved a considerable amount of time.

Secondly, I was unable to log into the mhn-admin panel, due to firewall configurations. Apparently, the firewall rules created during the assignment are not automatically applied (or did were not sufficient) to allow http / https request to be made. I had to manually configure the firewall from the GCP settings in order to fix this.

## A summary of the data collected: number of attacks, number of malware samples, etc.
None of the attackers provided any malware samples.
