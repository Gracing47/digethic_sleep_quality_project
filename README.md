# Projektarbeit: Analyse der Einflussfaktoren auf die Schlafqualität mittels maschinellen Lernens

Verfasst im Rahmen der EN ISO / IEC 17024-Zertifizierungsprüfung von  
**Thomas Fosu Serwah**  
04.10.2024

---

## Inhaltsverzeichnis

1. [Einleitung](#einleitung)
2. [Projektbeschreibung](#projektbeschreibung)
3. [Zielsetzung](#zielsetzung)
4. [Methodik](#methodik)
5. [Ergebnisse](#ergebnisse)
6. [Schlussfolgerungen](#schlussfolgerungen)
7. [Ausblick](#ausblick)
8. [Anforderungen](#anforderungen)
9. [Anleitung zur Reproduktion](#anleitung-zur-reproduktion)
10. [Kontakt](#kontakt)

---

## Einleitung

In der modernen Gesellschaft beeinflussen zahlreiche Faktoren die Schlafqualität der Menschen. Stress, Koffeinkonsum und digitale Medien sind nur einige der Elemente, die zu Schlafstörungen führen können. Diese Projektarbeit untersucht mithilfe von maschinellen Lernverfahren die verschiedenen Einflussfaktoren auf die Schlafqualität, um ein tieferes Verständnis für die zugrunde liegenden Zusammenhänge zu gewinnen.

## Projektbeschreibung

Diese Arbeit analysiert Daten, die verschiedene Gesundheits- und Lebensstilmetriken umfassen, um herauszufinden, welche Faktoren die Schlafqualität am stärksten beeinflussen. Dabei wird insbesondere der Koffeinkonsum in den Fokus gerückt, um Erkenntnisse darüber zu gewinnen, wie sich dieser auf das Schlafverhalten auswirkt.

## Zielsetzung

- **Identifikation der Hauptfaktoren**: Bestimmen, welche Variablen den größten Einfluss auf die Schlafqualität haben.
- **Modellierung der Zusammenhänge**: Einsatz von maschinellen Lernmodellen zur Vorhersage der Schlafqualität basierend auf den identifizierten Faktoren.
- **Verbesserung der Schlafqualität**: Entwicklung von Empfehlungen zur Reduzierung negativer Einflussfaktoren, insbesondere für Personen mit hohem Koffeinkonsum.

## Methodik

- **Datenbeschaffung**: Verwendung eines synthetischen Datensatzes mit Gesundheits- und Schlafmetriken.
- **Datenvorverarbeitung**: Bereinigung und Vorbereitung der Daten, Erstellung neuer Features.
- **Modellierung**: Anwendung verschiedener maschineller Lernmodelle, darunter Lineare Regression, Random Forest und Support Vector Regression (SVR).
- **Evaluation**: Vergleich der Modelle anhand von Metriken wie R² und Mean Squared Error (MSE).
- **Visualisierung**: Einsatz von Diagrammen und Grafiken zur Darstellung der Ergebnisse.

## Ergebnisse

- **Haupteinflussfaktoren**: Der Koffeinkonsum wurde als signifikanter Prädiktor für die Schlafqualität identifiziert, gefolgt von Stresslevel, Schlafdauer und Lichtexposition.
- **Modellleistung**: Der Random Forest erzielte die höchste Vorhersagegenauigkeit, was auf die Fähigkeit hindeutet, komplexe nichtlineare Zusammenhänge zu erfassen.
- **Feature Importance**: Konsistente Identifizierung der wichtigsten Variablen über verschiedene Modelle hinweg, was die Robustheit der Ergebnisse unterstreicht.

## Schlussfolgerungen

Die Analyse zeigt, dass der Koffeinkonsum einen maßgeblichen Einfluss auf die Schlafqualität hat. Um die Schlafqualität von Personen, die regelmäßig Kaffee konsumieren, zu verbessern, ist es essenziell, weitere reale Daten zu sammeln und detailliertere Untersuchungen durchzuführen. Die Ergebnisse legen nahe, dass durch gezielte Interventionen, wie die Reduzierung des Koffeinkonsums und das Stressmanagement, die Schlafqualität verbessert werden kann.

## Ausblick

- **Erweiterung der Datengrundlage**: Sammlung und Analyse von realen Daten, um die Generalisierbarkeit der Modelle zu erhöhen.
- **Tiefergehende Untersuchungen**: Berücksichtigung weiterer Einflussfaktoren wie genetischer Prädispositionen und detaillierter physiologischer Messungen.
- **Anwendung von Deep Learning**: Einsatz tiefer neuronaler Netze zur Erkennung noch komplexerer Muster in den Daten.
- **Langzeitstudien**: Durchführung longitudinaler Studien, um kausale Zusammenhänge zu identifizieren und die Wirkung von Interventionen zu bewerten.

## Anforderungen

- **Software**: Python 3.x
- **Bibliotheken**:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

## Anleitung zur Reproduktion

1. **Repository klonen**: Laden Sie das Projekt aus dem entsprechenden Repository herunter.
2. **Umgebung einrichten**: Installieren Sie die erforderlichen Python-Bibliotheken.
3. **Datensatz bereitstellen**: Stellen Sie sicher, dass der Datensatz `wearable_tech_sleep_quality_1.csv` im Arbeitsverzeichnis vorhanden ist.
4. **Notebook ausführen**: Öffnen Sie das Jupyter Notebook `Analyse_Schlafqualitaet.ipynb` und führen Sie die Zellen der Reihe nach aus.
5. **Ergebnisse überprüfen**: Analysieren Sie die generierten Visualisierungen und Modellbewertungen.

## Kontakt

Für Fragen oder Anmerkungen wenden Sie sich bitte an:

**Thomas Fosu Serwah**  
E-Mail: tom.blessed47@gmail.com