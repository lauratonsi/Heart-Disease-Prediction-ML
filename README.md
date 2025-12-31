# Heart Disease Prediction: Supporto Decisionale Clinico tramite ML

## 📌 Visione del Progetto
Sviluppo di modelli predittivi per la diagnosi precoce di malattie cardiache. L'obiettivo non è solo l'accuratezza statistica, ma l'ottimizzazione della **Recall** (sensibilità), fondamentale in ambito medico per ridurre al minimo i falsi negativi (pazienti malati non diagnosticati).

## 🛠️ Tech Stack
- **Linguaggio:** Python (su Google Colab).
- **Librerie:** Pandas, NumPy, Scikit-learn.
- **Algoritmi:** Support Vector Machine (SVM), Decision Tree.

## 📊 Analisi Clinica e Risultati
Ho confrontato diversi approcci modellistici, analizzando il trade-off tra le metriche:
- **SVM (Dataset Completo):** Migliore accuratezza globale (82%), ma minor sensibilità sui casi positivi.
- **SVM (Feature Selection):** Sebbene l'accuratezza scenda leggermente (79%), questo modello ha dimostrato una capacità superiore di intercettare i pazienti a rischio (Recall sulla Classe 1: 91% vs 81%).

## 💡 Insight Strategico
L'analisi dimostra che in contesti **HealthTech**, la metrica "vanitosa" (Accuracy) non è sempre la migliore. Ho scelto di privilegiare il modello che massimizza l'identificazione delle patologie, accettando un numero maggiore di falsi positivi pur di garantire la sicurezza del paziente.

## 📂 Dataset
Analisi effettuata su parametri biomedici standard tra cui:
- Pressione sanguigna a riposo (trtbps)
- Livelli di colesterolo (chol)
- Risultati ECG e Angina indotta da esercizio.
