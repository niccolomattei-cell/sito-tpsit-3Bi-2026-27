# Esempi guidati del modulo M2 — HTML

Questa cartella contiene il codice che il docente scrive insieme alla classe nella seconda parte di ogni
lezione. I file sono numerati nell'ordine in cui compaiono nella dispensa. Tutti gli esempi costruiscono lo
stesso sito, quello del laboratorio di informatica dell'istituto: è il modello su cui ciascuno studente
realizza, in autonomia, il proprio sito sull'argomento scelto nella prima lezione.

## Come si aprono

Le pagine sono documenti completi e non richiedono né un server né la rete. Si aprono in due modi. Con un
doppio clic sul file `.html` in Esplora file, che lo apre nel browser predefinito. Oppure da Visual Studio
Code, con il clic destro sul file nell'esplora risorse e la voce *Apri con Live Server*, se l'estensione è
installata, o semplicemente *Rivela nell'Esplora file* seguito dal doppio clic.

I due esempi della terza lezione, `04_TabellaOrario.html` e `05_ModuloPrenotazione.html`, sono
volutamente pagine isolate, senza testata e senza menu: servono a costruire un solo elemento per volta
senza il contorno che si ripete. Entrano nel sito nella quarta lezione, come `orario.html` e
`prenotazione.html` di `06_SitoSemantico`. Gli studenti, invece, aggiungono fin da subito le pagine
corrispondenti al proprio sito e al proprio menu di navigazione, come chiedono gli esercizi 7 e 8: il
confronto fra le due scelte è un punto da dichiarare a voce.

Per le cartelle `03_SitoLaboratorio` e `06_SitoSemantico` va aperto `index.html`: le altre pagine si
raggiungono dai collegamenti. Le due cartelle vanno copiate intere, perché contengono la sottocartella
`immagini`: spostando un solo file HTML i collegamenti alle immagini si rompono.

## Elenco dei file

| File | Lezione | Contenuto |
|---|---|---|
| `01_PrimaPagina.html` | 1 | Documento minimo completo: dichiarazione del tipo di documento, radice con la lingua, intestazione con codifica e titolo, corpo con un titolo e due paragrafi |
| `02_TestoStrutturato.html` | 1 | Marcatura del testo: i livelli di titolo come indice, paragrafi, `strong` ed `em`, interruzione di riga, caratteri speciali e spazio insecabile |
| `03_SitoLaboratorio/` | 2 | Prima versione del sito, due pagine collegate fra loro, con menu di navigazione, immagini con testo alternativo, elenchi ordinati, non ordinati e di definizione, collegamenti interni alla pagina |
| `03_SitoLaboratorio/index.html` | 2 | Pagina principale: presentazione, collegamenti alla seconda pagina, a un sito esterno e a un indirizzo di posta |
| `03_SitoLaboratorio/attrezzature.html` | 2 | Seconda pagina: elenchi dei tre tipi, immagine con testo alternativo descrittivo, collegamenti ai punti interni della pagina |
| `03_SitoLaboratorio/immagini/` | 2 | Le due immagini del sito, in formato SVG |
| `04_TabellaOrario.html` | 3 | Tabella dell'orario di occupazione: `caption`, `thead`, `tbody`, `tfoot`, intestazioni con `scope`, `colspan` |
| `05_ModuloPrenotazione.html` | 3 | Modulo di inserimento dati: `fieldset` e `legend`, campi di testo, posta, data, numero, pulsanti di scelta, casella da spuntare, elenco a discesa, area di testo, etichette collegate con `for` |
| `06_SitoSemantico/` | 4 | Versione finale del sito, quattro pagine, riscritta con gli elementi semantici e sottoposta al validatore |
| `06_SitoSemantico/index.html` | 4 | Pagina principale con `header`, `nav`, `main`, due `section`, due `article` negli avvisi, `aside` e `footer` |
| `06_SitoSemantico/attrezzature.html` | 4 | Gli elenchi della lezione 2 riorganizzati in `section` con identificatore |
| `06_SitoSemantico/orario.html` | 4 | La tabella della lezione 3 inserita nel sito |
| `06_SitoSemantico/prenotazione.html` | 4 | Il modulo della lezione 3 inserito nel sito |

## Vincoli rispettati da tutti gli esempi

Nessuna pagina contiene CSS in alcuna forma: non c'è l'attributo `style`, non c'è l'elemento `style`
nell'intestazione, non c'è alcun collegamento a un foglio di stile e non compaiono attributi di
presentazione obsoleti come `bgcolor` e `align`. Le pagine sono volutamente prive di aspetto grafico: è la
scelta didattica illustrata nella dispensa, e in questo modulo non va aggirata.

Nessuna pagina contiene JavaScript. Il modulo di inserimento dati è costruito ma non inviato: l'elemento
`form` non ha l'attributo `action` e non esiste alcun gestore di evento.

Nessun esempio richiede accesso alla rete. Gli unici indirizzi esterni presenti sono due collegamenti
testuali, al sito del W3C e al validatore, che servono come esempio di percorso assoluto: se la rete non è
disponibile la pagina si apre e funziona lo stesso, soltanto quei due collegamenti non portano da nessuna
parte.

## Le immagini

Le immagini sono in formato **SVG**, cioè grafica vettoriale descritta in un file di testo. La scelta ha
due motivi. Il primo è pratico: un file SVG si apre in Visual Studio Code e se ne legge il contenuto, che è
marcatura fatta di rettangoli, tracciati e coordinate; è un buon modo per far vedere che la marcatura non
riguarda solo i documenti. Il secondo è che un'immagine vettoriale resta nitida a qualunque ingrandimento e
pesa pochi kilobyte.

Il logo, `logo-laboratorio.svg`, compare nella testata di ogni pagina con `alt=""`, perché è decorativo: il
nome del laboratorio è già scritto in chiaro accanto, e farlo leggere due volte a chi usa un lettore di
schermo sarebbe un disturbo. La pianta dell'aula, `pianta-laboratorio.svg`, ha invece un testo alternativo
lungo e descrittivo, perché porta un'informazione che non è scritta da nessun'altra parte. Il confronto fra
i due casi è il punto della lezione sulle immagini.

## Che cosa succede a questo codice dopo il modulo M2

La cartella `06_SitoSemantico` è la versione che il modulo M3 riprende per applicarvi un foglio di stile
esterno, senza riscrivere l'HTML. In M4 la disposizione degli elementi verrà rifatta con Flexbox, in M5 il
sito sarà ricostruito con Bootstrap, in M7 il modulo di prenotazione comincerà a reagire alle azioni
dell'utente e in M8 i dati arriveranno da un servizio remoto. Il codice di questo modulo non si butta: si
amplia.

## Verifica delle pagine

Ogni pagina di questa cartella è stata sottoposta al validatore del W3C e non produce errori. Per
ripetere il controllo si apre `https://validator.w3.org/`, si sceglie la scheda *Validate by File Upload*
e si carica il file. Se la rete non è disponibile si usa, in Visual Studio Code, l'estensione **HTMLHint**,
che segnala nel pannello *Problemi* i tag non chiusi e gli identificatori duplicati. Il controllo sul testo
alternativo delle immagini non è attivo per impostazione predefinita: va abilitato con un file
`.htmlhintrc` nella radice del repository contenente
`{"alt-require": true, "input-requires-label": true}`.

Una sola pagina del modulo non supera la validazione, ed è voluto: è il file
`04_Allegato_PaginaDifettosa.html`, che sta nella cartella del modulo e non qui, e che contiene gli errori
che gli studenti devono trovare e correggere nell'esercizio 10.
