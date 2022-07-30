# knols
Created 30.7.2022 by M. F. Hasler

(My) Knowledge (and/or "How-To") units: A collection of useful information and "How-To"s, in "modular" form.

**This is made public so it can be useful for the largest possible benefit. <br/>
Any contributions are more than welcome! <br/>
If you find this useful, contribute and/or let us know otherwise how it helped you or what you are missing here.**

We expect this to grow by creating new entries for "problems" or nontrivial tasks we have to solve. <br/>
These problems will often be divided up in more elementary tasks which will finally become a "knol" once we know a solution. <br/>
We also expect these to be not always static, but evolve as we learn about better or alternative ways to solve the problem.
As this "knowledge base" grows, the sections will be conveniently structured and reorganized.
Whenever parts are outsourced to subdirectories and/or other files, we'll try our best to make it easy to find the new location for all those who have "bookmarked" the original file -- i.e., keep at least the title of all outsourced sections, with an indication to where the material can be found in future editions of this knowledge base.

## Open problems
Part 1: related to Applied Computer Science. In particular, web site design, management, maintenance, ... and all that's related: Drupal, Hosting plans, MySQL and alternatives, PHP, SQLite, SSL

### SSL
* How to install and/or use OpenSSL: There's a Python lib OpenSSL and 
  
  - We found ssl.py in C:\Program Files\MySQL\MySQL Shell 8.0\lib\Python3.10\Lib\site-packages\OpenSSL
  - Could that be used to create certificates?
  
  
* How to create & store SSL certificates
  - We found the following ressources:
  - [IT: How To Create a Self Signed Security (SSL) Certificate and Deploy it to Client Machines (How-To Geek.com)](https://www.howtogeek.com/107415/it-how-to-create-a-self-signed-security-ssl-certificate-and-deploy-it-to-client-machines/)
    - Suggests to use SelfSSL from the IIS 6.0 Resource Toolkit
    - link provided (not sure whether this still works as is...): https://click.linksynergy.com/deeplink?id=2QzUaswX1as&mid=24542&u1=htg/107415&murl=http%3A%2F%2Fwww.microsoft.com%2Fdownload%2Fen%2Fdetails.aspx%3Fid%3D17275)] 
    - explains how to use `selfssl` create the SSL (but it remains "hidden")
      and how to use mmc ((certificate?) management center) to find it and copy-paste it to a more visible location
  - [How To Create Free SSL Certificate For Your Website?](https://technicalwall.com/blogging/free-ssl-certificate/)
    - suggests to use "Let's Encrypt" for non-commercial or "Let's Certificate" for sites accepting payment, or hosting providers (+ list of names: affiliate...) that provide free SSL certificates, or
    - sslforfree.com is offering 90-day free SSL certificates in partnership with ZeroSSL.
    then better:
  - https://help.zerossl.com/hc/en-us/articles/360060119373-Creating-an-SSL-Certificate
  

## Solved problems

