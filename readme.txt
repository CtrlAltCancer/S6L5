SQLINj-1:
Questa stringa esegue un attacco di SQL injection per ottenere informazioni sulle tabelle presenti nel database utilizzando lo schema di informazioni (information_schema).
SQLINj-2:
Questa stringa esegue un attacco di SQL injection per recuperare informazioni sulle colonne della tabella 'users' utilizzando lo schema di informazioni 
SQLINj-3:
Questa stringa è un attacco di SQL injection per ottenere informazioni sulle tabelle presenti nel database utilizzando lo schema di informazioni (information_schema).
SQLINj-4:
Questa stringa è un tentativo di attacco di SQL injection con l'obiettivo di recuperare informazioni sensibili come i numeri delle carte di credito (ccnumber) e le date di scadenza delle carte di credito (expiration) dalla tabella credit_cards di un database, presumibilmente all'interno di un'applicazione vulnerabile.
SQLINj-5:
Questa stringa è simile allo screenshot precedente, dove l'obiettivo è quello di ottenere informazioni sensibili come il numero della carta di credito (ccnumber) e il codice di verifica della carta di credito (ccv) dalla tabella credit_cards.
SQLINj-6:
La stringa è un'attacco di SQL injection per recuperare le informazioni sugli utenti e le password dalla tabella users di un database, che sono però hashate.
SQLINj-7 e 8:
I comandi eseguito fanno chiamata al programma John the Ripper, un popolare strumento di cracking delle password. Questo comando viene utilizzato per eseguire un attacco di forza bruta o di dizionario (vedi S6_L5.txt) per cercare di recuperare le password da un file hash MD5. In questo caso ha avuto successo.

XSSStored.png:
Lo script imposta la posizione del browser all'URL indicato (http://192.168.50.100:12345/) aggiungendo i cookie dell'utente (document.cookie) alla fine dell'URL come parametro. Il server rimane in ascolto sulla porta 12345. Quando un client si connetterà a questa porta, netcat mostrerà i dati inviati dal client sullo stdout. Rimuove inoltre l'accesso al sito, consegnando un unable to connect.
XSSStored2.png:
Questa stringa esegue un attacco di Cross-Site Scripting (XSS) inserendo uno script JavaScript malevolo all'interno di un input, come un campo di un modulo web. Lo script <script>alert(document.cookie)</script> è progettato per mostrare una finestra di avviso nel browser dell'utente contenente il valore dei cookie del sito web corrente.

