# servidorDNS
(como no sabia meter las fotos te adjunto el word por si se viera mejor que asi https://github.com/Cax16/servidorDNS/blob/master/RAIDS%20y%20servidor%20DNS.docx )



Raid 0
 https://github.com/Cax16/servidorDNS/blob/master/raid%200.png
Raid 5
 
https://github.com/Cax16/servidorDNS/blob/master/raid%205.png

Servidor DNS
Primero configuramos la interfaz sudo  nano /etc/network/interfaces
https://github.com/Cax16/servidorDNS/blob/master/x%20pic1.png

Podremos ver las tarjetas red del ordenador con el comando “ifconfig –a”
 
https://github.com/Cax16/servidorDNS/blob/master/x%20pic2.png


Lo guardamos, Reiniciamos las tarjetas de red
sudo /etc/init.d/network restart
Le quitamos la almohadilla a net.ipv4.ip_forward=1 

https://github.com/Cax16/servidorDNS/blob/master/x%20pic3.png



Instalamos bind9
Y configuramos los archivos locales 
sudo nano /etc/bind/named.conf.local

https://github.com/Cax16/servidorDNS/blob/master/x%20pic4.png


Accedemos al archivo /etc/bind/rd.sitioa.com “sudo nano /etc/bind/rd.sitioa.com”
 
  https://github.com/Cax16/servidorDNS/blob/master/x%20pic6.png
 
 
Y hacemos lo mismo con el sitiob.net
Accedemos al archivo resolución inversa /etc/bind/ri.192.168.10 
Con “nano etc/bind/ri.192.168.10”

Configuramos en caso de que el servidor no conozca los nombres de dominio le pregunte a otro servidor.

 https://github.com/Cax16/servidorDNS/blob/master/x%20pic7.png

