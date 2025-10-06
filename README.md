# 🌍 Global Sustainable Development – SQL Data Analysis

## Titolo

**Analisi dello Sviluppo Sostenibile Globale: connessioni tra Economia, Ambiente e Migrazioni**

---

## Sommario

Progetto di analisi dati per un'organizzazione no profit impegnata nello sviluppo sostenibile globale. Attraverso query SQL su dataset internazionali, vengono esplorate le relazioni tra emissioni di CO₂, energie rinnovabili, PIL, qualità della vita e flussi migratori per supportare la redazione di un report comparativo tra Paesi.

**Risultati chiave:**
- Identificazione dei maggiori inquinatori e dei loro investimenti in energie rinnovabili
- Correlazioni tra energia rinnovabile, PIL e qualità della vita
- Collegamenti tra fragilità economica, sistemi sanitari deboli e migrazioni
- Evoluzione temporale degli indicatori di sostenibilità

---

## Problema

L'organizzazione necessita di comprendere le complesse relazioni tra sviluppo economico, sostenibilità ambientale e migrazioni per formulare raccomandazioni politiche efficaci. Domande chiave:

- Quali Paesi inquinano di più e stanno investendo in rinnovabili?
- Esiste correlazione tra energie rinnovabili e qualità della vita?
- Come si collegano sistemi sanitari precari e fragilità economica ai flussi migratori?
- Quali pattern emergono confrontando Paesi sviluppati e in via di sviluppo?

---

## 4️⃣ Metodologia

### Dataset Utilizzati

1. **Global Country Information Dataset (2023):** Dati economici, demografici e ambientali (PIL, disoccupazione, emissioni CO₂, sanità, istruzione)

2. **Global Data on Sustainable Energy:** Adozione energie rinnovabili, fonti di generazione elettrica, accesso all'energia

3. **Global Missing Migrants Dataset:** Migranti dispersi o deceduti durante il viaggio, con dettagli su rotte e paesi d'origine

### Processo di Data Cleaning

Ogni dataset è stato pulito accuratamente tramite script SQL dedicati:

- Rimozione duplicati con ROW_NUMBER() e PARTITION BY
- Validazione campi numerici (controllo separatori decimali multipli)
- Sostituzione valori vuoti con NULL
- Correzione caratteri speciali in nomi di paesi e città
- Rimozione simboli di valuta
- Conversione tipi di dati da TEXT a NUMERIC/INT/BIGINT
- Applicazione TRIM() per spazi bianchi

### Approccio Analitico

9 query SQL per rispondere a domande specifiche:

1. Top 10 Paesi per emissioni di CO₂
2. Paesi leader nell'uso di energie rinnovabili
3. Confronto emissioni vs investimenti rinnovabili (JOIN tra dataset)
4. Ranking sanità ed educazione (score composito)
5. Correlazione energia rinnovabile, PIL, aspettativa di vita e disoccupazione
6. Analisi migrazione e sistemi sanitari
7. Fragilità economica e flussi migratori
8. Impatto del PIL su migrazioni e disoccupazione
9. Evoluzione temporale PIL ed energia rinnovabile in Italia

---

## 5️⃣ Skills

**Tecniche SQL:**
- JOIN complessi (INNER, LEFT) tra tabelle multiple
- CTE per rilevamento duplicati
- Window functions (ROW_NUMBER, PARTITION BY)
- Funzioni aggregate (SUM, AVG, COUNT, MAX, MIN)
- Manipolazione stringhe (REPLACE, TRIM, REGEXP_REPLACE)
- Conversione tipi di dati con gestione errori (NULLIF)
- Pattern matching con espressioni regolari

**Analisi Dati:**
- Data cleaning e standardizzazione
- Gestione valori NULL
- Creazione metriche composite
- Identificazione correlazioni e pattern
- Analisi comparative tra Paesi
- Analisi di trend temporali

---

## 6️⃣ Risultati e Raccomandazioni

### Risultati Principali

**Ambiente ed Energia:**
- I maggiori emettitori di CO₂ mostrano impegni variabili verso le rinnovabili
- Più energia rinnovabile non implica necessariamente meno disoccupazione

**Sanità ed Educazione:**
- Forte divario tra Paesi con sistemi sanitari solidi (Nord Europa, Asia sviluppata) e Paesi in difficoltà (Africa Sub-Sahariana, Asia Centrale)

**Migrazioni ed Economia:**
- Paesi con alti flussi migratori presentano indicatori economici deboli (basso PIL, alta disoccupazione)
- Scarsa infrastruttura sanitaria correlata fortemente con emigrazione
- Paesi ricchi mostrano minore emigrazione e maggiore stabilità economica

### Raccomandazioni

1. **Programmi di Supporto Mirati:** Priorità ai Paesi con punteggio sanità-educazione più basso

2. **Assistenza Transizione Verde:** Supporto internazionale per Paesi ad alte emissioni che vogliono passare alle rinnovabili

3. **Strategia sulle Cause Migratorie:** Focus sul miglioramento delle condizioni economiche e sanitarie nei Paesi di origine

4. **Condivisione Best Practice:** Piattaforme di scambio tra Paesi che bilanciano con successo rinnovabili e crescita economica

5. **Framework di Monitoraggio:** Tracciamento regolare degli indicatori chiave identificati                           
```
