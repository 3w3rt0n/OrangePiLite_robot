# OrangePiLite_robot
Orange Pi Lite - robot

Processador: H3
Chip WiFi: RTL 8189 FTV

Configuração do Linux:

Ardquivo: /etc/modules
Incluir as linhas:
:: 8189fs
:: gc2035
:: vfe_v4l2

Drivers:
:: modprobe gc2035
:: modprobe vfe_v4l2
:: modprobe 8189fs

Configuração de rede:

Arquivo: /etc/network/interfaces

:: auto wlan0 ou wlan1
:: allow-hotplug wlanX
:: iface wlanX inet dhcp 
:: wpa-ssid "ssid da rede"
:: wpa-psk  "senha da rede"

Obs.:

:: auto lo
:: iface lo inet loopback

Obs.2:

:: service network-manager restart
:: service networking restart

Instalação de bibliotecas para Python:

:: apt-get install python-opencv
:: apt-get install python-flask





