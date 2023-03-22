
## Visualizzazione dello stato del repository

Per visualizzare lo stato del repository, puoi utilizzare il comando "git status":

	git status

Questo mostrerà la lista dei file tracciati da Git e le modifiche apportate ad ognuno di essi.
L'elenco dei file modificati e non ancora tracciati saranno mostrati nel primo elenco
Di seguito i nuovi file che non esistevano prima, ma che sono stati introdotti dall'ultimo commit

A questo punto, bisognerà attraverso il comanado add, tracciare nuovamente i file che sono cambiati o i nuovi file e concludere con un nuovo commit

Per visualizzare la sotria dei commit utilizzare il seguente comando

	git log

oppure

	git log --oneline

	git log --oneline --graph

Il comando mostra l'elenco dei commit, iniziando da quello più recente e andando all'indietro nel tempo
Le opzioni mostrate consentono di vedere l'elenco costituito da una sola line, oppure mostrare i diversi rami di sviluppo e le operazioni di merge effettuate

