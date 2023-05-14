# I Sistemi Distribuiti
Sono applicazioniu costituite da <strong>più processi cooperanti</strong>.

## Benefici
#### Affidabilità
Grazie alla sua ridondanza intrinseca un sistema distribuito è in grado di "sopravvivere" a un guasto di un suo componente; è comunque necessario prevenire queste situazioni, per esempio con l'implementazione di algoritmi che permettano alle entità non guaste di "sostituire" quella danneggiata e continuare l'elaborazione.

#### Integrazione
Un sistema distribuito è capace di integrare componenti eterogenei tra loro, sia per <strong>tipologia hardware</strong>, sia per <strong>sistema operativo</strong>.
Ogni componente deve poter interfacciarsi allo stesso modo con il sottosistema di comunicazione del sistema distribuito ed è proprio l'interfaccia che permette di rendere trasparenti i componenti dello strato inferiore del sistema all'intera rete.

#### Trasparenza
Come trasparenza si intende il concetto di vedere il sistema distribuito non come un insieme di componenti ma come un unico sistema di elaborazione: l'utente non deve accorgersi che sta interagendo con un sistema distribuito ma deve avere la percezione di utilizzare un singolo elaboratore, senza percepire eventuali mutamenti che si verificano nel tempo nel sistema.

<strong>Esistono 8 forme di trasparenza</strong>
- di Accesso
Si devono nascondere le differenze nella rappresentazione dei dati e nelle modalità di accesso alle risorse, in modo da permettere di accedere a risorse locali e remote con le stesse operazioni, in modo unico e uniforme

- di Locazione
Si deve nascondere dove è localizzata una risorse e permettere di accedere a essa senza conoscerne la locazione

- di Concorrenza
si permette ai processi di operare in maniera concorrente, cioè facendo in modo che l'accesso concorrente a una risorsa condivisa la lasci sempre in uno stato consistente, implementando per esempio meccanismi di locking

- di Replicazione
le operazioni di duplicazione vengono effettuate all'insaputa degli utenti mantenendo gli stessi nomi per ogni risorsa, in modo da avere copie di risorse che aumentano l'affidabilità e le prestazioni del sistema  

- ai Guasti
viene mascherato il guasto e il recovery di una risorsa

- alla Migrazione
si nasconde l'eventuale spostamento logico o fisico di una risorsa senza interferire sulla sua modalità di accesso, cioè senza influenzare le operazioni degli utenti che la riguardano

- alle Prestazioni
vengono nascoste le operazioni necessarie per riconfigurare il sistema al variare del carico per migliorarne le prestazioni

- di Scalabilità
il sistema viene espanso senta interrompere o modificare il funzionamento
  
#### Economicità
Generalmente i sistemi distribuiti offrono spesso un miglior rapporto prezzo/qualità dei sistemi centralizzati basati su mainframe: una rete di PC connessi ha un prezzo di alcuni ordini di grandezza inferiore rispetto a quello di un mainframe e con le tecnologie odierne la capacità computazionale è paragonabile. Inoltre, come già abbiamo detto, introduce la possibilità di connettere con un costo molto basso i sistemi legacy in modo da non dover abbandonare una tecnologia su cui è stato realizzato un certo investimento e poter convivere con la tecnologia piu recente.

#### Apertura
Con la definizione dei protocolli standard si favorisce l'apertura all'hardware e software di fornitori diversi in modo da avere:
- Interoperabilità
- Portabilità
- Ampliabilità

#### Connettività e collaborazione
Nei sistemi distribuiti la possibilità di condividere risorse hardware e software comporta vantaggi economici. Per esempio è possibile condividere apparecchiature speciali di costo elevato, quali stampanti particolari, plotter, oppure sistemi di storage e di recovery. Lo scambio e la condivisione di informazioni arricchisce ogni utilizzatore: per esempio vengono creati groupware con specifici interessi.

#### Prestazioni e scalabilità
Un sistema distribuito può essere composto semplicemente da due workstation e un file server oppure da una LAN che può contenere anche molti server, migliaia di workstation, molte stampanti ecc. La crescita di un sistema distribuito con l'aggiunta di nuove risorse e, quindi, di nuovi servizi, fornisce a tutti i suoi componenti un miglioramento delle prestazioni e permette di sostenre l'aumento del carico di richieste: questa possibilità prende il nome di scalabilità orizzontale.
Con la scalabilità si superano i problemi visti nel caso di un sistema centralizzato dove spesso alcune risorse condivise sono disponibilit in misura limitata: nei sistemi distribuiti concettualmente non esiste una limitazione nel numero di risorse disponibili, basta che il sistema abbia la "possibilità di espandersi".

## Classificazioni
- Sistemi di calcolo
  - Cluster Computing
  - Grid Computing
- Sistemi informativi
- Sistemi pervasivi

## Svantaggi
#### Produzione di software
I programmatori del "secolo scorso" hanno dovuto modificare il proprio stile di programmazione e aggiornarsi con lo studio dei nuovi linguaggi e dei nuovi strumenti di sviluppo per poter realizzare applicazioni distribuite.

#### Complessità
Proprio per la struttura hardware i sistemi distribuiti sono più complessi di quelli centralizzati: richiedono strumenti per l'interconnessione degli host e tecniche per l'instradamento corretto dei messaggi e dei dati. È anche più complesso valutare le performance di un sistema distribuito piuttosto che di un unico elaboratore.

#### Sicurezza
Con la connessione di più host tra loro si crea la possibilità di accedere a dati e risorse anche a chi non ne ha il diritto: nascono nuove problematiche connesse alla sicurezza che nel caso di sistemi centralizzati erano inesistenti. Infatti, nei vecchi sistemi per lo più bastava proteggere il sistema dall'accesso fisico delle persone ai locali dove erano presenti i dispositivi da proteggere. Oggi l'accesso avviene via etere e via cavo e anche le trasmissioni sono soggette a rischio di intercettazione (sniffing) e quindi richiedono l'applicazione di appositi accorgimenti per tutelare tutti gli utenti e garantire sicurezza e riservatezza nei dati, sia memorizzati sui computer personali, sia trasmetti per transazioni commerciali o semplicemente personali (email).

#### Comunicazione
Il trasferimento a distanza delle informazioni richiede nuove tipologie di sistemi di telecomunicazione, sia cablati sia wireless, e l'aumento esponenziale degli uenti fa si che giornalmente aumenti la richiesta di bande trasmissive, anche per migliorare la qualità del servizio offerto e offrire nuove tipologie di applicazioni sempre più performanti. La difficoltà maggiore sta nel fatto che si è sempre di frone a nuove problematiche delle quali non si ha ben chiaro ne il dominio di definizione ne di risposta del sistema che possono essere molto diverse anche a breve distanza di tempo. A volte l'utilizzo di tecniche sperimentali porta ll'aumento di complessità in modo accidentale anche a causa del fatto che le tecniche di analisi e progettazione sono spesso basate su vecchi metodi di sviluppo di applicazioni monoprocesso, non adeguate alle situazioni di sistema distribuito.