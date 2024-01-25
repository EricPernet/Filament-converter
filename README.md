# Filament-converter
Informatik Projekt Eric Pernet, Efraim Sander


Dies ist das Abschlussprojekt im Grundlagenfach Informatik der Kantonsschule Kreuzlingen von Eric und Efraim (Herbstsemester 2023). Dieses Projekt beinhaltet den OpenSCAD Code für die Vorrichtung der Spule, wie auch das komplette Arduino-Skript (C++), welches komplett funktionsfähig ist. 
Die Codes und Dokumentation sind vollständig von uns, ansonsten sind die Quellen verlinkt. Bei Fragen und anregungen bitte eric.pernet@ksk.ch oder efraim.sander@ksk.ch kontaktieren. 

## Informationen zum Projekt

Das Ziel des Filament-converters ist es, geschnittene PET-Flaschen Streifen durch einen Heizblock zu ziehen um dadurch Filament herzustellen, welches in einen üblichen 3D Drucker eingeführt werden kann. 

Unten folgt ein Bild mit einer Legende für die Ausführung des Projekts von Efraim und mir. Das Setup könnte auch beliebig geändert werden. 

![FIlamentmaker](https://github.com/EricPernet/Filament-converter/assets/142325259/c59eba51-0d83-4b5b-847e-01949284855a)

**1. PET-Faden Spule:** Die Spule musste einmal erneut gedruckt werden, da die alte zu gross war (Siehe Session 6). Nun passt sie jedoch und der geschnittene PET-Flaschen Streifen kann gut hineingedreht werden und anschliessend in den Heatblock geschoben werden.

**2. Heatblock:** Der Heatblock wurde mithilfe eines Metallstücks montiert, da eine 3D gedruckte Vorrichtung geschmolzen wäre. Dieses Setup funktioniert sehr zuverlässig, man muss jedoch darauf aufpassen, das Material nicht zufällig anzufassen da es beim erhitzen sehr hohe Temperaturen erreicht. Hier kann der PET Faden eingezogen werden. Auf der anderen Seite kommt ein etwa 1.8 milimeter breiter Filament-Streifen heraus.

**3. Lüfter:** Der Lüfter kann mithilfe des Knopfes auf dem Breadboard (9) angeschaltet werden und unterstützt die Kühlung des Heatblocks bei Bedarf.

**4. Spule:** Die Spule wird mithilfe des Motors (7) angetrieben und wickelt den fertigen Filament-Streifen auf. Durch diesen Mechanismus erfolgt die Schmelzung des Filaments autonom. Die Spule zieht den Filament-Streifen aus dem Heatblock heraus.

**5. Arduino:** Der Arduino ist hier mit einem Motorshield ausgestattet und nimmt den Strom von einem externen Labornetzteil.

**6. Filament cutter:** Diese Vorrichtung ermöglicht es, die PET-Flasche in einen Streifen zu schneiden und dabei bleibt der Streifen immer gleichmässig breit.

**7. Motor:** Der Motor treibt die Spule an und wurde so programmiert, dass er sich an die Temperatur des heatblocks anpasst. Dies ist daher wichtig, da sich das Filament bei tiefer Temperatur schwerer herausziehen lässt als bei einer hohen. Daher dreht der Motor schneller bei tiefer Temperatur als bei hoher.

**8. Display:** Das Display Zeigt den gemessenen Widerstand vom Temperaturmesser an, welcher in den Heatblock (2) integriert ist. Aktuell wird jedoch erst ein Widerstands-Wert angezeigt, dies muss noch mit der richtigen Temperatur gewechselt werden.

**9. Breadboard:** Das Breadboard enthält die vollständige Elektronik, dieses ist jedoch nur temporär da und wird noch durch eine Platine ausgetauscht.


WICHTIG: Das Projekt auf dem Bild stellt nur unsere Ausführung dar für ein Informatikprojekt mit relativ wenig verfügbarer Zeit und Ressourcen. Das Projekt kann auch noch stetig verbessert werden und Ansätze zur Lösung von Problemen könnten auch anders sein.

## Codes fürs Modellieren und Arduino 

Zum modellieren wurde ein CAD Programm namens OpenSCAD (https://openscad.org) genutzt, der Code zur gesamten Spule (siehe Bild oben) kann hier auf Github unter https://github.com/EricPernet/Filament-converter/blob/main/Spule%20OpenSCAD gefunden werden. Als Microcontroller wurde ein Arduino uno (https://www.arduino.cc) benutzt, der gesamte Code dazu kann ebenfalls auf Github unter https://github.com/EricPernet/Filament-converter/blob/main/Arduino%20PET%20to%20filament%20converter gefunden werden. 

Für den OpenSCAD Code wird eine Library namens getriebe.scad benötigt, diese ist auf Thingiverse verfügbar: 

https://www.thingiverse.com/thing:1604369

Für den Arduino Code wird ebenfalls eine Library benötigt:

https://www.arduino.cc/reference/en/libraries/ht16k33/


## Dokumentation zum Projekt

Eine vollständige Dokumentation der Arbeitsschritte und ein Fazit von unserem persönlichen Projekt ist in diesem PDF Dokument enthalten: https://github.com/EricPernet/Filament-converter/blob/main/diy_pet_flaschen_zu_filament_converter_efraim_und_eric.pdf


## Teile, die im Projekt enthalten sind

**Heatblock:**https://de.aliexpress.com/item/32902780945.html?spm=a2g0o.detail.1000014.22.68353f3etGCuNz&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.40000.267768.0&scm_id=1007.40000.267768.0&scm-url=1007.40000.267768.0&pvid=10ce223b-449c-4e80-98b3-86e08aba30e1&_t=gps-id%3ApcDetailBottomMoreOtherSeller%2Cscm-url%3A1007.40000.267768.0%2Cpvid%3A10ce223b-449c-4e80-98b3-86e08aba30e1%2Ctpp_buckets%3A668%232846%238110%23322&pdp_ext_f=%7B

**Nozzle:** https://de.aliexpress.com/item/1005005772823867.html?spm=a2g0o.productlist.main.1.46412130rM69h8&algo_pvid=9fbe4379-e494-4034-8c4c-f0dfec1b8216&algo_exp_id=9fbe4379-e494-4034-8c4c-f0dfec1b8216-0&pdp_npi=4%40dis%21CHF%213.60%210.44%21%21%2128.87%21%21%402103011217001396470721642e0df6%2112000034367533471%21sea%21CH%210%21AB&curPageLogUid=m0TIKRMCpsHY

**Digital Display:** https://store.arduino.cc/collections/displays/products/grove-4-digit-display


## Weitere Tutorials und Anleitungen zu verschiedenen Teilen des Projekts

**Tutorial PET to Filament converter:** https://www.youtube.com/watch?v=ueJXQ7appC0

**PET bottle cutter:** https://www.youtube.com/watch?v=QyOKVBeIQ5w











