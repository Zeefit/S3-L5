Il cloud rappresenta la connessione a Internet da cui proviene il traffico esterno. Qualsiasi connessione dalla rete pubblica verso la DMZ o verso la rete interna deve passare attraverso il firewall, 
che filtra il traffico per garantire sicurezza.

I server HTTP e SMTP: La DMZ(Demilitarized zone) deve ospitare i server a cui si accede sia dall’ambito interno, sia dall’ambito esterno (Internet)
Il server in questo esempio HTTP e server di posta SMTP. Questi due server per l’hardening della sicurezza fanno parte della DMZ 
altrimenti, sarebbero facilmente accessibili a possibili attacchi diretti alla rete interna
Il server HTT͏P in DMZ è re͏sponsabile per dare con͏tenuti web ͏a utenti esterni o interni. ͏Questo server us͏a proto͏collo HTT͏P per gestire richieste da part͏e degli utenti e rispondere con pagine ͏web richieste,come porta usa quella standard (80)
Il server SMTP nella DMZ gestisce l'invio di e-mail verso l'esterno (Internet) e l'invio tra server di posta elettronica e la sua porta è la (25)

Poi ho messo gli switch nella DMZ: Questo componente deve fare parte della DMZ per poter permettere ai server sopra citati di comunicare tra di loro,
Questo consente di instradare al meglio il traffico locale tra i server nella DMZ senza dover passare per il firewall. Migliora la performance e la gestione delle risorse disponibili
Inoltre, permette l’espandibilità della DMZ, consentendo agli amministratori IT di aggiungere più server senza dover apportare modifiche strutturali alla rete principale
La DMZ ha un IPS (Intrusion Prevention System) l'IPS protegge i server da intrusioni esterne monitorando e bloccando traffico malevolo
Un'importante differenza tra un IDS (Intrusion Detection System) e un IPS (Intrusion Prevention System) è che l'IPS, intervenendo in modo attivo per interrompere il traffico sospetto, ha il difetto di generare falsi positivi e di conseguenza provocare interruzioni o blocchi non giustificati di traffico lecito. L'IDS, pur limitandosi a rilevare e a segnalare le potenziali minacce, senza che interferisca direttamente con il traffico di rete,

Gestione del traffico: Il firewall perimetrale è posizionato tra Internet, la DMZ e la rete interna. Servea a filtra il traffico in entrata e in uscita cosi da garantire che solo le connessioni autorizzate possano essere stabilite.
Esso agisce come la prima linea di difesa contro gli attacchi esterni, limitando l’accesso non autorizzato alla rete.
Il firewall deve far si che il traffico in arrivo da Internet possa accedere direttamente alla rete interna. 
Solo il traffico diretto ai server localizzati nella DMZ può accedere al firewall 

Poi la rete interna possiede un server NAS(Network Attached Storage) attraverso il quale vengono conservati e distribuiti i dati e le altre fonti della compagnia
è isolato dal traffico esterno grazie al firewall e dall'IDS (Intrusion Detection System) che monitora e segnala eventuali intrusioni o attività sospette che potrebbero superare il firewall
e di conseguenza, solo i dispositivi interni possono accedere a tale sorgente

i pc sono collegati trammite uno switch, questa zona della rete è esclusa dalla DMZ e dall’Internet. Infatti la distanza minore all’obiettivo riduce le minaccie di tutte le forme di intrusioni e attacchi.

