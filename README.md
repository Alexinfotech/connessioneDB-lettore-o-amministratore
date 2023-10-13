# connessioneDB-lettore-o-amministratore

Sistema di Autenticazione PHP
Questo progetto rappresenta un sistema di autenticazione in PHP, permettendo agli utenti di effettuare il login e, per coloro che sono autorizzati, di accedere come amministratori.

Caratteristiche Principali
Login Base: Gli utenti possono accedere inserendo la loro email e password.
Accesso Amministratore: Gli utenti con i permessi necessari possono accedere come amministratori inserendo una password aggiuntiva.
Dettagli Implementativi
loging.html: Questa è la pagina principale di login. Gli utenti possono inserire le loro credenziali e, se autorizzati, una password addizionale per l'accesso amministrativo.
conn_db.php: Questo script gestisce la connessione al database. Può stabilire una connessione come utente standard o come amministratore, a seconda delle credenziali fornite.
loging.php: Questo script PHP gestisce l'autenticazione. Controlla le credenziali dell'utente e, se valide, reindirizza alla pagina successiva.
tessera_att.html: Una volta effettuato l'accesso, gli utenti vengono reindirizzati a questa pagina, che visualizza le informazioni dell'utente o dell'amministratore.
Funzionamento
Gli utenti inseriscono le credenziali nella pagina loging.html.
Se fornita, la "Password Root" viene utilizzata per tentare un accesso come amministratore.
Il file loging.php verifica le credenziali nel database.
Se l'utente ha i diritti di amministratore, viene stabilita una connessione al database con privilegi elevati.
L'utente viene poi reindirizzato a tessera_att.html, dove vengono mostrate le relative informazioni.
Nota sulla Sicurezza
Questo progetto è stato sviluppato con un focus didattico. Pertanto, per mantenere il codice il più semplice e leggibile possibile, non sono state implementate misure di sicurezza avanzate come l'hashing delle password o la protezione avanzata delle connessioni. Si sottolinea che questo progetto non dovrebbe essere utilizzato in ambienti di produzione senza adeguate modifiche e miglioramenti in termini di sicurezza.
