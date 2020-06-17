# Timeline Heng Wang
## 22.Woche(1): Entwurf und Expose(Version 1.0)

25.Mai.2020, Kick-Off Meeting, begin

26.Mai.2020, Vorbereitung des Expose

27.Mai.2020, Gruppe Meeting, inhalt Expose
	env.: 是否需要nvida驱动 cuda cudnn tensorflow-gpu  

28.Mai.2020, Bücher suchen und download

29.Mai.2020, Andere packet installieren? Spyder? 

30.Mai.2020, Mit Huiqi diskutieren, Arbeitspacket
	* Bsp Code probieren
	* handson, 01, 线性回归

31.Mai.2020, Gruppe treffen, 10 Uhr, Expose

## 23.Woche(2): Entwurf und Expose(Änderung)

1.Juni.2020,

2.Juni.2020,
	EPIC-KITCHENS 2018
	https://data.bris.ac.uk/data/dataset/3h91syskeag572hl6tvuovwv4d
	The Breakfast Actions Dataset
	https://serre-lab.clps.brown.edu/resource/breakfast-actions-dataset/

3.Juni.2020, Treffen mit Betreuer, 11 Uhr, Expose --> Protokoll

4.Juni.2020, Versuch build opencv c++ in Laptop, aber nicht geschafft

5.Juni.2020, Bücher Sharing/Lesen.

6.Juni.2020, Vorbereitung für Gruppe treffen/Expose, Änderung des Exposes
    Start Bild sammeln

7.Juni.2020, Gruppe treffen, 10 Uhr, Expose, Protokoll schreiben, Bücher teilen. Aufgabe Verteilen

## 24.Woche(3): (Expose fertig stellen und Bild sammlern)

8.Juni.2020, Expose ändern(Zeitplan anpassen)

9.Juni.2020, herunterladen images von Flickr mit Hilfe des Extension von Chrome "Fatkun" und Hochladen nach Github
    Fater-RCNN--大目标检测，工业检测更担心的是漏检率recall
    FPN 多尺度检测问题，小目标检测

10.Juni.2020,
11.Juni.2020,
12.Juni.2020,
13.Juni.2020, 
14.Juni.2020, Bilder vorbearbeitung, Literatur--> Protokoll

## 25.Woche(4): (Bilder vorbearbeiten) ==> Katalog + Test Bild 
15.Juni.2020, Expose Deadline, Expose abgeben, zwischenpräsentationstermin Abgeben

16.Juni.2020,

17.Juni.2020,
































































Plattforms vergleichen, die erste Modell bauen
Plattforms probieren. und 

(Nutzen 1-1-Conv CNN realisieren, 2-3-Conv CNN realisieren, Plotten training und validation accuracy)




\item Ausblick auf Industrieanwendungen
















\ganttset{calendar week text={\currentweek}}
%\pgfcalendarmonthshortname{\startmonth}~\startday%
}%
}

\begin{ganttchart}[vgrid={draw=none,draw=none},%
            %today=15,%
            %today offset=.5,%
            %today label=Heute,%
            %progress=today,%
            time slot format=isodate
            x unit=0.5cm,
            y unit title=0.7cm,
            y unit chart=0.8cm,
            bar incomplete/.append style={fill=red},%
            progress label text=  {\quad\pgfmathprintnumber[precision=0,verbatim]{#1}\%},
            milestone label font=\tiny,
            group label font=\tiny,
            title label font=\tiny,
            bar label node/.style={text width=3cm,align=right,font=\scriptsize\RaggedLeft,anchor=east},
            milestone label node/.style={text width=2cm,align=right,font=\scriptsize\RaggedLeft,anchor=east},
            group label node/.style={text width=3cm,align=right,font=\scriptsize\RaggedLeft,anchor=east}
            ]{2020-05-25}{2020-09-30}

    \gantttitle{Projektwochen}{2020-09-30} \\
    \gantttitlelist{22,...,40}{1} \\
    \ganttgroup{Projektplanung}{22}{40} \\
    \ganttbar{Entwurf und Exposé}{2020-05-}{2} \\
    \ganttlinkedbar{A2,3: Datensammelung und -Analyse, Literaturrecherche}{3}{5} \ganttnewline
    \ganttnewline
    \ganttlinkedmilestone{Abschluss Datensammlung und Literaturrecherche}{5} \\ 
    \ganttnewline
    \ganttlinkedbar{A4: Modell (SVM) aufbauen und realisieren}{6}{7} \ganttnewline
    \ganttlinkedmilestone{SVM fertig}{7} \ganttnewline
    \ganttlinkedbar{A5: Mehrere Modelle aufbauen und realisieren}{8}{9}\\
    \ganttlinkedbar{Vorbereitung für Zwischsenpräsentation}{10}{10}\\
    \ganttlinkedmilestone{Zwischsen-präsentation}{11}{11}\\
    \ganttlinkedbar{A6: Neuronales Netzwerk realisieren}{12}{14}
    \ganttnewline
    \ganttlinkedmilestone{NN fertig}{14} \ganttnewline
    \ganttlinkedbar{A7: Eigenes Neuronales Netzwerk aufbauen}{15}{16}\\
    \ganttlinkedbar{A8: Auswertung und Dokumentation}{17}{17}\\
    \ganttnewline
    \ganttlinkedmilestone{Abschluss-präsentation und Projektabschluss}{18}{18}\\

% \ganttlink{elem3}{elem5}
% \ganttlink{elem4}{elem5}
% \ganttlink{elem5}{elem6}
\end{ganttchart}




