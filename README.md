# city-transit-network-analysis
Progetto per corso universitario 2025. Analisi dei dati e teoria dei grafi applicata alle reti di trasporto pubblico di 25 città globali. Sviluppato in Python utilizzando Pandas e NetworkX.

L'obiettivo del progetto è l'analisi strutturale e temporale delle reti di trasporto pubblico di 25 città globali utilizzando la teoria dei grafi.

## 📝 Descrizione del Progetto
Il software analizza dataset relativi a fermate (nodi) e viaggi (archi) per estrarre statistiche sulla connettività urbana. L'analisi viene condotta su due livelli temporali: giornaliero (`day`) e settimanale (`week`).

### Città Analizzate
La lista include 25 metropoli tra cui: Adelaide, Belfast, Berlino, Bordeaux, Brisbane, Canberra, Detroit, Dublino, Grenoble, Helsinki, Kuopio, Lisbona, Lussemburgo, Melbourne, Nantes, Palermo, Parigi, Praga, Rennes, Roma, Sydney, Tolosa, Turku, Venezia e Winnipeg.

## 🛠️ Funzionalità Principali
Il programma risponde a quattro quesiti fondamentali:

1.  **Top 10 Partenze**: Calcola le 10 località con il maggior numero di viaggi in uscita per ogni città e periodo.
2.  **Distribuzione di Grado**: Identifica le 10 località più "connesse" costruendo un grafo non orientato $U(G)$.
3.  **Diametro della Rete**: Calcola esattamente il diametro della componente connessa più grande del grafo indotto.
4.  **Analisi Statistica e Temporale**:
    * Tracciamento del numero di archi nel tempo tramite grafici orari.
    * Conteggio delle località uniche e delle connessioni dirette totali.

## 🧩 Gestione dei Dati e Sfide Tecniche
Durante lo sviluppo sono state implementate soluzioni per risolvere criticità strutturali dei dataset:
* **ID Compositi**: Creazione di mappature univoche per risolvere il problema di più "stop id" associati alla medesima località fisica.
* **Data Cleaning**: Rimozione automatica dei valori "NaN" derivanti da stop id presenti nei file temporali ma assenti nel file dei nodi.
* **Efficienza**: Rimozione di archi duplicati e self-loops per ottimizzare memoria e tempi di esecuzione.


## 🚀 Requisiti e Installazione
Il progetto richiede Python 3.x e le seguenti librerie:
* `pandas`
* `networkx`

---
**Contatti:** [Luca Solito](https://linkedin.com/in/tuo-profilo)  
**Università:** Università degli Studi di Firenze - Scuola di Economia e Management
