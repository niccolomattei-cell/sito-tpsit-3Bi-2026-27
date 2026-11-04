# Colonne sonore al cinema

Sito che raccoglie e presenta le colonne sonore di dieci film, con la scheda di ogni
compositore e l'elenco dei brani principali. È il progetto personale di Laboratorio di TPSIT
della classe 3Bi, costruito lungo tutto l'anno scolastico 2026-2027.

## Che cos'è

Il repository contiene il materiale di un sito che cresce a ogni modulo del corso. Nella sua
forma finale mostra una pagina per ciascuno dei dieci film scelti, con il titolo, l'anno, il
nome del compositore e i brani più noti della colonna sonora. I dati sono raccolti a mano da
schede e da recensioni pubblicate; le fonti sono indicate in fondo a questo documento.

Il progetto nasce come esercitazione didattica: non ha alcuna pretesa di completezza e non è
un catalogo di riferimento.

## Come si consulta

Le pagine del sito non sono ancora state scritte: per ora il repository contiene gli appunti delle
lezioni e le schede dei film raccolte finora, che si leggono aprendo i file della cartella
`appunti` e della cartella `dati` direttamente su GitHub.

Quando le pagine saranno pronte, il sito verrà pubblicato con GitHub Pages all'indirizzo

`https://mbianchi-marconi.github.io/tpsit-3bi-bianchi/`

e basterà aprire quell'indirizzo in un browser; in alternativa si apriranno dalla propria copia del
repository, con un doppio clic sul file `index.html` della cartella `sito`.

## Come si lavora sulla propria copia

Sulla postazione del laboratorio, dopo aver aperto il prompt dei comandi:

```bash
git clone https://github.com/mbianchi-marconi/tpsit-3bi-bianchi.git
cd tpsit-3bi-bianchi
code .
```

L'ultimo comando apre la cartella in Visual Studio Code. Non serve installare nulla: il sito è
fatto di file che il browser apre direttamente, senza alcun programma da avviare.

In alternativa si può lavorare in un Codespace creato dal pulsante verde della pagina del
repository su GitHub, ricordando di spegnerlo a fine lezione per non consumare quota.

## Come è organizzato

| Cartella o file | Contenuto |
|---|---|
| `sito/` | le pagine del sito e i file che le accompagnano, ancora da scrivere |
| `appunti/` | gli appunti delle lezioni, in Markdown |
| `dati/` | le schede dei film, raccolte prima di scrivere le pagine |
| `README.md` | questo documento |

## Strumenti usati

Git per il controllo di versione, GitHub per la pubblicazione, Visual Studio Code come editor.
Le pagine sono scritte a mano, senza generatori automatici e senza librerie di terze parti.

## Stato del lavoro

- [x] repository creato e collegato a GitHub
- [x] scelta dell'argomento e raccolta delle schede dei primi cinque film
- [x] file di descrizione del progetto
- [ ] pagine del sito
- [ ] pubblicazione con GitHub Pages

## Autrice e contesto

Marta Bianchi, classe 3Bi, Istituto Tecnico Tecnologico "G. Marconi" di Rovereto.
Lavoro svolto per il corso di Laboratorio di TPSIT, anno scolastico 2026-2027,
docente Andrea Trentini.

## Fonti dei dati

Le informazioni su anni, compositori e titoli dei brani provengono dalle schede dei film
pubblicate sui siti delle case di distribuzione e dai libretti dei dischi posseduti
dall'autrice. Le copertine dei dischi non sono riprodotte nel sito, perché sono materiale
protetto da diritto d'autore.
