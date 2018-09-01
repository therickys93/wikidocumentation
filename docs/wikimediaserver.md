# Wiki Media Server

## Harware

Testato su un pc a 32 bit. Richiesta di un hard disk da molti GB per il salvataggio di film immagini etc...

## Software

- installare ubuntu server.
- ```curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -```.
- ```sudo apt install supervisor git nginx nodejs -y```.
- clonare il repo wikimediaserver.
- configurare il tutto.
- installare inoltre un server ftp che punti alla cartella mediaserver in modo tale da caricare direttamente li i file.