# Arduino 

## Hardware

Testato con Arduino Uno con una Ethernet Shield. 

I pin usabili sono il 2°, 3°, 4°, 5°, 6°, 7°, 8° e 9°.

## Software

Per installare il codice di Arduino è molto semplice:

1. Importare la libreria "Redis Client", situata in lib/, in Arduino IDE seguendo la documentazione ufficiale dal sito Arduino.

2. Aprire nell'ide il file .ino che si trova nella cartella src/.

3. Nel file .ino modificare le seguenti variabili: ```arduino_mac```, ```arduino_ip```, ```server``` e ```key```. ```key``` è il nome della chiave nel database Redis alla quale arduino cercherà di leggere la stringa.

4. Verificare e uplodare il codice su Arduino.