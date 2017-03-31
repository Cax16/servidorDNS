# servidorDNS
Raid 0
 
Raid 5
 


Servidor DNS
Primero configuramos la interfaz sudo  nano /etc/network/interfaces
 


Podremos ver las tarjetas red del ordenador con el comando “ifconfig –a”
 


Lo guardamos, Reiniciamos las tarjetas de red
sudo /etc/init.d/network restart
Le quitamos la almohadilla a net.ipv4.ip_forward=1 







Instalamos bind9
Y configuramos los archivos locales 




sudo nano /etc/bind/named.conf.local



 










Accedemos al archivo /etc/bind/rd.sitioa.com “sudo nano /etc/bind/rd.sitioa.com”
 
Y hacemos lo mismo con el sitiob.net
Accedemos al archivo resolución inversa /etc/bind/ri.192.168.10 
Con “nano etc/bind/ri.192.168.10”
  


Configuramos en caso de que el servidor no conozca los nombres de dominio le pregunte a otro servidor.

 

