# Quantum Classification on Wine Dataset  
> Variational Quantum Circuits on the UCI Wine dataset

## 🗺️ Che cosa troverai qui

**Obiettivo del progetto**  
Costruire, addestrare e analizzare **Variational Quantum Circuits (VQC)** per la classificazione del *Wine Dataset* e confrontare l’intero flusso di lavoro con i migliori algoritmi di Machine Learning classici.  
Il focus è metodologico: come progettare pipeline ibride (classico + quantum), come gestire la fase di ottimizzazione parametrica, come valutare la robustezza ai rumori hardware.

**Step principali**

1. **Data pipeline**  
   - Caricamento e pulizia del *Wine dataset* da UCI ML Repository.  
   - Feature scaling e PCA per ridurre il numero di qubit necessari.  
2. **Encoding quantistico**  
   - Mappe di feature \(ZFeatureMap, ZZFeatureMap, ecc.\) per trasformare i vettori reali in stati quantistici.  
3. **Progettazione dell’ansatz**  
   - Vari schemi (EfficientSU2, TwoLocal, ecc.) modulati da *reps* e *entanglement* pattern.  
4. **Ottimizzazione dei parametri**  
   - Confronto fra ottimizzatori derivative-free (COBYLA, Nelder–Mead, Powell) e gradient-based (L-BFGS-B, SLSQP).  
5. **Back-end di esecuzione**  
   - Simulatore ideale *AerSimulator*.  
   - Noise model realistico (IBM FakeVigoV2) per studiare l’impatto dei gate error e della decoerenza.  
6. **Baseline classiche**  
   - SVM, Random Forest, K-NN, Naïve Bayes, Gradient Boosting, Logistic Regression.  

---

## 📂 Struttura della repo

| Path | Contenuto |
|------|-----------|
| `PROGETTO_QC_MARTUCCI_271316_ZAPPIA_268784.ipynb` | Notebook “main”: preprocessing, design dei circuiti, training e valutazione |
| `OTTIMIZZATORI_NON_QUANTISTICI.ipynb` | Esperimenti sugli ottimizzatori classici per i parametri del VQC |
| `SIMULAZIONI_CON_RUMORE_1_E_2_REPS.ipynb` | Studio della robustezza dei circuiti su noise model IBM |
| `Relazione_progetto_Quantum_Computing.pdf` | Report analitico con dettagli teorici e diagrammi |
| `requirements.txt` | Dipendenze principali (Qiskit, scikit-learn, ecc.) |
| `README.md` | Questa descrizione |


## 👥 Autori

- Anastasia Martucci
- Giuseppe Zappia


---

## 📌 Note finali

Il progetto è stato sviluppato nell’ambito del corso di Quantum Computing (A.A. 2024/2025), all’interno del corso di laurea magistrale in Ingegneria Informatica presso l’Università della Calabria.

