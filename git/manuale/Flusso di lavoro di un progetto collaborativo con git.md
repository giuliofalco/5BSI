## Flusso di lavoro di una esercitazione didattica

Un possibile flusso di lavoro e schema organizzativo per la conduzione di un progetto didattico, collaborato utilizzando git potrebbe prevedere i seguenti passi:

 1. ==Definizione degli obiettivi del progetto==
     coinvoglimento degli studenti nell'analisi dei requisti e funzionale
2. ==Fase operativa== 
    gli studenti si suddividono in gruppi di lavoro, e nominamo un referente del gruppo. (preferibilmente max tre componenti per ogni gruppo)
3. ==Lezione introduttiva su git==
    a cosa serve come puà essere utilizzato. Lezione frontale con uso di slides
4. ==impostazione del progetto==
    Il docente condividendo mediante schermo o lim, imposta il progetto creando una cartella sul server della LAN, prepara gli account e le credenziali per il collegamento per ogni referente del gruppo. Inizializza il repository remoto sul server
5. ==lezione sui comandi de terminale==
    Invita ciascun gruppo a inizializzare per la prima volta git, e fornisce i comandi essensiali da terminale per:
  - muoversi fra le directory (cd cartella, cd ..)
  - visualizzare il contenuto di una cartella (ls -l)
  - rimuovere un file o una intera directory (rm nome_file, rm -rf directory)
6. ==clone del sistema remoto==
    Invita ad eseguire il comando clone, per clonare il sistema sul proprio computer locale
   esempio:
   
	   git clone ssh://nome:utente@10.0.0.122/var/www/html/progetto

7. ==creazione di un proprio branch ==
    Invita gli studenti a creare un proprio branch e a renderlo attivo

	   git checkout -b nome_branch
 --------------------------------------------------------------------
### Studenti al lavoro

  Si invitano a questo punto gli studenti, a scegliere una delle sottocartelle del progetto e a occuparsi delle modifiche rispetto agli elementi temporanei inseriti dal docente

Ad esempio nel caso di un sito web, si potrebbe inizialmente invitarli a creare una home page del sito e a sostituirla al prototipo fornito dal docente.
**Nelle fasi successive, di potranno suddividere gli interventi assegnando ai gruppi parti differenti del progetto.**

Si chiede durante ciascuna sessione di lavoro, prima della chiusura di effettuare le operazioni di

		git add "file da tracciare"
		git commit -m "commento"
		
Al termine di ciascuna fase, fissata una scadenza si raccoglono i contributi invitando gli studenti ad eseguire una operazioni di push utilizzando il proprio branch

	git push origin nome_branch

-------------------------------------------
### Il docente valuta i contributi

mediante il comando 

	 git branch
	 
il docente sarà in grado di vedere l'elenco dei branch che si sono uniti al progetto, e mediante il comando

	git checkout nome_branch

valutare il risultato insieme alla classe
potrò scegliere uno dei contributi o effettuare lui stesso un mix

Aggiornerà quindi il sistema effettuando un merge dal proprio branch principale

	git checkout main
	git merge nome_branch

Nel caso risolverà i conflitti, se invece tutto è andato a buon fine, inviterà i ragazzi ad aggiornar e proprio sistema locale con il comando

	git pull origin main

A questo puntoi il ciclo ricomincia


