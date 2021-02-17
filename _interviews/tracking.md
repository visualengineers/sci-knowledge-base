---
layout: interview
title:  Interactions result in a stream of depth images.
teaser: 
image: 
image-credits: Mathias Müller
---

**Wozu braucht man das Tracking bei einem elastischen Display?**
wird verwendet um die Positionen, die Tiefe und die Art der Interaktion aus dem Depth-Touch zu erkennen

**Beschreibt das Setup nachvollziehbar (technisch und funktional). Was ist besonders wichtig?**
Azure Kinect ist unter dem flexiblen Display so angebracht dass die gesamte Touch-Fläche optimal erfasst werden kann
stabiles Anbringen der Kinect nötig um Nachkalibrierungen zu vermeiden

**Warum habt ihr euch für Tracking mit Tiefen-Kameras entschieden?**
direkte und schnelle Berechnung und Übermittlung der Tiefen-Karte durch die Tiefen-Kamera
unabhängig von Störlicht (ausserhalb des IR Spektrums), Beamer-Bild beeinflusst Tracking nicht
Beschaffenheit und Farbe der getrackten Oberfläche spielt bei diesem Verfahren weniger eine Rolle als bei anderen Methoden
ToF Kameras weniger IR störanfällig als IR Projektion

**Gibt es aus technischer Sicht relevante Unterschiede zwischen den aktuell verfügbaren Tiefen-Kameras?**
ToF (Kinect 2, Azure Kinect) - measuring the time emitted light takes from the camera to the object and back, constantly emits infrared light with modulated waves and detects the shifted phase of the returning light
Pattern Projection (Kinect 1) - known infrared pattern is projected into the scene and out of its distortion
the depth is computed
Vergleich: https://www.dfki.de/fileadmin/user_upload/import/8767_wasenmuller2016comparison.pdf

**Welche Kamera ist aktuell die beste und warum?**
ToF kamera: warscheinlich Azure Kinect: höchste Auflösung und Genauigkeit (1-Megapixel ToF imaging chip)

**Welche Daten erfasst die Kamera?**
Tiefenbild (bis zu 1MP) mit tiefenInformation pro pixel
Farbbild (bis zu 3840x2160 px)
IR Reflektion/Intensität ?
Position der Kamera (Gyro und accelerometer)

**Wie sieht der Datenstrom aus, den sie sendet?**
Tiefenbild: b16g (16-bit Grayscale, Big-endian)
RGB: Mode-Dependent (MJPEG, NV12, or YUY2)

**Könnte man die Interaktionen auf dem Display auch anders erfassen? Wenn ja, wie?**
Pattern projection (kinect1)
berührung könnte kapazitiv oder mittels leitfähigen flexiblen stoffen erfasst werden
evtl mechanische auswertung der Interaktion möglich
optisch über seitlich angebrachte stereo kameras
optische Auswertung der durchscheinenden hand / schatten
auch gestenerkennung über sihouette denkbar

**Wie fein (Auflösung) kann man tracken? Was bedeutet das hinsichtlich der möglichen Displaygröße?**
aktuell 1 MP mit Azure Kinect
displaygröße damit weiter skalierbar, aber aus usabilitysicht nicht praktikabel

**Welche Faktoren wirken sich negativ auf die Bildqualität aus?**
https://docs.microsoft.com/de-de/azure/kinect-dk/depth-camera siehe Invalidation
zu starke oder keine Reflektion des IR Signals (Oberflächeneigenschaften)
Umleitung des ausgesendeten lichts durch die geometrie,  multi-path detection (Verlängerung des licht-laufwegs)

**Wie kann man eine hohe Bildqualität sicherstellen?**
Der Stoff ist teilweise durchlässig. Welche Auswirkungen hat das auf das Tiefenbild und wie geht man damit um?

**Auf welche Probleme seid ihr (noch) gestoßen?**

**Was war besonders knifflig?**

**Was habt ihr gelernt?**

