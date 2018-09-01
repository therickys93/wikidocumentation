# Wiki Controller

## Hardware

Come Harware è stato usato un semplice Raspberry Pi a 64 bit.

## Software

### Requisiti

- scaricare Raspbian version lite ( senza interfaccia grafica ).
- con Etcher mettere il file .img sulla scheda micro sd.
- riconnettere la scheda sd e inserire nella root il file vuoto ssh ( senza estensione ).
- togliere la scheda ed inserirla nell'apposita slot di raspberry pi.
- collegare cavo di rete e alimentazione a raspberry pi.
- trovare indirizzo ip di raspberry pi dal router.
- connettersi in ssh: username: pi password: raspberry ( possibilita di cambiare la password appena ci si logga ).
- sudo apt update.
- sudo apt upgrade -y.
- sudo raspi-config - Expand File System
                    - Memory Split ( 16 )
                    - Change password ( non necessario ai fini del setup )
                    - Hostname ( non necessario ai fini del setup )
                    - Update
                    - Finish.
- sudo reboot ( se non fatto appena si preme su finish ).
- curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
- sudo apt install redis-server supervisor git nginx nodejs -y
- nella configurazione di Redis modificare i seguenti parametri: bind 0.0.0.0 e protected-mode no.
- sudo service redis-server restart

### Installazione

- clonare il repo
- configurare nginx e supervisor ( i file di esempio si trovano nella cartella config/ ).
- con supervisor avviare il programma.