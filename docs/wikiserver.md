# Wiki Server

## Hardware

Qualsiasi macchina va bene. Testato su un pc 32 bit. Ma dovrebbe funzionare benissimo anche su Raspberry PI.

## Software

- installare ubuntu server o raspbian
- ```sudo apt-get update```
- ```sudo apt-get upgrade -y```
- ```sudo apt-get install nginx supervisor -y```
- ```sudo apt-get install postgresql postgresql-contrib -y```
- clonare il repo wikidatabase
- ```sudo -i -u postgres```
- ```psql < wiki.sql```
- ```psql -d wiki``` ( controllare che il comando precedente sia andato a buon fine )
- ```exit```
- ```sudo add-apt-repository -y ppa:webupd8team/java```
- ```sudo apt-get update```.
- ```sudo apt-get install -y oracle-java8-installer``` ( seguire l installazione perchè chiederà alcune informazioni )
- clonare il repo wikiserver.
- ```./gradlew clean stage```.
- configurare nginx e supervisor.

## Comandi per interagire:

La prima parola corrispondente a una di quelle sotto elencate viene usata a meno di comandi complessi.

- ```ciao``` -> saluta semplicemente.
-  ```data``` -> dice la data di oggi.
- ```ore``` o ```ora``` -> dice l'ora attuale.
- ```grazie``` -> risponde prego.
- ```conferma comando``` --> risponde comando confermato.
- ```cerca <argomento>``` --> cerca l'argomento su Wikipedia.
- ```calcola <argomento>``` --> esegue i calcoli che segueno (es. calcola 5 + 4).
- ```meteo``` --> dice il meteo attuale.
- ```db``` --> chiede lo stato del database (comando di debug).
- ```aggiungi <nome> in <chiave> alla presa <numero>``` --> aggiunge l'accessorio che si chiama nome nel database con la chiave e al numero.
- ```rimuovi <nome>``` --> rimuove l'accessorio che si chiama nome.
- ```accendi <nome>``` --> accende l'accessorio che si chiama nome.
- ```spegni <nome>``` --> spegne l'accessorio che si chiama nome.
- ```come stai``` --> risponde bene grazie.
- ```come ti chiami``` --> risponde il mio nome è Wiki.
- ```connessioni``` o ```collegamenti``` --> dice quali sono gli accessori collegati.
- ```stato <nome>``` --> dice lo stato dell'accessorio che si chiama nome.
- ```apri <nome>``` -> apre l'accessorio che si chiama nome.
- ```chiudi <nome>``` --> chiude l'accessorio che si chiama nome.