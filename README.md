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
- di Locazione
- di Concorrenza
- di Replicazione
- ai Guasti
- alla Migrazione
- alle Prestazioni
- di Scalabilità
  
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
- Produzione di software
- Complessità
- Sicurezza
- Comunicazione