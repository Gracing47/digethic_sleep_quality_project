

**1. Einleitung**

**1.1 Hintergrund und Motivation**  
Die Schlafqualität ist einer der wichtigsten Faktoren für das allgemeine Wohlbefinden und die Gesundheit des Menschen. Zahlreiche wissenschaftliche Studien haben gezeigt, dass schlechter Schlaf mit einer Vielzahl von gesundheitlichen Problemen, wie erhöhtem Stress, kardiovaskulären Erkrankungen und einer reduzierten Lebensqualität, in Verbindung steht. Gleichzeitig sind die Faktoren, die die Schlafqualität beeinflussen, vielfältig und komplex. Dazu gehören physiologische Parameter wie Herzfrequenzvariabilität, Bewegungen während des Schlafs, Stresslevel und Umweltbedingungen wie die Konsistenz der Schlafenszeiten und die Lichtexposition.

Moderne Technologien und tragbare Geräte haben es ermöglicht, eine große Menge an Gesundheits- und Schlafdaten zu sammeln. Diese Daten bieten eine wertvolle Grundlage, um durch den Einsatz von Methoden des maschinellen Lernens (ML) tiefergehende Erkenntnisse zu gewinnen und Zusammenhänge zu analysieren, die für die Vorhersage der Schlafqualität relevant sind. Insbesondere können Modelle des maschinellen Lernens dabei helfen, die komplexen Interaktionen der verschiedenen Einflussfaktoren zu analysieren, die mit der menschlichen Schlafqualität verbunden sind.

In der heutigen Zeit, in der Daten zunehmend als wertvoller Rohstoff betrachtet werden, bietet das Gebiet der Vorhersage der Schlafqualität durch maschinelles Lernen ein enormes Potenzial. Die Verwendung prädiktiver Modelle kann nicht nur zur besseren Selbstüberwachung und Optimierung der individuellen Schlafgewohnheiten beitragen, sondern auch Gesundheitsdienstleistern ermöglichen, präventive Maßnahmen zu entwickeln. Diese Projektarbeit soll genau diesen Bereich untersuchen und einen Beitrag zur besseren Vorhersage der Schlafqualität leisten, indem ein umfassender Ansatz zur Analyse synthetischer Schlaf- und Gesundheitsmetriken unter Einsatz von ML-Techniken vorgestellt wird.

**1.2 Zielsetzung und Forschungsfragen**  
Das Hauptziel dieser Arbeit ist es, die Schlafqualität auf Basis verschiedener synthetischer Schlaf- und Gesundheitsmetriken vorherzusagen. Dafür werden verschiedene prädiktive Modelle, von einfachen linearen Modellen bis hin zu komplexeren Verfahren wie Random Forest und XGBoost, verwendet und miteinander verglichen. Das Ziel ist es, herauszufinden, welches Modell am besten geeignet ist, um die Schlafqualität genau vorherzusagen und welche Faktoren dabei eine besonders wichtige Rolle spielen.

Im Rahmen dieser Arbeit sollen folgende Forschungsfragen beantwortet werden:
1. Können die entwickelten Modelle die Schlafqualität zuverlässig vorhersagen?
2. Welche Faktoren beeinflussen die Schlafqualität am stärksten?
3. Wie schneiden einfache Modelle im Vergleich zu komplexen Modellen ab, wenn es um die Vorhersagegenauigkeit der Schlafqualität geht?
4. Welche Faktoren könnten in zukünftigen Studien integriert werden, um die Vorhersage weiter zu verbessern?

Diese Forschungsfragen sollen durch eine umfassende Modellierung und Analyse der synthetischen Gesundheits- und Schlafmetriken beantwortet werden. Dabei wird nicht nur die Vorhersagegenauigkeit analysiert, sondern es werden auch die zugrunde liegenden Merkmale in ihrer Bedeutung für die Schlafqualität untersucht.

**1.3 Aufbau der Arbeit**  
Diese Arbeit gliedert sich in sechs Hauptkapitel. Das zweite Kapitel beschreibt den verwendeten Datensatz im Detail. Dazu gehört eine Übersicht der synthetischen Merkmale, die in die Analyse einfließen, sowie die angewendeten Schritte zur Datenaufbereitung und dem Feature Engineering. Das dritte Kapitel widmet sich der Methodik und den Modellen, die im Rahmen dieses Projekts verwendet werden. Es werden sowohl einfache als auch komplexe Algorithmen des maschinellen Lernens eingeführt, die später zur Vorhersage der Schlafqualität verwendet werden.

Im vierten Kapitel werden die Trainingsmethoden und die Modellbewertung beschrieben. Hierzu gehören die Aufteilung der Daten, das Training der Modelle und die angewendeten Bewertungsmethoden wie die Kreuzvalidierung und das Hyperparameter-Tuning. Die Ergebnisse dieser Modelle werden im fünften Kapitel dargestellt und diskutiert. Besondere Schwerpunkte liegen auf dem Vergleich zwischen einfachen und komplexen Modellen sowie der Analyse der wichtigsten Einflussfaktoren.

Das sechste Kapitel schließt die Arbeit ab und fasst die wesentlichen Erkenntnisse zusammen. Außerdem wird ein Ausblick auf mögliche zukünftige Arbeiten gegeben, wie beispielsweise die Integration weiterer Daten, um die Vorhersage der Schlafqualität weiter zu verbessern.



-----------------------------------------
-----------------------------------------

**2. Datenbeschreibung**

**2.1 Datensatzbeschreibung**  
Der verwendete Datensatz in dieser Arbeit ist der "Comprehensive Sleep and Health Metrics"-Datensatz, der vollständig synthetisch erstellt wurde. Dieser Datensatz wurde entwickelt, um eine breite Palette von Szenarien und Bedingungen zu simulieren, die die Schlafqualität beeinflussen könnten. Durch die Verwendung synthetischer Daten wird gewährleistet, dass eine umfassende Darstellung möglicher Variationen und Interaktionen zwischen verschiedenen Gesundheits- und Schlafmetriken bereitgestellt wird, ohne dass der Datenschutz verletzt wird.

Der Datensatz enthält Messungen verschiedener physiologischer und verhaltensbezogener Parameter, die eine potenzielle Auswirkung auf die Schlafqualität haben. Dazu gehören unter anderem Herzfrequenzvariabilität, Bewegung während des Schlafs, Stresslevel, Koffeinkonsum und Lichtexposition während des Tages. Insgesamt umfasst der Datensatz neun grundlegende Merkmale, die sowohl in ihrer isolierten Wirkung als auch in Kombination untersucht wurden.

**2.2 Datenmerkmale**  
Die Merkmale des Datensatzes lassen sich in verschiedene Kategorien unterteilen: physiologische Messungen, Verhaltensmerkmale und externe Einflussfaktoren. Jedes dieser Merkmale ist numerisch und wurde im Rahmen der Analyse in geeigneter Form verarbeitet und vorbereitet. Die wichtigsten Merkmale des Datensatzes sind:

- **Heart Rate Variability (HRV)**: Die Variabilität zwischen Herzschlägen, gemessen in Millisekunden. Ein höherer Wert deutet auf eine bessere Anpassungsfähigkeit des Körpers hin.
- **Body Temperature**: Die Körpertemperatur des Individuums, gemessen in Grad Celsius. Schwankungen der Körpertemperatur können Aufschluss über die Schlafqualität geben.
- **Movement During Sleep**: Die Anzahl der Bewegungen während des Schlafs, ein Indikator für Schlafstörungen oder Unruhe.
- **Sleep Duration Hours**: Die Gesamtdauer des Schlafs in Stunden. Ein adäquater Schlaf von mindestens sieben Stunden wird oft als gesundheitsförderlich angesehen.
- **Sleep Quality Score**: Ein synthetischer Wert zur Bewertung der Schlafqualität, der als Zielvariable für die prädiktive Analyse dient. Die Werte reichen von 1 bis 10, wobei höhere Werte auf eine bessere Schlafqualität hinweisen.
- **Caffeine Intake (mg)**: Die Menge des Koffeinkonsums in Milligramm. Koffein ist bekannt dafür, die Schlafqualität negativ zu beeinflussen.
- **Stress Level**: Ein Index, der das Stressniveau einer Person während des Tages darstellt. Ein höherer Wert deutet auf ein höheres Stressniveau hin, das sich negativ auf den Schlaf auswirken kann.
- **Bedtime Consistency**: Eine Skala von 0 bis 1, die angibt, wie konsistent die Schlafenszeiten einer Person sind. Niedrigere Werte zeigen größere Inkonsistenz.
- **Light Exposure Hours**: Die Anzahl der Stunden, die eine Person tagsüber natürlichem Licht ausgesetzt war. Lichtexposition ist wichtig, um den Schlaf-Wach-Rhythmus zu regulieren.

Diese Merkmale wurden nicht nur individuell betrachtet, sondern auch zu neuen, zusammengesetzten Merkmalen verarbeitet, um potenzielle Wechselwirkungen und nichtlineare Zusammenhänge zu berücksichtigen.

**2.3 Datenaufbereitung und Feature Engineering**  
Die Datenaufbereitung und das Feature Engineering sind wesentliche Schritte, um sicherzustellen, dass die Daten in einem optimalen Zustand für die Modellierung vorliegen. Zunächst wurden die synthetischen Daten auf fehlende Werte und Ausreißer untersucht. Fehlende Werte wurden entfernt, da eine Imputation aufgrund der synthetischen Natur der Daten nicht zielführend war. Potenzielle Ausreißer wurden identifiziert und entfernt, um die Vorhersagegenauigkeit der Modelle zu verbessern.

Im Rahmen des Feature Engineering wurden zusätzliche Merkmale erstellt, um potenzielle Wechselwirkungen zwischen den vorhandenen Merkmalen abzubilden. Beispiele hierfür sind:
- **Caffeine Squared**: Ein quadratisches Merkmal, um die nichtlineare Wirkung des Koffeinkonsums auf die Schlafqualität zu modellieren.
- **Caffeine_Stress_Interaction**: Ein Interaktionsmerkmal, das den kombinierten Einfluss von Koffein und Stress auf die Schlafqualität misst. Dies wurde erstellt, um mögliche Wechselwirkungen zwischen Koffeinkonsum und dem täglichen Stresslevel zu berücksichtigen.
- **Sleep Efficiency**: Ein Verhältnis zwischen der tatsächlichen Schlafdauer und der im Bett verbrachten Zeit, das als Maß für die Schlafqualität dient.
- **Light_Sleep_Ratio**: Ein Verhältnis zwischen der Lichtbelastung und der Schlafdauer, um den Einfluss der Lichtexposition auf den Schlaf zu erfassen.

Alle numerischen Merkmale wurden zudem skaliert und standardisiert, um die Daten für die verschiedenen Modelle des maschinellen Lernens vorzubereiten. Eine Kombination aus Min-Max-Skalierung und Standardisierung wurde verwendet, um sicherzustellen, dass die Modelle sowohl lineare als auch nichtlineare Beziehungen zwischen den Merkmalen erkennen können.

Die vorbereiteten und erweiterten Merkmale wurden in einem finalen Datensatz zusammengeführt, der anschließend in Trainings- und Testdatensätze aufgeteilt wurde. Dieser Prozess bildete die Grundlage für die Modellierung und Vorhersage der Schlafqualität mithilfe verschiedener Algorithmen des maschinellen Lernens.


-----------------------------------------
-----------------------------------------


**3. Methodik**

**3.1 Auswahl der Modelle**  
Zur Vorhersage der Schlafqualität wurden sowohl einfache als auch komplexe Modelle des maschinellen Lernens ausgewählt, um ihre Leistung in Bezug auf die Fähigkeit, die zugrunde liegenden Muster zu erkennen, zu vergleichen. Die Modellpalette wurde so konzipiert, dass eine Balance zwischen Interpretierbarkeit, Rechenaufwand und Vorhersagegenauigkeit erreicht wird. Die ausgewählten Modelle sind:

- **Lineare Regression**: Ein einfaches und interpretierbares Modell, das untersucht, ob die Schlafqualität linear durch die Eingabemerkmale beschrieben werden kann. Dies bietet eine grundlegende Einschätzung, ob ein linearer Zusammenhang zwischen den Variablen besteht.
- **k-Nearest Neighbors (kNN)**: Ein nicht-parametrisches Modell, das Vorhersagen auf Basis der k ähnlichsten Beobachtungen trifft. kNN dient als Referenz für die Modellleistung und zeigt, ob ähnliche Eingabemuster zu ähnlichen Ausgabewerten führen.
- **Random Forest Regressor**: Ein Ensemble-Lernalgorithmus, der aus einer Vielzahl von Entscheidungsbäumen besteht. Random Forest hilft dabei, die Bedeutung der einzelnen Merkmale zu identifizieren, und zeigt auch, wie gut ein Modell nichtlineare Beziehungen erfassen kann.
- **Support Vector Machine (SVM)**: Ein Modell, das eine robustere Vorhersage ermöglicht, indem es versucht, die Datenpunkte durch eine geeignete Trennlinie zu klassifizieren. Für die Regressionsaufgabe wurde der Kernel "rbf" verwendet, um komplexere Zusammenhänge zu modellieren.
- **XGBoost**: Ein Gradient-Boosting-Modell, das zur Verbesserung der Vorhersagekraft auf iterativer Optimierung basiert. XGBoost ist bekannt für seine Fähigkeit, starke Vorhersagen zu treffen und Feature-Importanzen präzise zu bewerten.

Ziel dieser Modellauswahl war es, ein tiefes Verständnis für die zugrunde liegenden Zusammenhänge im Datensatz zu entwickeln und die Vorhersagegüte der einfachen gegenüber der komplexen Modelle zu vergleichen. Zudem sollte untersucht werden, welche Merkmale die Schlafqualität maßgeblich beeinflussen.

**3.2 Datenaufbereitung (Normalisierung und Standardisierung)**  
Eine sorgfältige Datenaufbereitung ist von entscheidender Bedeutung, um die bestmögliche Modellleistung zu gewährleisten. Dabei wurden die folgenden Schritte durchgeführt:

- **Normalisierung**: Bei der Normalisierung wurden die numerischen Merkmale auf einen Wertebereich zwischen 0 und 1 skaliert. Dieser Schritt ist besonders wichtig, da die Modelle wie kNN und SVM empfindlich auf die unterschiedlichen Skalen der Merkmale reagieren. Durch die Normalisierung wird sichergestellt, dass alle Eingabemerkmale gleichwertig in die Berechnung der Distanzen einfließen.

- **Standardisierung**: Die Standardisierung wurde durchgeführt, indem jedes Merkmal z-standardisiert wurde, also der Mittelwert subtrahiert und durch die Standardabweichung geteilt wurde. Dieser Prozess sorgt dafür, dass die Merkmale eine Standardnormalverteilung mit einem Mittelwert von 0 und einer Standardabweichung von 1 haben. Insbesondere Modelle wie die lineare Regression profitieren von dieser Standardisierung, da sie auf Merkmale mit einer Normalverteilung empfindlicher reagieren.

Die Kombination dieser Techniken ermöglichte es, die Dateneigenschaften für die verschiedenen Modelle anzupassen und sicherzustellen, dass sowohl lineare als auch nichtlineare Modelle die bestmögliche Leistung erzielen.

**3.3 Trainings- und Testdatenaufteilung**  
Nach der Datenaufbereitung wurde der Datensatz in Trainings- und Testdaten aufgeteilt, um die Modellgüte zu evaluieren und eine Überanpassung zu vermeiden. Die Aufteilung erfolgte in einem Verhältnis von 80 % zu 20 %, wobei 80 % der Daten für das Training und die Hyperparameteroptimierung der Modelle verwendet wurden, während die verbleibenden 20 % als unabhängige Testdaten zur Evaluierung der Vorhersagegüte dienten.

Diese Aufteilung gewährleistet, dass die Modelle ausreichend Daten zur Verfügung haben, um die zugrunde liegenden Muster zu lernen, und dass gleichzeitig genügend Daten für eine unabhängige Bewertung der Modellleistung vorhanden sind. Um die Konsistenz der Ergebnisse sicherzustellen, wurde ein fester Zufallswert (Random Seed) verwendet, sodass die Ergebnisse reproduzierbar bleiben.

Die Trainingsdaten wurden zudem in einem Cross-Validation-Verfahren verwendet, wobei eine 5-fache Kreuzvalidierung durchgeführt wurde. Dies bedeutet, dass der Trainingsdatensatz in fünf gleich große Teile unterteilt wurde, von denen jeweils vier Teile zum Training und ein Teil zur Validierung verwendet wurden. Dieses Verfahren wurde iterativ wiederholt, sodass jedes Teil einmal als Validierungsdatensatz fungierte. Durch die Verwendung dieses Ansatzes wurde sichergestellt, dass die Modelle robust gegenüber Schwankungen und potenziellen Verzerrungen in den Daten sind.

Zusätzlich wurde eine Hyperparameteroptimierung, beispielsweise mittels Grid Search, durchgeführt, um die besten Parameter für Modelle wie Random Forest und SVM zu finden. So konnte die Vorhersagequalität der Modelle weiter verbessert und eine bestmögliche Generalisierung auf die Testdaten erreicht werden.



-----------------------------------------
-----------------------------------------


**4. Modelltraining und -bewertung**

**4.1 Modelle und Trainingsmethoden**  
Für das Modelltraining wurden die zuvor beschriebenen Modelle (Lineare Regression, k-Nearest Neighbors, Random Forest Regressor, Support Vector Machine und XGBoost) eingesetzt, um die Vorhersage der Schlafqualität zu optimieren. Jede Modellart bringt spezifische Stärken und Schwächen mit sich:

- **Lineare Regression** dient als Basismodell und bietet durch ihre Einfachheit eine grundlegende Einschätzung der linearen Zusammenhänge zwischen den Merkmalen und der Zielvariable.
- **k-Nearest Neighbors (kNN)** vergleicht Beobachtungen auf Basis ihrer Merkmalswerte und ermöglicht eine einfache, aber wirkungsvolle Methode, die Ähnlichkeit zwischen Beobachtungen zu quantifizieren.
- **Random Forest Regressor** nutzt die Stärke mehrerer Entscheidungsbäume und liefert nicht nur präzise Vorhersagen, sondern auch eine Einschätzung der Wichtigkeit einzelner Features, wodurch wertvolle Einblicke in die Relevanz verschiedener Merkmale gewonnen werden können.
- **Support Vector Machine (SVM)** versucht durch den Einsatz des Radial Basis Function (RBF) Kernels, komplexe und nichtlineare Zusammenhänge in den Daten zu modellieren und bietet damit eine gute Balance zwischen Einfachheit und Flexibilität.
- **XGBoost** ist ein Gradient-Boosting-Framework, das durch seine iterative Optimierung komplexe Zusammenhänge effizient modellieren kann. Es wird häufig bei Wettbewerben im Bereich maschinelles Lernen eingesetzt und erzielt in der Regel eine hohe Vorhersagegenauigkeit.

Zur Bewertung der Modelle wurden die Trainingsdaten in einem Verhältnis von 80 % zu 20 % in Trainings- und Testdaten aufgeteilt. Die Trainingsdaten wurden mittels **5-facher Kreuzvalidierung** (Cross-Validation) genutzt, um die Generalisierungsfähigkeit der Modelle sicherzustellen. Dieses Verfahren reduziert die Wahrscheinlichkeit von Überanpassung und ermöglicht eine robustere Einschätzung der Modellleistung.

**4.2 Hyperparameter-Tuning**  
Für die komplexeren Modelle, wie den **Random Forest Regressor** und **XGBoost**, wurde ein **Hyperparameter-Tuning** durchgeführt, um die Modellleistung zu optimieren. Beim Random Forest wurden unter anderem Parameter wie die Anzahl der Bäume (n_estimators) und die maximale Tiefe der Bäume (max_depth) variiert. Beim XGBoost wurden Parameter wie die Lernrate (learning_rate) und die Anzahl der Bäume untersucht.

Zur Optimierung wurde eine **Grid Search** verwendet. Dieses Verfahren sucht systematisch durch eine vorgegebene Menge an Hyperparameterkombinationen, um die Kombination zu finden, die die besten Ergebnisse auf den Validierungsdaten liefert. Im Falle des Random Forest Regressors führte die Grid Search zur Optimierung der Parameter „n_estimators“ und „max_depth“, was zu einer erheblichen Steigerung der Vorhersagegüte führte.

Nach dem Hyperparameter-Tuning wurde der Random Forest Regressor mit den optimalen Parametern erneut trainiert und zeigte eine signifikante Verbesserung der Modellgüte, insbesondere im Vergleich zu den Standardparametern. XGBoost profitierte ebenfalls von der Feinjustierung seiner Parameter und erzielte konsistent sehr niedrige Fehlerwerte.

**4.3 Evaluationsmetriken**  
Die Bewertung der Modelle erfolgte anhand folgender **Evaluationsmetriken**:

- **Mean Squared Error (MSE)**: Der mittlere quadratische Fehler (MSE) misst die durchschnittliche Abweichung der Vorhersagen von den tatsächlichen Werten. Ein niedriger MSE zeigt an, dass die Vorhersagen des Modells nahe an den tatsächlichen Werten liegen. Er wurde als Hauptmetrik zur Messung der Modellleistung verwendet, um die Unterschiede in den Vorhersagegüten der verschiedenen Modelle herauszustellen.
  
- **R²-Score**: Der R²-Score gibt an, wie gut das Modell die Varianz der Zielvariable erklärt. Ein hoher R²-Wert zeigt an, dass das Modell die zugrunde liegenden Zusammenhänge zwischen den Merkmalen und der Zielvariable gut erfasst. Dieser Wert wurde verwendet, um die Anpassungsgüte der Modelle zu bewerten und deren Erklärungskraft miteinander zu vergleichen.

**Vergleich der Modelle:**  
Nach dem Training und der Bewertung der Modelle zeigte sich, dass die **lineare Regression** und **kNN** eine vergleichsweise geringere Vorhersagegüte aufwiesen. Der **Random Forest Regressor** und **XGBoost** hingegen zeigten eine überragende Leistung mit einem MSE von nahezu 0, was auf eine sehr präzise Vorhersage hindeutet. Der **Support Vector Machine** (SVM) lag leistungstechnisch zwischen den einfachen und den komplexeren Modellen, wobei auch hier eine gute Anpassung beobachtet wurde.

Die Analyse der Feature-Importanzen zeigte, dass insbesondere der **Koffeinkonsum** einen erheblichen Einfluss auf die Schlafqualität hatte, während andere Merkmale wie Herzratenvariabilität und Lichtexposition eine geringere Rolle spielten. Diese Erkenntnisse können genutzt werden, um gezielte Empfehlungen zur Verbesserung der Schlafqualität zu geben.


-----------------------------------------
-----------------------------------------



## 5. **Ergebnisse und Diskussion**

### 5.1 Modellvergleich (Einfachere vs. Komplexere Modelle)

Im Rahmen der Analyse wurden sowohl einfache als auch komplexe Modelle verwendet, um die Vorhersage der Schlafqualität zu untersuchen. Die einfacheren Modelle, wie die lineare Regression und k-Nearest Neighbors (kNN), zeigten eine mäßige Vorhersagegenauigkeit. Das Modell der linearen Regression erreichte einen Mean Squared Error (MSE) von 3,82 und einen R²-Score von 0,56, was darauf hindeutet, dass es weniger geeignet ist, die komplexen Zusammenhänge zwischen den Features und der Schlafqualität zu modellieren. Das kNN-Modell zeigte eine bessere Leistung mit einem MSE von 2,19 und einem R²-Score von 0,75.

Auf der anderen Seite erreichten die komplexeren Modelle, wie der Random Forest Regressor, das Support Vector Machine (SVM) Modell und XGBoost, deutlich bessere Ergebnisse. Der Random Forest Regressor und XGBoost erzielten beide sehr niedrige MSE-Werte von 0,06 und hohe R²-Scores von 0,99, was auf eine hervorragende Vorhersageleistung hinweist. Das SVM-Modell erreichte ebenfalls eine gute Leistung mit einem MSE von 1,32 und einem R²-Score von 0,85.

Der Modellvergleich zeigt, dass die komplexeren Modelle in der Lage sind, die komplexen Beziehungen der Daten besser zu erfassen und damit eine genauere Vorhersage der Schlafqualität zu ermöglichen. Insbesondere die Verwendung von Ensemble-Methoden wie Random Forest und Boosting (XGBoost) hat sich als vorteilhaft erwiesen, um eine robuste und zuverlässige Modellleistung zu erzielen.

### 5.2 Feature-Importance-Analyse

Eine der wichtigsten Analysen im Modelltraining war die Untersuchung der Feature Importance, um zu verstehen, welche Variablen den größten Einfluss auf die Vorhersage der Schlafqualität haben. Die Feature-Importance-Analyse wurde insbesondere für den Random Forest Regressor und XGBoost durchgeführt, da diese Modelle die Möglichkeit bieten, die Bedeutung einzelner Features zu bestimmen.

Bei der Analyse der Feature Importances zeigten sich einige interessante Muster. Für beide Modelle war der **Koffeinkonsum** das wichtigste Feature für die Vorhersage der Schlafqualität, was darauf hinweist, dass Koffein eine erhebliche Auswirkung auf die Qualität des Schlafs hat. Insbesondere war dies der dominierende Faktor bei XGBoost, das diesem Feature eine sehr hohe Bedeutung zuwies.

Andere Features, wie **Bewegung während des Schlafs**, **Schlafdauer** und **Lichtexposition**, spielten ebenfalls eine Rolle, jedoch mit geringerer Bedeutung. Diese Analyse zeigt, dass die Reduktion von Koffeinkonsum und eine stabile Schlafumgebung (Bewegung und Licht) potenziell wichtige Einflussfaktoren auf die Verbesserung der Schlafqualität sein könnten.

Die weniger wichtigen Merkmale, wie die verschiedenen normalisierten und standardisierten Versionen derselben Variablen, hatten eine vernachlässigbare Auswirkung auf die Vorhersage und wurden daher in der finalen Analyse entfernt, um die Effizienz und Interpretierbarkeit der Modelle zu verbessern.

### 5.3 Vorhersage der Schlafqualität

Die Vorhersage der Schlafqualität wurde anhand von Kategorien durchgeführt, die den Schlaf in **"guter Schlaf"**, **"entspannter Schlaf"** und **"schlechter Schlaf"** unterteilen. Die Modelle zeigten eine bemerkenswerte Fähigkeit, die Schlafqualität basierend auf den verfügbaren Eingabedaten vorherzusagen. Besonders auffällig war, dass das optimierte Random Forest Modell die meisten Vorhersagen in die Kategorie "schlechter Schlaf" einordnete.

Die Analyse zeigt auch, dass es wenige Vorhersagen im Bereich des "guten Schlafs" gibt, was darauf hindeuten könnte, dass die vorliegenden Eingabedaten möglicherweise nicht ausreichend sind, um alle Faktoren für guten Schlaf zu erfassen. Beispielsweise könnten zusätzliche Faktoren, wie die genaue Einschlafzeit, die Ernährung und deren Qualität, emotionale Zustände sowie Ruhezeiten und möglicherweise der Einsatz von Medikamenten, entscheidend sein, um eine höhere Vorhersagegenauigkeit für besseren Schlaf zu erzielen.

Diese Erkenntnisse liefern wertvolle Hinweise darauf, welche zusätzlichen Daten benötigt werden könnten, um die Modelle weiter zu verbessern und genauere Vorhersagen über die Schlafqualität zu ermöglichen. Es ist geplant, die Modelle mit zusätzlichen Datenquellen zu erweitern, um eine umfassendere und realistischere Einschätzung der Schlafqualität bieten zu können.



-----------------------------------------
-----------------------------------------



## 6. **Schlussfolgerungen und Ausblick**

### 6.1 Zusammenfassung der Ergebnisse

In dieser Projektarbeit wurden verschiedene prädiktive Modelle eingesetzt, um die Schlafqualität auf der Grundlage von synthetischen Schlaf- und Gesundheitsmetriken vorherzusagen. Der Vergleich zwischen einfachen Modellen (wie der linearen Regression und k-Nearest Neighbors) und komplexeren Verfahren (wie Random Forest und XGBoost) hat deutlich gezeigt, dass die komplexeren Modelle eine deutlich höhere Vorhersagegenauigkeit erreichen. Besonders der Random Forest Regressor und XGBoost erzielten sehr niedrige Mean Squared Error (MSE)-Werte von 0,06 und hohe R²-Scores von 0,99, was eine nahezu perfekte Anpassung an die zugrunde liegenden Daten bedeutet.

Die Feature-Importance-Analyse hat aufgezeigt, dass der Koffeinkonsum ein bedeutender Einflussfaktor für die Schlafqualität ist. Diese Erkenntnis unterstützt die Annahme, dass Lebensgewohnheiten, wie z. B. der Konsum von Koffein, eine wesentliche Rolle bei der Verbesserung oder Verschlechterung der Schlafqualität spielen können. Die komplexeren Modelle waren in der Lage, die wesentlichen Einflussfaktoren genauer zu identifizieren und die komplexen Interaktionen zwischen den verschiedenen Merkmalen zu berücksichtigen.

Es wurde jedoch auch festgestellt, dass die vorliegenden Daten möglicherweise nicht ausreichen, um alle Faktoren, die für eine gute Schlafqualität entscheidend sind, umfassend zu berücksichtigen. Einfache Modelle, wie die lineare Regression, konnten die Beziehungen nicht so präzise erfassen wie die komplexeren Modelle. Dies deutet darauf hin, dass die Schlafqualität von vielen, möglicherweise nicht erfassten Variablen beeinflusst wird.

### 6.2 Potenzielle Anwendungen

Die Ergebnisse dieser Arbeit bieten wertvolle Einblicke in die prädiktive Modellierung der Schlafqualität und haben verschiedene potenzielle Anwendungen. Für Einzelpersonen können die entwickelten Modelle als Grundlage für personalisierte Empfehlungen zur Verbesserung der Schlafqualität dienen. Durch die Analyse individueller Gesundheitsmetriken und Schlafgewohnheiten könnten tragbare Geräte oder mobile Anwendungen genaue Vorhersagen und konkrete Tipps geben, um den Schlaf zu optimieren. Beispielsweise könnte die Reduktion des Koffeinkonsums als Maßnahme zur Verbesserung der Schlafqualität empfohlen werden.

Auch für Gesundheitsdienstleister bieten die entwickelten Modelle Potenzial. Sie könnten in der präventiven Gesundheitsvorsorge eingesetzt werden, um gefährdete Personen frühzeitig zu identifizieren und ihnen geeignete Maßnahmen zur Verbesserung der Schlafqualität vorzuschlagen. Langfristig könnte diese Art der Schlafanalyse dazu beitragen, die allgemeine Lebensqualität zu verbessern und die Häufigkeit von schlafbezogenen Gesundheitsproblemen zu reduzieren.

### 6.3 Zukünftige Arbeiten

Die vorliegende Arbeit hat gezeigt, dass die Vorhersage der Schlafqualität auf Basis von Gesundheits- und Schlafmetriken möglich ist. Um jedoch die Genauigkeit und die praktischen Anwendungen der Modelle weiter zu verbessern, sind zusätzliche Arbeiten erforderlich. Eine mögliche Erweiterung wäre die Integration weiterer Datenquellen. Beispielsweise könnten Informationen zu den genauen Schlafenszeiten, der Kalorienaufnahme, der körperlichen Aktivität sowie zu emotionalen Zuständen und Ruhezeiten eine tiefere Analyse ermöglichen. Auch der Einsatz von Daten zu Medikamenten und bestehenden gesundheitlichen Einschränkungen könnte die Modelle noch weiter verbessern.

Eine weitere Richtung für zukünftige Arbeiten wäre die Untersuchung zeitlicher Abhängigkeiten durch den Einsatz von Recurrent Neural Networks (RNNs) oder Long Short-Term Memory (LSTM)-Netzwerken. Diese Modelle könnten insbesondere die zeitliche Dynamik von Schlafmustern besser erfassen und damit zu noch präziseren Vorhersagen führen.

Zusätzlich sollte auch die Übertragbarkeit der Modelle auf reale Daten geprüft werden. Der in dieser Arbeit verwendete Datensatz war vollständig synthetisch, was zwar eine kontrollierte Untersuchung ermöglichte, jedoch möglicherweise nicht alle Aspekte der realen Welt widerspiegelt. Die Validierung der Modelle mit echten Gesundheits- und Schlafdaten wäre ein wichtiger Schritt, um die Anwendbarkeit in der Praxis sicherzustellen und die Modelle auf reale Szenarien zu optimieren.

