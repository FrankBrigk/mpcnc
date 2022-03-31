# Dokumentation

# Baumraum
Geplanter Baumraum: (X|Y|Z): 980 x 1500 x 81 mm
Tatsächlicher Baumraum: (X|Y|Z): ? x ? x ? mm

Der Unterschied entsteht, da die Trucks auf der X-Achse anders als vorgesehen auf Rohre montiert wurden und damit der Core nicht in die Nut der Trucks fahren kann. Das die Trucks nicht nach Dokumentation montiert wurden hatte den Grund, dass der Fräßer von dem PC aus sichtbar sein sollte, um den Fräßvorgang von dort beobachten und ggf eingreifen zu können.

# Komponentenübersicht

Die Komponentenübersicht zeigt alle im Kontext der MPCNC genutzen Komponenten und deren Schnittstellen. 

<img src="MPCNC_Component_View.png" style="background-color: white;">


## Estlcam
Estlcam wird in der Version 11 verwendet

## Motoren
Es werden Nema 17 Motoren verwendet.

## Endschalter
Die Endschalter sind öffner und werden in reihe geschalten. Das hat den Vorteil, dass Kabelbrüche erkannt werden können, da in diesen Fall die Schalter immer als Ausgelöst erkannt werden. 

Die Reihenschaltung ist möglich, da Estlcam bei der Referenzfahrt in folgender Sequenz vorgeht:
 
- Einlernen der Z-Achse 
- Einlernen der X-Achse
- Einlernen der Y-Achse

Das Einlernen beinhaltet das Verfahren der Achse bis zum Endanschlag, anschließendes reversieren um einen konfigurierbaren Weg, nochmals Verfahren bis zur Achse und ein erneutes reversieren.

Das zweite Verfahren ist eine genaue Messfahrt um den Endanschlag so genau wie möglich zu ermitteln um anhand der vorherigen Messung Pulsverluste zu ermitteln.

## Tastplatte
Maße: 


# CNC Shield v3

## Pinout

<img src="CNC Shield v3.jpg" style="background-color: white;">