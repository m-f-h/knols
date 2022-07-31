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
  
### Drupal
* main link: [my Drupal repo](/../../../drupal)
* Find out the frequency of releases: we installed 9.4.1 on Beinning of July, but 9.4.3 was aloready released, by the end of July 9.4.4 was released...!! 
* ...
## Solved problems
### Drupal
* main link: [my Drupal repo](/../../../drupal)
* [differential core update](/../../../drupal/tree/main/core_update)

### WSL vs CygWin and Ubuntu vs Debian
31.7.22 : We've just learned about [WSL - the Windows Subsystem for Linux](https://docs.microsoft.com/windows/wsl/about)

is it better than Cygwin? read here:
- [Compare the difference between Cygwin, MinGW and WSL](https://ericzhng.github.io/eric-blogs/2019/07/25/comparison-cygwin-mingw-wsl/)
(good description of Cygwin vs MinGW but almost nothing on WSL ()
- [WSL vs Cygwin. Should I migrate?](https://www.reddit.com/r/windows/comments/a8innb/wsl_vs_cygwin_should_i_migrate/)
(among the replies: 110% WSL. once set up correctly, it integrates absolutely perfectly with the rest of your toolkit) 
- [Cygwin vs WSL2 - which is (currently) faster?](https://www.reddit.com/r/sysadmin/comments/fckypi/cygwin_vs_wsl2_which_is_currently_faster/)
- [Cygwin vs Windows Subsystem for Linux](https://www.slant.co/versus/11867/24657/~cygwin_vs_windows-subsystem-for-linux)
- [MS : install](https://docs.microsoft.com/en-us/windows/wsl/install)
==> we chose to give WLS a try

Q: which distro to install?
  - [Debian vs Ubuntu: What’s the Difference? Which One Should You Use?](https://itsfoss.com/debian-vs-ubuntu/)
  Ubintu is based on debian ; intermediate between Deb stable (aka stale) and testing
  - [Debian vs Ubuntu: Which distro is best for you?](https://www.techrepublic.com/article/debian-vs-ubuntu/)
  - [Debian vs. Ubuntu Linux: Which Distro Should You Choose?](https://www.howtogeek.com/749045/debian-vs-ubuntu/)
    * Debian Has Lower System Requirements.
  
    A Debian 11 desktop install requires at least a 1GHz processor, 1GB RAM, and 10GB storage. Ubuntu Desktop more than doubles those requirements with a 2GHz dual-core processor, 4GB of RAM, and 25GB of disk space.
   
    That said, when we tested ... didn’t differ significantly, using about 1GB of RAM at idle. 

    * Ubuntu Makes Proprietary Software Easier to Get
    * Debian Supports Older Hardware
    * Ubuntu Is Corporate-Backed
    Ubuntu is maintained by an organization called Canonical. Debian, in contrast, is developed completely by a community of volunteers. 

  It looks as if we'd stick to the default = Ubuntu for our WSL install
  
