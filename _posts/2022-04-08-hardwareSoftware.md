---
layout: post
title: "Entwicklung von Hard- und Softwareschnittstellen I"
date:   2022-04-08 15:00:00 +0000
categories: Werkstattkurse
---

## 1. Treffen 08.04.22

Michael Ohme zeigt uns einige kleine Beispielprojekte. Jeder erzählt, welche Wünsche/ Erwartungen er an den Kurs hat.

### Spannung **U** [V]
- Als Spannung bezeichnet man die Fähigkeit einer elektrischen Quelle, in einem Stromkreis einen Strom aufrechtzuerhalten.

- Die elektrische Spannung hat das Formelzeichen **U** und wird in der Einheit **[U] = 1 (Volt)** angegeben.<br>
siehe Leifiphysik: 
[Elektrische Spannung](https://www.leifiphysik.de/elektrizitaetslehre/elektrische-grundgroessen/grundwissen/elektrische-spannung)

### Stromstärke **I** [A]
- Die elektrische Stromstärke, Symbol **I**, ist ein Maß für die elektrische Ladung, die pro Sekunde durch einen Leiterquerschnitt hindurchfließt.
- Die Einheit der elektrischen Stromstärke ist das Ampere, Symbol **A**.<br> 
siehe Leifiphysik: [Elektrische Stromstärke](https://www.leifiphysik.de/elektrizitaetslehre/elektrische-grundgroessen/grundwissen/elektrische-stromstaerke)

### Leistung **P** [W]
- Die elektrische Leistung gibt dir an, wie viel elektrische Energie in einer gewissen Zeit umgesetzt wird. Sie beschreibt sozusagen den Energieverbrauch der Verbraucher. Die Leistung lässt dich berechnen mittels der Stromstärke– und Spannung:<br> 
**W = U * I**<br>
siehe: [Elektrische Leistung](https://studyflix.de/elektrotechnik/elektrische-leistung-1878)

### Widerstand **R** [Ω]
**R = U / I**<br>
Bei den Kohlenstoffwiderständen: Jede Farbe steht für eine Ziffer.<br>
Braun: 1<br>
Schwarz: 0<br>
Rot: 2 (Steht für die Zehnerpotenz)<br>
Also bei einem Widerstand mit einem braunen, schwarzen und roten Streifen beträgt der Widerstand 1000 Ohm.<br>
Siehe: [Widerstandsfarbcode-Tabelle](https://www.elektronik-kompendium.de/sites/bau/1109051.htm)


**Beim Messen:**<br>
Eins der Pole kennzeichne ich als 0 Volt (schwarzes Kabel). Das rote Kabel für die Spannung.
Bei der Batterie lege ich das schwarze Kabel and das Minus und das rote an das plus (um einen positiven Wert für die Stromstärke zu erhalten.)

Eher Arbeit mit hohen Spannungen und nicht so hohen Stromstärken.

_Treffen am 15.04. ist Feiertag und fällt daher aus._

## 2. Treffen – 22.04.22

Kurze Klärung zur Thematik Gleichstrom vs Wechselstrom (siehe [Stromkrieg](https://de.wikipedia.org/wiki/Stromkrieg)).

Wenn eine Arbeit mit größeren Stromspannungen im öffentlichen Raum ausgestellt wird, muss sie von einem Elektriker abgenommen werden.

Kurze Wiederholung von letzter Woche: 
- Strom **I** [A] 
- Spannung **U** [V]
- Leistung **P** [W]
    - P = I * U
    - 1W = 1A * V
- Widerstand **R** [Ω]
    - U =  R * I, R = U / I

**Schalter**<br>
[(Liste der Schaltzeichen)](https://de.wikipedia.org/wiki/Liste_der_Schaltzeichen_(Elektrik/Elektronik)#Schalter)
Mit einer Durchgangsprüfung (Menüpunkt am Messgerät) kann ich feststellen, um es sich um einen Taster oder Tastschalter handelt. Alternativ kann auch einfach der Widerstand gemessen werden.

––– Kleine Pause –––

**Potentiometer**<br>
Über Widerstandsring realisiert.

**Kirchhoffsche Regeln**<br>
1. Kirchhoffsches Gesetz (Knotenregel):<br>
_In einem Knotenpunkt eines elektrischen Netzwerkes ist die Summe der zufließenden Ströme gleich der Summe der abfließenden Ströme._
2. Kirchhoffsches Gesetz (Maschenregel): <br>
_Alle Teilspannungen eines Umlaufs bzw. einer Masche in einem elektrischen Netzwerk addieren sich zu null._<br>
(von [wikipedia](https://de.wikipedia.org/wiki/Kirchhoffsche_Regeln))

## 3. Treffen – 29.04.22

Spannungsteiler<br>

Anders als ein Widerstand ist eine Diode kein lineares Bauelement.
20mA ist ein Standardwert zum Betreiben von Leuchtdioden. Es gibt auch einige, dir nur 2mA benötigen.

Rechnung:<br>
_Bei Spannungquelle von 5 Volt und einer Leuchtdiode die 20mA braucht. Wie hoch soll der Widerstand sein?_<br>
_I = U / R umstellen nach R = U / I_<br>
_5V / 20mA_ <br>
_= 5V / 0.02A_ <br>
_= 250 V/A_ <br>
_= 250 Ω_


U<sub>1</sub> / U<sub>2</sub> = R<sub>1</sub> / R<sub>2</sub><br>

R = U<sub>1</sub> / I<sub>1</sub> = (U<sub>G</sub> - U<sub>LED</sub>) / I<sub>1</sub> = 5V - 2V / 20mA = 150Ω

Wir stecken eine kleinen Schaltkreis auf dem Steckboard.

––– Kurze Pause –––

### Aufbau Diode

Diode besteht aus einer P Schicht, einer N Schicht und einer Sperrzone.
![Diode](/assets/images/diode.webp)


<img src="{{ site.baseurl }}/assets/images/diode.webp" width="400">


### Aufbau Transistor
<img src="{{ site.baseurl }}/assets/images/npnTransistor.gif" width="300">

<!-- ## 4. Treffen am 06.05.22
## 5. Treffen am 13.05.22 -->

## Treffen am 10.06.22
Wir expertieren mit verschiedenen Sensoren und schreiben kleine Arduino Programme.<br>

Mikrokontroller der besser für Audio geeignet ist: Teensy oder ASP32.

## Treffen am 17.06.22
Ich war krank :(
