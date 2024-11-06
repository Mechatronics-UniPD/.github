Le repository riportate qui sotto sono disponibi per l'utilizzo a personale, dottorandi, assegnisti e tesisti del gruppo di meccanica applicata.

# Utilizzo delle repository senza modifica

Il metodo più semplice è quello di accedere alla repository, selezionare `<>CODE` e successivamente `Download ZIP`.
Questo approccio è valido per chiunque debba utilizzare il codice già pronto, senza doverci fare modifiche

<details>
<summary>Screenshot Download ZIP</summary>
  
![image](https://github.com/user-attachments/assets/1e333296-05a7-4561-9963-e8f245601aff)

</details>

In alternativa, è necessario installare Git sul proprio PC: basta aprire PowerShell e digitare il comando `winget install --id Git.Git -e --source winget`.

Dopodiché basta di copiare il link presente all'interno della sezione `<>CODE`, aprire il terminale, portarsi nella cartella dove scaricare la repository ([qui come fare](https://www.howtogeek.com/659411/how-to-change-directories-in-command-prompt-on-windows-10/)) e digitare il comando `git clone URL`

sostituendo a `URL` il link copiato in precedenza.

<details>
<summary>Screenshot Clone URL</summary>
  
![image](https://github.com/user-attachments/assets/754e12e6-4720-448b-8051-6949eb1ee388)

</details>

Nel caso alcune classi dipendano da altre classi (es: KINpro contiene dis e trans) è necessario aggiungere due comandi dopo aver clonato la repository:
1. `git submodule init`
2. `git submodule update`

In questo modo nella vostra cartella troverete anche le sottoclassi aggiornate.

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

# Aggiungere una repository

È possibile aggiungere tutte le repository che potrebbero tornare utili agli altri.
Si raccomanda di:
- Impostare la repository come `privata` e aggiungere il team Personale alla repository andando sotto `Settings > Collaborators and teams > Add teams > Mechatronics-UniPD/personale > Maintain`
- Compilare in maniera esaustiva il file README.md generato in ogni repository
- Aggiungere la repository alla lista presente qui sotto

# Sintesi delle repository attive

| Nome repository (con link) | Contenuto |
| -------------------------- | --------- |
| [Beckhoff](https://github.com/Mechatronics-UniPD/Beckhoff) | File per l'utilizzo di Beckhoff in Matlab |
| [Classe-dis](https://github.com/Mechatronics-UniPD/Classe-dis) | Classe Matlab per il disegno di oggetti |
| [Classe-KINpro](https://github.com/Mechatronics-UniPD/Classe-KINpro) | Classe Matlab per la simulazione robot |
| [Classe-STL](https://github.com/Mechatronics-UniPD/Classe-STL) | Classe Matlab per la gestione dei file STL (comprese sezioni) |
| [Classe-trans](https://github.com/Mechatronics-UniPD/Classe-trans) | Classe Matlab per le trasformazioni di coordinate (compreso Denavit-Hartenberg) |
| [Classe-TSP](https://github.com/Mechatronics-UniPD/Classe-TSP) | Classe Matlab che gestisce il Travelling Salesman Problem (TSP) |
| [DOI2Bibtex](https://github.com/Mechatronics-UniPD/DOI2Bibtex) | App per estrarre tante bibtex entries da Scopus usando solamente il DOI |
| [Manim-PPTdaSezioni](https://github.com/Mechatronics-UniPD/Manim-PPTdaSezioni) | Se si ha un codice [manim](https://docs.manim.community/en/stable/index.html) composto da sezioni, è possibile crearne un PPT |
| [Matlab-ACE](https://github.com/Mechatronics-UniPD/MatlabACE) | Comunicazione Matlab - ACE per il controllo di robot a 6 o 4 assi |
| [Matlab-AppSTL](https://github.com/Mechatronics-UniPD/Matlab-AppSTL) | App Matlab per la modifica degli STL |
| [Matlab-CreareVideodaSimulazione](https://github.com/Mechatronics-UniPD/Matlab-CreareVideodaSimulazione) | Codice per creare un video partendo da una simulazione Matlab (utile soprattutto per simulazione meccanismi e movimenti) |
| [Matlab-Mouse3D](https://github.com/Mechatronics-UniPD/Matlab-Mouse3D) | Codice per utilizzare il mouse 3D [3Dconnexion Space Compact](https://3dconnexion.com/it/product/spacemouse-compact/)|
| [Report-A_LaTeX_Template](https://github.com/Mechatronics-UniPD/Report-A_LaTeX_Template) | Una classe LaTeX per i report |
| [Utilities](https://github.com/Mechatronics-UniPD/Utilities) | File vari utili: **bibtex2bibitem**, **clearPotente**, **DAQ_accelerometer_MONO**, **listaDependenciesFile**, **tgprintf**, **traj_pp** |
