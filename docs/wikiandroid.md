# Android

## Installazione

Installare la app dal file .apk generato da Gitlab CI o Travis CI.

## Configurazione Wiki

- Inserire indirizzo ip o nome dns di wikicontroller.
- Configurare la casa aggiungendo nome del led, chiave ( stessa data per arduino ) e posizione del pin a cui è collegato.
- Salvare la configurazione.
- ( in caso esista già una configurazione si può scaricare tale configurazione dal controller ).
- ( uplodare nuova configurazione se necessario ).

## Configurazione Wiki AI

- Prima di tutto bisogna installare [wikiserver](wikiserver.md).
- Tenere premuto sul pulsante del microfono.
- Nella dialog che compare inserire l'indirizzo di wikiserver in questo formato: ```<scheme>://<ip_or_dns_name>:<port>/v1/wiki```.
- Per usarla premere semplicemente sul microfono e parlare semplicemente.