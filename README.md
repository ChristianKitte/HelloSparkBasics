# EA 13 - Spark Basics
### Data Science SS 21
### Christian Kitte 

### Aufgabe ###
Die aktuelle Aufgabe gliedert sich in zwei Teile. Zum einen soll versucht werden, Spark auf mehr als 
eine Art und Weise zum Laufen zu kriegen. Zum anderen sollen die Wortvorkommen aus den gesammelten 
[**Werken von Shakespeare**](https://ocw.mit.edu/ans7870/6/6.006/s08/lecturenotes/files/t8.shakespeare.txt) gezählt und das 24. meist verwendete Wort gefunden werden.

### Umsetzung ###
Als Zielsysteme für die reine Installation habe ich mir **Windows 10** und das als WSL (**Windows Subsystem 
für Linux**) verfügbare Linux verwendet. Letzteres läuft bei mir als ein vollwertiges Ubuntu. Die
Erklärungen hierzu finden sich in dem [**PDF**](https://github.com/ChristianKitte/HelloSparkBasics/blob/main/Installation%20von%20Spark%20unter%20Windows%2010.pdf), welches aktuell unter Firefox ein Anzeigeproblem hat.

Als drittes Zielsystem habe ich **Colab** verwendet. Diese Lösung ist als [**Notebook**](https://github.com/ChristianKitte/HelloSparkBasics/blob/main/SparkWordCount.ipynb) hier eingefügt. Sie ist schon alleine daher etwas umfangreicher, da zu Anfang die Installation von Spark selbst 
durch den jeweiligen Verwender erfolgen muss und daher diese selbst Teil der Lösung ist.

In dem Notebook wird daher durch Ausführung des Codes zunächst Spark installiert, die Quelldatei geholt und
in Colab abgelegt, dann einige Methoden definiert und letztlich die Wörter ausgezählt.

Alle Vorgänge sind hierbei sehr umfangreich dokumentiert und durch Verlinkungen erweitert.

### Lösung ###
Das 24. am häufigsten vorkommende Wort steht an der 24. Stelle der nullbasierten, absteigenden Liste 
am Ende des Notebooks und lautet **"have"** mit **5838 Vorkommen**. Warum an der 24. Stelle, wenn die Liste 
nullbasiert ist? Die Antwort liegt darin, dass an erster Stelle das einfache Leerzeichen steht. Ein 
Leerzeichen trennt Wörter, ist aber keins.
