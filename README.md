# Comuni-Italiani-2017-Sql-Json-Excel

## [STRUTTURA DEL DATABASE](https://github.com/MatteoHenryChinaski/Comuni-Italiani-2017-Sql-Json-excel/blob/master/create-database-comuni-italiani.sql)
Tutte le tabelle sono corredate di identificativo univoco della riga in modo da poter eseguire query, view, stored procedures e richieste incrociate. 
Nello specifico vengono fornite le colonne riportate qui sotto, per ogni tabella/foglio.  
Si precisa che alcuni dati (esempio numero di abitanti, patroni o coordinate geografiche) potrebbero non essere presenti o non essere aggiornati.  

## TABELLA DELLE REGIONI ITALIANE 
- id regione 
- nome regione 
- superficie (in mq) 
- numero di residenti (valore Istat non sempre aggiornato) 
- numero di comuni 
- numero di province 
- presidente 
- codice istat regione 
- codice fiscale 
- piva 
- pec 
- sito web 
- indirizzo sede 

## TABELLA DELLE PROVINCE ITALIANE 
- id regione 
- nome provincia 
- sigla 
- superficie (in mq) 
- numero di residenti (valore Istat non sempre aggiornato) 
- numero di comuni (valore Istat aggiornato) 

## TABELLA DELLE CITTÀ METROPOLITANE 
- id città 
- denominazione 
- capoluogo 
- popolazione 
- superficie (in mq) 
- densita 
- numero comuni 

## TABELLA DEI COMUNI ITALIANI 
- cod. istat 
- comune 
- regione 
- sigla provincia 
- prefisso 
- codice fisco 
- superficie 
- numero di residenti (valore Istat non sempre aggiornato) 

## TABELLA DELLE INFORMAZIONI 
- cod. istat 
- comune 
- abitanti 
- nome patrono 
- data patrono 

## TABELLA DELLE COORDINATE GEOGRAFICHE 
- cod. istat 
- citta 
- latitudine 
- longitudine 

## TABELLA DEGLI INDIRIZZI DEI MUNICIPI 
- cod. istat 
- comune 
- regione 
- sigla provincia 
- indirizzo 

## TABELLA DEI COMUNI RIMOSSI 
- cod. istat 
- comune 
- sigla provincia 

## TABELLA RIASSETTO ISTAT 2017 SARDEGNA 
- cod. istat pre-2017 
- cod. istat 2017 
- comune 

## TABELLA DEI CAP ITALIANI 
- cod. istat 
- cap


## HISTORY VERSIONI
- Ver 4.6 [11 novembre 2017]: Fornita tabella CAP
- Ver 4.5b [15 settembre 2017]: Database completo disponibile anche in formato JSON (.json)
- Ver 4.5 [19 giugno 2017]: Inserito il riassetto dei codici istat Sardegna, corretti alcuni comuni, uniformati i nomi delle colonne
- Ver 4.4 [6 giugno 2017]: Inserita la siglia automobilista della provincia del Sud Sardegna (SU, istituita provvisoriamente il 30 maggio 2017)
- Ver 4.3 [24 aprile 2017]: Inserito il comune di Val Liona (VI) e rimossi i comuni di Grancona e Sam Germano dei Berici
- Ver 4.2 [01 febbraio 2017]: Corretti circa 15 nomi di comuni italiani precedentemente non aggiornati
- Ver 4.1 [22 gennaio 2017]: Riordino delle province della Sardegna; corretti alcuni nomi di comuni
- Ver 4.0 [11 gennaio 2017]: Aggiunti i comuni istituiti il 1° gennaio 2017; aggiunte info alle regioni
- Ver 3.8 [15 novembre 2016]: Sistemate numerose coordinate geografiche
- Ver 3.7 [07 settembre 2016]: Uniformate alcune colonne doppie
- Ver 3.6 [14 luglio 2016]: Rimossi due comuni (Prestine e Ivano-Francena) soppressi a luglio 2016
- Ver 3.5: Aggiornati alcuni comuni italiani modificati in data 16 aprile 2016
- Ver 3.4: Aggiornate alcune informazioni e risolto problema con due comuni isitutit nel 2016
- Ver 3.3: Inseriti i comuni istituiti il 23 febbraio 2016, e rimossi i soppressi
- Ver 3.2: Risolti alcuni problemi su due comuni mancanti
- Ver 3.1: Aggiunte le tabelle delle città metropolitane e delle informazioni; aggiornati i comuni
- Ver 3.0 [8 gennaio 2016]: Aggiornamenti minori e preparazione alla nuova struttura db 2016.
- Ver 2.3: Corretti alcuni comuni italiani modificati nell’anno 2015.
- Ver 2.2: Inseriti alcuni codici fisco mancanti nella tabella delle città.
- Ver 2.1: Aggiornate coordinate geografiche e corretta nomenclatura di alcuni comuni
- Ver 2.0 [16 gennaio 2015]: Prima release con coordinate di geolocalizzazione dei comuni
- Ver 1.0 [10 agosto 2014]: Prima release pubblica
