Le repository riportate qui sotto sono disponibi per l'utilizzo a personale, dottorandi, assegnisti e tesisti del gruppo di meccanica applicata.

# Utilizzo delle repository senza modifica

Il metodo più semplice è quello di accedere alla repository, selezionare `<>CODE` e successivamente `Download ZIP`.
Questo approccio è valido per chiunque debba utilizzare il codice già pronto, senza doverci fare modifiche

<details>
<summary>Screenshot Download ZIP</summary>
  
![image](https://github.com/user-attachments/assets/1e333296-05a7-4561-9963-e8f245601aff)

</details>

L'alternativa è quella di copiare il link presente all'interno della sezione `<>CODE`, aprire il terminale, portarsi nella cartella dove scaricare la repository ([qui come fare](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/)) e digitare il comando `git clone URL`

sostituendo a `URL` il link copiato in precedenza.

<details>
<summary>Screenshot Clone URL</summary>
  
![image](https://github.com/user-attachments/assets/754e12e6-4720-448b-8051-6949eb1ee388)

</details>

# Proporre modifiche ad una repository

Per prima cosa, è bene [leggere un tutorial](https://www.w3schools.com/git/default.asp?remote=github) sull'utilizzo di Git e Github.

Ogni persona che voglia contribuire deve creare un [nuovo branch](https://www.w3schools.com/git/git_branch_push_to_remote.asp?remote=github) e eseguire una `push` request.
Dottorandi e personale controlleranno le modifiche e eseguiranno il merge sulla `master` branch.

In maniera molto sintetica:
1. `git clone URL` per clonare la repository. Se si sta già lavorando con quella repository, un `git pull origin` permette di aggiornare il codice da GitHub (nella stessa branch).
2. `git checkout -b NOMEBRANCH` permette di creare e passare ad una nuova branch (se necessario)
3. Eseguo modifiche al codice
4. `git add -a` aggiunge tutte le modifiche al commit
5. `git commit -m "MESSAGGIO"` crea il commit
6. `git push origin NOMEBRANCH` invia la modifica a GitHub

Si consiglia di inviare frequenti commit per tenere traccia delle piccole modifiche.

# Sintesi delle repository attive

| Nome repository (con link) | Contenuto |
| -------------------------- | --------- |
| [Beckhoff](https://github.com/Mechatronics-UniPD/Beckhoff) | File per l'utilizzo di Beckhoff in Matlab |
| [DOI2Bibtex](https://github.com/Mechatronics-UniPD/DOI2Bibtex) | App per estrarre tante bibtex entries da Scopus usando solamente il DOI |
| [MatlabACE](https://github.com/Mechatronics-UniPD/MatlabACE) | Comunicazione Matlab - ACE per il controllo di robot a 6 o 4 assi |
| [Report-A_LaTeX_Template](https://github.com/Mechatronics-UniPD/Report-A_LaTeX_Template) | Una classe LaTeX per i report |
| [Utilities](https://github.com/Mechatronics-UniPD/Utilities) | File vari utili: **bibtex2bibitem**, **clearPotente**, **DAQ_accelerometer_MONO**, **listaDependenciesFile**, **tgprintf**, **traj_pp** |
