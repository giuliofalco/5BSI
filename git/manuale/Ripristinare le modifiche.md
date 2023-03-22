Se le modifiche effettuate nel tempo, e salvate attraverso le operazioni di commit, portassero a situazioni non più desiderabili è possibile ripristinare la situazione dei file, esattamente corrispondente al momento in cui è stato salvata con il relativo commit

Il comando è il seguente

	git checkout numero_hash

il numero_hash è qual numero identificativo di un commit, mostrato nell'elenco derivato dall'esecuzione di git log

Se invece si è associato ad un particolare ramo di sviluppo un branch, si potrà utilizzare il nome di quel branch al posto del numero

E' poi possibile ritornare all'ultima situazione ripetendo il comando verso i lbranche corrente.

Oltre a consentire di ripristinare la situazione ad uno stato precedente a modifiche indesiderate, il comando è utile per verificare branch differenti, ricevuto da collaboratori esterni e che non si è ancora deciso di incorporare nella propria storia mediante l'operazione di merge
