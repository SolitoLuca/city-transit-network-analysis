# city-transit-network-analysis
Progetto per corso universitario 2025. Analisi dei dati e teoria dei grafi applicata alle reti di trasporto pubblico di 25 città globali. Sviluppato in Python utilizzando Pandas e NetworkX.

L'obiettivo del progetto è l'analisi strutturale e temporale delle reti di trasporto pubblico di 25 città globali [cite: 54] utilizzando la teoria dei grafi.

## 📝 Descrizione del Progetto
[cite_start]Il software analizza dataset relativi a fermate (nodi) e viaggi (archi) per estrarre statistiche sulla connettività urbana[cite: 20, 21]. [cite_start]L'analisi viene condotta su due livelli temporali: giornaliero (`day`) e settimanale (`week`)[cite: 80].

### Città Analizzate
[cite_start]La lista include 25 metropoli tra cui: Adelaide, Belfast, Berlino, Bordeaux, Brisbane, Canberra, Detroit, Dublino, Grenoble, Helsinki, Kuopio, Lisbona, Lussemburgo, Melbourne, Nantes, Palermo, Parigi, Praga, Rennes, Roma, Sydney, Tolosa, Turku, Venezia e Winnipeg[cite: 54].

## 🛠️ Funzionalità Principali
Il programma risponde a quattro quesiti fondamentali:

1.  [cite_start]**Top 10 Partenze**: Calcola le 10 località con il maggior numero di viaggi in uscita per ogni città e periodo[cite: 6].
2.  [cite_start]**Distribuzione di Grado**: Identifica le 10 località più "connesse" costruendo un grafo non orientato $U(G)$[cite: 18, 19].
3.  [cite_start]**Diametro della Rete**: Calcola esattamente il diametro della componente connessa più grande del grafo indotto[cite: 26].
4.  **Analisi Statistica e Temporale**:
    * [cite_start]Tracciamento del numero di archi nel tempo tramite grafici orari[cite: 34].
    * [cite_start]Conteggio delle località uniche e delle connessioni dirette totali[cite: 39, 45].

## 🧩 Gestione dei Dati e Sfide Tecniche
[cite_start]Durante lo sviluppo sono state implementate soluzioni per risolvere criticità strutturali dei dataset[cite: 7]:
* [cite_start]**ID Compositi**: Creazione di mappature univoche per risolvere il problema di più "stop id" associati alla medesima località fisica[cite: 8, 11].
* [cite_start]**Data Cleaning**: Rimozione automatica dei valori "NaN" derivanti da stop id presenti nei file temporali ma assenti nel file dei nodi[cite: 9, 13].
* [cite_start]**Efficienza**: Rimozione di archi duplicati e self-loops per ottimizzare memoria e tempi di esecuzione[cite: 22].



## 🚀 Requisiti e Installazione
Il progetto richiede Python 3.x e le seguenti librerie:
* `pandas`
* `networkx`
