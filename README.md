# Comuni-Italiani-2017-Sql-Json-Excel

STRUTTURA DEL DATABASE 
Tutte le tabelle sono corredate di identificativo univoco della riga in modo da poter eseguire query, view, stored procedures e richieste incrociate. 
Nello specifico vengono fornite le colonne riportate qui sotto, per ogni tabella/foglio.  
Si precisa che alcuni dati (esempio numero di abitanti, patroni o coordinate geografiche) potrebbero non essere presenti o non essere aggiornati.  

TABELLA DELLE REGIONI ITALIANE 
id regione nome regione superficie (in mq) 
numero di residenti (valore Istat non sempre aggiornato) 
numero di comuni numero di province presidente codice istat regione codice fiscale piva pec sito web indirizzo sede 

TABELLA DELLE PROVINCE ITALIANE 
id regione nome provincia sigla superficie (in mq) numero di residenti (valore Istat non sempre aggiornato) 
numero di comuni (valore Istat aggiornato) 

TABELLA DELLE CITTÀ METROPOLITANE 
id città denominazione capoluogo popolazione superficie (in mq) densita numero comuni 

TABELLA DEI COMUNI ITALIANI 
cod. istat comune regione sigla provincia prefisso codice fisco superficie 
numero di residenti (valore Istat non sempre aggiornato) 

TABELLA DELLE INFORMAZIONI 
cod. istat comune abitanti nome patrono data patrono 

TABELLA DELLE COORDINATE GEOGRAFICHE 
cod. istat citta latitudine longitudine 

TABELLA DEGLI INDIRIZZI DEI MUNICIPI 
cod. istat comune regione sigla provincia indirizzo 

TABELLA DEI COMUNI RIMOSSI 
cod. istat comune sigla provincia 

TABELLA RIASSETTO ISTAT 2017 SARDEGNA 
cod. istat pre-2017 cod. istat 2017 comune 

TABELLA DEI CAP ITALIANI 
cod. istat cap
