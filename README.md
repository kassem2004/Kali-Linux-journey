# Kali-Linux-journey

Hello this will be a documentation of my journey of learning Kali Linux,
I will be using VirtualBox to set up my Virtual Machines, then exploring
and learning how to use Kali Linux and its tools.

# Linux
Commands learnt:
```
sudo  | Runs commands with superuser privileges.
nano  | Opens the nano text editor.
cat   | Concatenates and displays the content of files.
chattr| Changes file attributes on a Linux file system.
```

# Netwroks
Commands learnt:
```
ping    | Sends echo requests to test network connectivity.
netstat | Display network connections and stats with IP addresses and Port numbers.
```
   
1. DNS,
     I changed my DNS from the DNS server that is being used by my ISP to public DNS servers provided by Quad9 and Google by editing the IP addresses in the ```/etc/resolv.conf``` file, to improve my security as this stops my ISP from obtaining my Domain Name requests. This is how I did it:
```
   sudo chattr -i /etc/resolv.conf
   sudo nano /etc/resolv.conf
   sudo chattr +i /etc/resolv.conf 
```
This just removes the immutability of the resolv.conf file, then opens the nano text editor for me to change the DNS servers being used, then adds the immutability again.
