# Anomaly-Detector
# Descriere:
### Setul de date contine 3650 de randuri cu temperaturi diverse in intervalul: 1/1/1981 - 12/31/1990.
# Motivatia:
### Proiectul se focuseaza asupra detectarea anomaliilor folosind metode si grafice relevante pentru setul de date.
# Implementare:
  ## Preprocesarea datelor:
  -  incarcarea fisierului de tip csv.
  -  convertirea coloanei de data in datetime.
  -  verificarea daca exista valori nule in setul de date.
  ## Explorarea setului de date si plotarea graficelor:
  -  Pentru un set de temperaturi voi afisa temperaturile minime si maxime pentru afisarea posibilelor anomalii.
  -  informatii generale despre seturile de date.
  -  plotarea unui grafic de tip scatter pentru a plota temperaturile de-alungul anilor.
  -  plotarea unui grafic de tip histograma pentru a observa frecventa temperaturilor care vor aparea pentru recunoasterea anomaliilor.
  ## Metoda OCVSM:
  -  se bazeaza pe identificarea unei majoritati in cadrul unui set de date care sunt separate de potentialele anomalii.
  -  se defineste o frontiera marginala prin intermediul unui kernel si prin intermediul hiperparametrului "nu" care controleaza cate anomalii sunt permise.
  ## Metoda KNN:
  -  se calculeaza distanta dintre un punct si toate celelalte din cadrul setului de date.
  -  se selecteaza cei mai apropiati k vecini.
  -  se va atribui clasa majoritara.
  ## Metoda LODA:
  -  LODA proiecteaza datale pe mai multe axe unidimensionale alese aleator.
  -  algoritmul face o histograma pentru a estima densitatea datelor.
  ## Scoruri si indici de performanta:
  -  pentru verificarea corectitudinii algoritmilor vom implementa anumiti indici de performanta.
  ## Evaluarea rezultatelor:
  -  apelarea functii de test care foloseste mai multi parametrii diferiti.
  -  afisarea rezultatelor pentru fiecare metoda.
  ## Main:
  -  se apeleaza toate functiile.
  -  se declara parametrii diferiti pentru fiecare metoda care vor fi apelati in functia `evaluate_and_display_results(...)`.
# Performante:
  ## Acuratetea :
  - OCSVM: 98.08%
  - KNN: 91.95%
  - LODA: 91.64%
  ## F1-score, Recall , Precizie :
  - avand in vedere ca le calculez in cadrul anomaliilor vor fi destul de mici.
