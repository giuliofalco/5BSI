Il comando `stash` in Git viene utilizzato per salvare temporaneamente le modifiche locali che non sono ancora state committate, consentendo all'utente di passare a un altro branch o a un'altra attività senza perdere le modifiche effettuate. Ecco come utilizzarlo:

1.  Aprire il terminale o la riga di comando nella directory del repository Git.
    
2.  Digitare il comando `git stash` per salvare le modifiche locali.
    
3.  Se si desidera includere un messaggio descrittivo per le modifiche salvate, digitare il comando `git stash save "Messaggio del commit"`.
    
4.  Git salverà le modifiche locali in una memoria temporanea chiamata "stash". Si può eseguire qualsiasi altra operazione desiderata, come cambiare branch o eseguire un'operazione pull, senza perdere le modifiche salvate.
    
5.  Per ripristinare le modifiche salvate in precedenza, digitare il comando `git stash apply`. Questo ripristinerà l'ultima "stash" creata. Se si desidera applicare una "stash" precedente, è possibile utilizzare il comando `git stash apply stash@{n}`, dove "n" è l'indice della "stash" da applicare.
    
6.  Se si desidera eliminare completamente la "stash", digitare il comando `git stash drop`. Se si desidera applicare e eliminare la "stash" in un solo comando, è possibile utilizzare il comando `git stash pop`.
    
7.  Dopo aver applicato la "stash", si potrebbe essere in grado di committare le modifiche o salvare ulteriori modifiche nella "stash" se necessario.
    

>Nota: il comando `stash` salva solo le modifiche locali e non le modifiche già committate. Inoltre, le modifiche salvate nella "stash" non vengono salvate nel repository fino a quando non vengono committate.

Se si sono effettuate diverso operazioni di salvataggio mediante il comando stash + possibile elencare tutti i salvataggi mediante il seguente comando:

	git stash list
 
 un esempio di output potrebbe essere il seguente:
 
	stash@{0}: WIP on feature-branch: 3c34a15 Added new feature
	stash@{1}: WIP on master: 86e6597 Fixed bug in login form

per ripristinare i cambiamenti salvati nella seconda stash si dovrebbe eseguire il seguente comando

	git stash apply stash@{1}

