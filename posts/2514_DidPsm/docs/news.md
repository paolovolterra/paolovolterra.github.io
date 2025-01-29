# Oltre DID e PSM

Ci sono diverse tecniche più moderne rispetto al Difference-in-Differences (DiD) e al Propensity Score Matching (PSM), che sfruttano i progressi nell'analisi dei dati, il machine learning e la causal inference. 

Queste tecniche sono particolarmente utili se:
- Hai dataset complessi, con molte covariate o relazioni non lineari
- Vuoi stime robuste agli errori modellistici
- Devi gestire trattamenti eterogenei o bias di selezione complessi


### **1. Synthetic Control Method (SCM)**
Il metodo del controllo sintetico crea un "gruppo di controllo sintetico" combinando una serie di unità non trattate che approssimano le caratteristiche del gruppo trattato. Questo approccio è particolarmente utile quando c'è solo un'unità trattata (es., una singola azienda o paese).

- **Vantaggi**:
  - Permette analisi causali robuste in contesti con una sola unità trattata.
  - Minimizza il bias di selezione.

- **Libreria Python**: 
  - [`synthdid`](https://github.com/synth-inference/synthdid) o implementazioni in R.

### **2. Double Machine Learning (DML)**
Il DML combina tecniche di machine learning (come alberi decisionali, reti neurali o boosting) con stima degli effetti causali. È utile per affrontare problemi di endogeneità e per gestire dataset con molte variabili.

- **Vantaggi**:
  - Migliora la previsione dei propensity score e degli outcome.
  - Rende le stime meno sensibili ai modelli parametrici tradizionali.

- **Libreria Python**:
  - [`econml`](https://github.com/microsoft/EconML) sviluppata da Microsoft, che fornisce implementazioni di DML e altre tecniche causali.


### **3. Causal Forests**
I causal forests, basati sui Random Forests, sono progettati per stimare gli effetti causali eterogenei. Possono fornire stime degli effetti del trattamento individualizzati.

- **Vantaggi**:
  - Adatto per stimare effetti del trattamento variabili su subpopolazioni.
  - Non richiede ipotesi parametriche.

- **Libreria Python**:
  - [`grf`](https://grf-labs.github.io/grf/) (in R, ma può essere adattata per Python).


### **4. Bayesian Structural Time Series (BSTS)**
Questa tecnica utilizza modelli bayesiani per stimare effetti causali, in particolare quando si analizzano serie temporali. È simile al Synthetic Control Method ma con un'implementazione bayesiana.

- **Vantaggi**:
  - Include incertezza direttamente nelle stime.
  - Efficace per analisi di serie temporali.

- **Libreria Python**:
  - [`pybsts`](https://github.com/pybsts/pybsts).


### **5. Generalized Random Forests (GRF)**
Un'evoluzione dei causal forests, i GRF sono progettati per stimare una vasta gamma di parametri econometrici, inclusi effetti medi del trattamento, effetti eterogenei e persino parametri strutturali.

- **Vantaggi**:
  - Flessibilità nell'analisi causale e nella stima di effetti eterogenei.
  - Migliora le stime con regressori complessi.

- **Libreria Python**:
  - [`econml`](https://github.com/microsoft/EconML) e [`grf`](https://grf-labs.github.io/grf/) (implementato in R).


### **6. Instrumental Variable (IV) Methods with Machine Learning**
Le variabili strumentali combinate con il machine learning (ad esempio, Double Machine Learning con IV) migliorano l'identificazione di effetti causali nei contesti in cui c'è endogeneità.

- **Vantaggi**:
  - Riduce i problemi di endogeneità.
  - Usa modelli di machine learning per migliorare le previsioni delle variabili.

- **Libreria Python**:
  - [`econml`](https://github.com/microsoft/EconML).


### **7. Neural Causal Models**
Questi modelli utilizzano reti neurali per stimare effetti causali, con particolare enfasi sulle relazioni non lineari e sulla complessità strutturale dei dati.

- **Vantaggi**:
  - Estremamente flessibili e adattabili a grandi dataset.
  - Possono modellare relazioni non lineari tra trattamento, covariate e outcome.

- **Libreria Python**:
  - [`causalnex`](https://github.com/quantumblacklabs/causalnex) per modelli causali basati su grafi.
  - Implementazioni personalizzate con TensorFlow o PyTorch.


### **8. Targeted Maximum Likelihood Estimation (TMLE)**
Il TMLE è un metodo semi-parametrico che ottimizza la stima degli effetti causali, correggendo i bias residui in modelli non parametrici.

- **Vantaggi**:
  - Fornisce stime causali efficienti e robuste.
  - Basato su approcci statistici formali.

- **Libreria Python**:
  - [`zEpid`](https://zepid.readthedocs.io/) per analisi epidemiologiche e causali.

