# cyberrange
Cyber ranges are designed to model corporate networks or the internet.  They can be used for validating blue team tools (does the tool prevent or detect what it's supposed to?).  They can be used for testing red team tools (are they appropriately modeling a threat?).  They can be used for free-play CTFs.  They can be used...well, you get the idea.

## What this is
Cyberrange will have a reference infrastructure (probably several), but the real goal of this project is to help highlight techniques that can be used to help model a range and some of the unique challenges therein.  For example, how should you bootstrap your range?  Many ranges will have no internet connectivity and you probably don't want the players to easily access the build infrastructure.  How will you insert vulnerabilities on your range?  A common technique is to just download machines from VulnHub (https://www.vulnhub.com/) and deploy them.  There's certainly nothing wrong with this, but if you built the range you also know what vulnerabilities to expect.  How will you model users? How will you model the internet? Where will you run it? How many users do you have to support?  How will they get access?

# Helpful Resources
https://github.com/secdevops-cuse/CyberRange
Thomas Cappetta has put together a great toolset here targeted at AWS.  He has expressed in the past that AWS is his preferred platform (or at least a cloud provider of some sort), but he does have a blog post on locally building a range: https://medium.com/aws-cyber-range/building-an-on-site-cyber-range-74f7112ac975

https://www.vulnhub.com/
This is a great selection of prebuilt vulnerable machines.  They may need some massaging to deploy in your target network.

https://github.com/cliffe/SecGen
This is another great tool built with VirtualBox, Packer, Puppet, and Vagrant.  What's especially interesting about it is the random VM generation so that you truly don't know what vulnerabilities will be on a box.
