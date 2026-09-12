NASA Turbofan Jet Engine Data Set 
Der NASA C-MAPSS-Datensatz enthält Betriebs und Sensordaten von simulierten Turbofan
Triebwerken. Für mehrere Triebwerke werden die Betriebszustände über aufeinanderfolgende 
Betriebszyklen hinweg aufgezeichnet. 
Der Datensatz umfasst 26 Variablen: die Triebwerks-ID (unit_number), den Betriebszyklus 
(time_in_cycles), drei Betriebsparameter (setting_1–setting_3) sowie 21 Sensorwerte 
(sensor_1–sensor_21). 
Für dieses Projekt werden drei Dateien verwendet: train_FD001.txt (vollständige Lebenszyklen 
zum Trainieren), test_FD001.txt (Beobachtungen bis zu einem unbekannten Zeitpunkt vor dem 
Ausfall) sowie RUL_FD001.txt (die tatsächliche verbleibende Nutzungsdauer der Test
Triebwerke, zur Evaluation). 
Die zeitliche Entwicklung der Sensorwerte ermöglicht die Untersuchung von 
Degradationsmustern und Veränderungen des Triebwerkszustands. Aus den Betriebszyklen 
kann außerdem die verbleibende Nutzungsdauer (Remaining Useful Life, RUL) bestimmt 
werden. Diese dient als Grundlage für die spätere Prognose mit Machine-Learning-Verfahren. 

( https://www.kaggle.com/datasets/behrad3d/nasa-cmaps ).

Projektidee, Beschreibung: 
Ziel des Projekts ist die Analyse von Betriebs- und Sensordaten von Flugzeugtriebwerken auf 
Basis des NASA C-MAPSS-Datensatzes. Die Daten werden zunächst eingelesen, strukturell 
untersucht und hinsichtlich ihrer Datenqualität überprüft und bereinigt. Anschließend werden 
die Daten im Rahmen einer explorativen Datenanalyse (EDA) untersucht, um Verteilungen, 
Zusammenhänge und Veränderungen der Sensorwerte über die Betriebszyklen zu erkennen. 
Ein Schwerpunkt liegt auf der Untersuchung der Sensorwerte und ihrer Entwicklung während 
des Betriebs der Triebwerke. Mithilfe statistischer Analysen, Korrelationsanalysen und 
geeigneter Visualisierungen sollen relevante Muster und Merkmale identifiziert werden. 
Darüber hinaus werden Unterschiede und Auffälligkeiten im Betriebsverhalten einzelner 
Triebwerke sowie Degradationsmuster untersucht. 
Auf Basis der gewonnenen Erkenntnisse werden geeignete Data-Mining-, Machine-Learning- 
sowie Deep-Learning-Verfahren zur Prognose der verbleibenden Nutzungsdauer (Remaining 
Useful Life, RUL) angewendet und anhand geeigneter Kennzahlen bewertet und verglichen. 
Die wichtigsten Ergebnisse der Analyse und Modellierung werden abschließend in einem 
Dashboard dargestellt. 

#How to run :

Clone the repo and enter it:
   
   git clone https://github.com/MehrBSh/Analysis-and-Prediction-of-Remaining-Useful-Life-of-Turbofan-Engines-.git
   
   cd Analysis-and-Prediction-of-Remaining-Useful-Life-of-Turbofan-Engines-


#Create and activate a virtual environment:

   python -m venv .venv
   
   # Windows
   
   .venv\Scripts\activate
   
   # macOS/Linux
   
   source .venv/bin/activate

   pip install -r requirements.txt

   #Launch and run the notebook

      
  jupyter notebook


