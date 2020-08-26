Webmin is excellent if you wish to have a web-based interface for system administration.
It removes the need to manually edit configuration files and makes administration a lot easier.

Installing Webmin

1. First, make sure Raspbian is completely up to date by running the following commands.

    sudo apt-get update

    sudo apt-get upgrade


2. preparing system for installing all the required packages of Webmin.

    sudo apt-get install perl libnet-ssleay-perl openssl libauthen-pam-perl libpam-runtime libio-pty-perl apt-show-versions python
    
3. Download the required deb file check the latest version form here
   http://www.webmin.com/deb.html
   

    wget http://prdownloads.sourceforge.net/webadmin/webmin_1.900_all.deb
    
4.  Once the downloaded, run dpkg
    
    
    sudo dpkg --install webmin_1.900_all.deb
    
    It may take some time to install.
    
5. Find out the Raspberry Pi’s IP address by using hostname -I

    Below is an example of my address to access Webmin.

    https://192.168.43.1:10000
 
 6. You will receive a warning because the SSL will be invalid. 
    It is safe to ignore this as we can’t receive a valid SSL certificate on an local IP address.

 7. the username will be pi and the password will be raspberry.
