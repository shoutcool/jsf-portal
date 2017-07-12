jsf-portal
==========

Lightweight JSF 2 portal-like implementation with test web apps (POC)

> **Adopted to run on Tomcat 8.5:**

> - Added JBoss Weld
> - Tested on Tomcat 8.5.16
> - To get the primefaces maven repository work you need to add the ssl certificate to 
    your jre keystore (cacerts)
<br>   
   
   
Example for MacOS

    $ openssl s_client -showcerts -connect repository.primefaces.org:443 </dev/null 2>/dev/null|openssl x509 -outform PEM >mycertfile.pem
    $ sudo /Library/Java/JavaVirtualMachines/jdk1.8.0_73.jdk/Contents/Home/bin/keytool -importcert -file mycertfile.pem -keystore /Library/Java/JavaVirtualMachines/jdk1.8.0_73.jdk/Contents/Home/jre/lib/security/cacerts 
    
