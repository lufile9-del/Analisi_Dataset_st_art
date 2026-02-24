# **Analisi dei Dati Storico-Artistici**:  *Arte come specchio di vita*


## Descrizione
Questo progetto consiste in un'analisi esplorativa ed esplicativa di un dataset contenente dati storico-artistici, relativi ad opere d'arte localizzate in Italia. Esso compre un periodo cronologico molto vasto: dall'XI sec. al XXI.


L'analisi si focalizza sulle modalità di evoluzione dei diversi generi artistici nel periodo considerato, in particolare partendo dalla distinzione tra "arte religiosa" ed "arte laica", evidenziando altresì la correlazione con gli inevitabili mutamenti culturali della civiltà occidentale.

In tal senso è stata svolta anche un'analisi comparativa tra la produzione femminile e maschile di opere d'arte, evidenzianone le differenze soprattutto in termini di generi artistici.


## Quali sono i risultati?
I risultati principali dell'analisi computazionale (contenuti nel Jupyter Notebook) includono:

- La verifica di una crescita della produzione dell'arte laica a partire dal 1700, a discapito dell'arte religiosa;
- L'attestazione di una produzione di arte laica ed imparticolare di ritratti tra le opere delle pittrici considerate;
- L'evidenza di una maggiore produzione di arte religiosa e diversificazione dei generi artistici da parte degli artisti maschi;

## Fonte dei dati
I dati in input sono costituiti da un file CSV contenente informazioni dettagliate su opere d'arte visiva collocate in Italia. Le variabili considerate sono:

| Variabile | Tipo |	Definizione | Esempio |
| :------- | :--- | :--------- | :------ |
| id       |	object | ID degli artisti | 	408 |
| titolo | object | Titolo originario dell'opera | Betsabea |
| artisti |	object |	Nome dell'artista |	Artemisia Gentileschi |
| data_creazione |	object | Data realizzazione opera |	1610 |
| generi | object | Tematiche raffigurate |	Arte religiosa |
| luoghi |	object | luogo fisico di conservazione dell'opera | Palazzo Medici Riccardi; Galleria delle Pitture |
| collezioni |	object | collezione in cui è si trova l'opera |	Galleria degli Uffizi |
| contenuti | object | Elementi presenti nelle opere, ognuno dei quali è separato da ; |	libro; carta; scrittura; strabismo; posizione |
| movimenti | object | Corrente artistica in cui rientra l'opera| Alto Rinascimento |
| soggetti | object | Soggetti del quadro | Tommaso Inghirami |
| altezza | float64 | Altezza del quadro | 91.0 |
| larghezza |	float64 |	Larghezza del quadro| 61.0 |

I dati originali sono stati estratti da Wikidata e sono stati recuperati dalla repository GitHub di sbrzt come file CSV.

Link al dataset: https://raw.githubusercontent.com/dhdmch/2025-2026/refs/heads/main/data/vapod/data.csv


## Metodi e strumenti
Il progetto è stato sviluppato in un ambiente Google Colab utilizzando il linguaggio di programmazione Python. Lo strumento principale utilizzato per la manipolazione, l'analisi e la visualizzazione dei dati è la libreria Pandas.

Le operazioni includono:

- Caricamento e ispezione dei dati (_pd.read_csv_, _df.info()_, _df.describe()_);
- Bonifica e normalizzazione dei dati (conversione delle date_creazioe in tipo int64, pulizia della colonna artisti e realizzazione di una nuova generi_artisti);
- Analisi esplorativa tramite aggregazioni (_value_counts()_, _groupby()_) e visualizzazioni tramite grafici a linea (_plot.line()_), a linee (_plot.line()_) e a dispersione (*plot.scatter()*)
- Analisi esplicativa focalizzata sulla produzione diversificata di opere a carattere laico da parte di pittori e pittrici, per evidenziare la stigmatizzazione del mestiere di pittrici, ma allo stesso tempo la sua graduale riduzione.

## Responsabili
- Miraglia, Luisa - [https://orcid.org/0009-0001-3877-7777](https://orcid.org/0009-0001-3877-7777)

## Licenza
I dati di input e il codice di output (incluso in questo Notebook) sono rilasciati sotto licenza [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).
