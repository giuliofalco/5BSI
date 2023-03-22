Per clonare un repository di Git esistente tramite SSH ad esempio dall'indirizzo IP: 10.0.0.122 e dal percorso /var/www/html/progetto, seguire questi passaggi:

1.  Aprire il terminale o la riga di comando sul computer in cui si desidera clonare il repository.
    
2.  Digitare il comando `cd` seguito dalla directory in cui si desidera clonare il repository. Ad esempio, se si desidera clonare il repository nella directory `progetti`, digitare `cd progetti`.
    
3.  Digitare il comando `git clone` seguito dall'URL del repository. In questo caso, l'URL del repository sarebbe `ssh://nome_utente@10.0.0.122/var/www/html/progetto`. Quindi, il comando completo sarebbe:


```
git clone ssh://nome_utente@10.0.0.122/var/www/html/progetto

```
<ol start="4">
Premere INVIO per eseguire il comando. Git chiederà la password dell'account SSH per accedere al repository. Digitare la password e premere INVIO.
</li>
4. Git clonerà il repository nella directory corrente. Dopo il completamento del processo di clonazione, si potrà lavorare sul repository clonato come si farebbe con qualsiasi altro repository Git.

Nota: è necessario avere un account SSH valido sul server di destinazione per accedere al repository tramite SSH. Inoltre, il server di destinazione deve avere Git installato e configurato per funzionare con SSH.
