
In Git, l'operazione `push` viene utilizzata per inviare le modifiche locali a un repository remoto, mentre l'operazione `pull` viene utilizzata per scaricare le modifiche effettuate in un repository remoto sul proprio sistema locale. Ecco come utilizzarle per mantenere il proprio sistema aggiornato rispetto a quello remoto:

## Push:

1. 
Aprire il terminale o la riga di comando nella directory del repository Git.

2. 
Digitare il comando `git add` seguito dal nome del file o dalla directory contenente i file che si desidera aggiungere al commit.

3. 
Digitare il comando `git commit -m` seguito da una descrizione del commit.

4. 
Digitare il comando `git push` seguito dal nome del repository remoto e dal nome del branch locale su cui si stanno lavorando le modifiche. 
Per non generare conflitti con il repository remoto è bene, aver creato un nuovo branch con il proprio nome, ed essere posizionati su quel branch, ad esempio usando il comando

	git checkout -b mio_branch

ora sarà possibile inviare le modifiche etichettate con il priprio branch mediante il comando:

	git push origin mio_branch

5. 
Git chiederà le credenziali per accedere al repository remoto. Inserire le credenziali e premere INVIO.

in questo modo sul repository remoto vi saranno due branch distinti, pronti all'occorrenza, per essere uniti mediante una operazione di merge

## Pull:

L'operazione di pull consente di incorporare nel proprio branch, le modifiche apportate nel branche remoto.

>Se ad esempio il branche remoto, da cui inizialmente si è clonato il proprio sistema, prima di passare al proprio branch si chiamasse main, il comando seguente incorporerà le modifiche remote nel proprio branch

`git pull origin main`.

>NOTA BENE: 
 non utilizzare come nome di branch il proprio. Se si è clonato il sistema partendo da main, e successivamente si è cambiato branch, il proprio risulta essere un 'figlio' di main.
 L'aggiornamento di main, porterà automaticamente gli aggironamenti a propgarsi sul proprio.

Inoltre:
prima di effettuare un'operazione `push` o `pull`, è consigliabile controllare se ci sono conflitti tra i file locali e quelli remoti. In caso contrario, potrebbe essere necessario risolvere i conflitti prima di eseguire l'operazione per evitare di sovrascrivere modifiche importanti.