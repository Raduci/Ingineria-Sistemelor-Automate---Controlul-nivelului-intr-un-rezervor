# Proiect: Controlul Nivelului într-un Rezervor  
**Ingineria Sistemelor Automate**

## Descriere Generală

Acest proiect abordează problema menținerii unui nivel constant al apei într-un rezervor care alimentează un proces industrial, în ciuda variațiilor de debit la evacuare. Pentru a realiza acest obiectiv, este utilizat un sistem automatizat cu control feedback, care reglează debitul de alimentare.

Sistemul include următoarele componente și mărimi principale:

- **LC**: Regulator de nivel (Level Controller)  
- **LT**: Traductor de nivel (Level Transducer)  
- **E/P**: Element de execuție electric/pneumatic  
- **RR**: Robinet de reglare  
- **Q_i**: Debitul de intrare  
- **Q_e**: Debitul de ieșire (evacuare)  
- **i_m**: Semnal de măsură (curent 4...20 mA)  
- **i_r**: Semnal de referință (curent 4...20 mA)  
- **i_e**: Semnal de comandă (curent 4...20 mA)  
- **p_e**: Presiune de comandă (0.2...1 bar)

Traductorul de nivel măsoară înălțimea lichidului (**h**) și generează un semnal electric **V(t)** proporțional cu aceasta. Acesta este modelat ca un sistem de ordinul I, cu:

- Câștig static: **K = 0.5 V/m**
- Timp de răspuns: **T = 2 secunde**

---

## Obiective și Cerințe

Proiectul urmărește îndeplinirea următoarelor cerințe:

### 1. Analiza sistemului de execuție și a procesului
- Determinarea funcției de transfer a elementului de execuție (EE) și a procesului (P), pe baza caracteristicilor frecvență-amplitudine-pulsație.
- Modelarea intrare-ieșire a procesului folosind o ecuație liniară.
- Schițarea repartiției polilor și zerourilor în planul complex.
- Evaluarea stabilității interne și externe a procesului.

### 2. Analiza sistemului de reglare
- Evaluarea stabilității utilizând un criteriu de stabilitate în frecvență (la alegere).
- Calcularea performanțelor dacă sistemul este stabil.

### 3. Proiectarea unui regulator PID
- Aplicarea unei metode experimentale pentru reglajul PID.
- Calculul performanțelor sistemului obținut cu PID.

### 4. Proiectarea unui regulator fuzzy
- Implementarea unui regulator pe bază de logică fuzzy.
- Compararea performanțelor cu cele obținute în cazul regulatorului PID.

---

## Informații Suplimentare

- **Nivel dorit**: 150 cm  
- **Înălțime totală a bazinului**: 200 cm  
- **Perturbație aplicată**: Implementată cu blocul **Signal Builder** din Matlab/Simulink, conform unui semnal temporal definit.

---

## Structura Proiectului

Proiectul conține fișiere Matlab/Simulink (.m și .slx), utilizate pentru:

- Simularea sistemului de control
- Proiectarea regulatorilor (PID și fuzzy)
- Analiza răspunsului la perturbații și a performanțelor dinamice

---

## Cerințe Software

- **MATLAB/Simulink**  
  Necesare pentru:
  - Rularea simulărilor
  - Modelarea componentelor sistemului
  - Proiectarea și testarea regulatorilor

---

## Rulare și Verificare

1. Deschide fișierele `.m` sau `.slx` în MATLAB/Simulink.
2. Rulează simulările corespunzătoare fiecărui punct din proiect.
3. Evaluează performanțele obținute și compară rezultatele între cele două tipuri de regulatori.

---

## Autor

- **Student**: Tene Radu-Ștefan  
- **Specializare**: Automatică și Informatică Aplicată  
- **Anul**: III  
- **Facultatea**: Hidrotehnică  
- **Universitatea**: Universitatea Tehnică de Construcții București

---

