
# I metodi **DID (Difference-in-Differences)** e **PSM (Propensity Score Matching)** 

sono tecniche statistiche utilizzate per valutare l'impatto di un intervento o trattamento, come ad esempio una politica pubblica o un programma di incentivazione, su un gruppo di soggetti (le imprese, in questo caso).

**Propensity Score Matching (PSM)**
*   Il PSM è una tecnica utilizzata per creare un gruppo di controllo che sia il più simile possibile al gruppo trattato in termini di caratteristiche osservabili. L'obiettivo è quello di ridurre il bias di selezione che può verificarsi quando i gruppi trattati e di controllo sono diversi all'inizio dello studio.
*   Il PSM si basa sulla stima della probabilità che un'impresa riceva il trattamento, dato un insieme di caratteristiche osservabili (il "propensity score"). Le imprese trattate vengono quindi abbinate alle imprese non trattate con propensity score simili.
*   Le variabili utilizzate per stimare il propensity score possono includere caratteristiche dell'impresa come la dimensione, il settore di appartenenza, l'area di provenienza, la propensione all'export, la produttività del lavoro, il capitale umano.
*   Esistono diversi metodi di "gemellaggio" all'interno del PSM, come il "nearest neighbor matching", che seleziona le imprese di controllo più simili a quelle trattate.
*   Il PSM è utilizzato per creare un gruppo di controllo che sia un valido controfattuale per il gruppo trattato. Un controfattuale è ciò che sarebbe successo al gruppo trattato se non avesse ricevuto il trattamento.

**Difference-in-Differences (DID)**
*   Il DID è una tecnica utilizzata per stimare l'effetto causale di un trattamento confrontando le variazioni nei risultati nel tempo tra il gruppo trattato e il gruppo di controllo.
*   Il DID si basa sull'assunto che, in assenza del trattamento, i due gruppi avrebbero avuto andamenti simili nel tempo.
*   Il DID viene spesso utilizzato in combinazione con il PSM, in modo da confrontare le variazioni nei risultati nel tempo tra gruppi che sono simili all'inizio dello studio.

**Combinazione PSM e DID**
*   La combinazione di PSM e DID è una tecnica robusta per la valutazione di impatto, poiché il PSM aiuta a ridurre il bias di selezione e il DID aiuta a controllare per i trend temporali.
*   Dopo aver abbinato le imprese trattate con le imprese di controllo tramite PSM, si applica il DID per stimare l'effetto causale del trattamento confrontando le variazioni nei risultati nel tempo tra i due gruppi.
*   Questa combinazione è utilizzata in diversi ambiti, come la valutazione delle politiche pubbliche nel mercato del lavoro, gli effetti dell'internazionalizzazione e le politiche di incentivazione alle imprese.

**Applicazioni specifiche**
*   Queste tecniche sono utilizzate per valutare l'efficacia di politiche di incentivazione alle imprese, come ad esempio gli aiuti per investimenti, per l'internazionalizzazione o per l'innovazione.
*   Possono essere applicate anche per analizzare l'impatto di programmi di politica attiva del lavoro o di politiche per lo sviluppo locale.
*   L'analisi può riguardare diverse variabili di outcome, come l'occupazione, la produttività (TFP), i ricavi, il valore aggiunto, la redditività e la stabilità finanziaria.

**Considerazioni metodologiche**
*   È importante riportare la diagnostica del PSM, come lo Pseudo R2, e i risultati del probit prima e dopo il matching per valutare la qualità del matching.
*   È necessario considerare la possibilità di "effetti di anticipo", cioè se le imprese iniziano a modificare il proprio comportamento prima di ricevere il trattamento.
*   È fondamentale valutare se le imprese che richiedono e ricevono finanziamenti sono simili a quelle che non lo fanno, controllando per le caratteristiche osservabili, e considerare anche le differenze in caratteristiche non osservabili.
*   Bisogna anche tenere conto del fatto che il successo di una politica di aiuto alle imprese può essere multidimensionale e che gli effetti possono manifestarsi in tempi diversi.
*   L'analisi deve considerare anche la possibilità di effetti di spillover, cioè se il trattamento ha effetti anche su imprese che non lo ricevono direttamente.

In sintesi, il **PSM** viene utilizzato per creare un gruppo di controllo comparabile a quello trattato, mentre il **DID** serve a misurare l'impatto del trattamento nel tempo. La combinazione delle due metodologie permette di ottenere stime più affidabili dell'effetto causale delle politiche pubbliche o di altri interventi sulle imprese.
