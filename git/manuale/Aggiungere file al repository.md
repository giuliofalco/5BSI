
Dopo aver inizializzato il repository, devi indicare a Git quali file devono essere tracciati. Puoi farlo con il comando "git add":

	git add nome_file

Questo aggiungerà il file specificato alla lista dei file tracciati da Git. Puoi anche aggiungere tutti i file presenti nella cartella corrente con il comando "git add ."

Nota: ad ogni cambiamneto o aggiornamento dei file nel proprio progetto, occorre lanciare il comando precedente per tutti i file che si desidera tracciare.
Non basta averlo fatto la prima volta.

Per sapere quali files sono cambiati rispetto all'ultima situazione stabile, basta lanciare il seguente comando:

	git status

verrà fornito un elenco dei file modificati colorati in rosso e in basso dei nuovi file inseriti per la prima volta.
Non è obbligatorio tracciare tutt i file, i file non tracciati non saranno sottoposti alla memorizzazione dei cambiamenti.

L'esecuzione del comando inserirà i file coinvolti in area chaimata di STAGE
Il contenuto di quest'area è pronto per la successiva operazione di "commit"

rieseguendo di nuovo il comando i file inseriti nella'rea di stage saranno colorati in verde