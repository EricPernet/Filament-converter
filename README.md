# Filament-converter
Informatik Projekt Eric Pernet, Efraim Sander


Dies ist das Abschlussprojekt im Grundlagenfach Informatik der Kantonsschule Kreuzlingen von Eric und Efraim (Herbstsemester 2023). Dieses Projekt beinhaltet den OpenSCAD Code für die Vorrichtung der Spule, wie auch das komplette Arduino-Skript (C++), welches komplett funktionsfähig ist. 

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


//WICHTIG: Das Projekt auf dem Bild stellt nur unsere Ausführung dar für ein Informatikprojekt mit relativ wenig verfügbarer Zeit und Ressourcen. Das Projekt kann auch noch stetig verbessert werden und Ansätze zur Lösung von Problemen könnten auch anders sein.//





