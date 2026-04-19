# Progetto_MAP
Il progetto presentato è stato sviluppato per il corso di Metodi Avanzati di Programmazione 2024-2025 e ha 
come obiettivo la realizzazione di un sistema client–server per l'esecuzione dell'[algoritmo QT 
(Quality Threshold Clustering)](https://www.ibm.com/it-it/think/topics/unsupervised-learning) su dati memorizzati in un database.
L'architettura è suddivisa in due componenti principali: un client, che invia le richieste e un server,
che gestisce l'accesso al database ed esegue l'algoritmo di clustering.

# Struttura del progetto
Il progetto è stato realizzato in una forma base ed una con estensione:

## 1. Progetto Base
Il progetto base implementa le funzionalità fondamentali del sistema.

Il **Client**, dopo aver indicato i dati necessari per collegarsi al Server, invia al Server una richiesta contenente:
- il nome della tabella da analizzare
- il valore del raggio da utilizzare per l'algoritmo QT

Il **Server** riceve la richiesta del Client e:
- Accede al database fornito dalla docente
- Esegue l'algoritmo Quality Threshold Clustering sulla tabella indicata
- Invia i risultati dei cluster generati al client
- Salva il Clusterset prodotto dall'algoritmo in un file dedicato

## 2. Progetto Esteso
Il progetto con estensione implementa un'interfaccia grafica lato Client, che consente all'utente di inserire i parametri per accedere al server e per eseguire (oltre a visualizzare i risultati) l'algoritmo QT in modo più intuitivo.

# Obiettivo
L'obiettivo del progetto è applicare e consolidare l'utilizzo dei principali costrutti della programmazione orientata agli oggetti, con particolare riferimento al linguaggio Java, supportato dall'uso di SQL per l'accesso e la gestione dei dati. Il progetto mira inoltre all'implementazione di un'architettura client–server basata su socket, alla gestione della comunicazione tra i due componenti e alla separazione delle responsabilità tra interfaccia, logica applicativa ed elaborazione dei dati.
