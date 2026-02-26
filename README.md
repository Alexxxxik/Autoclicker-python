Autoclicker Python - ReadME
Beschrijving
Dit is een eenvoudige Python autoclicker die de linker muisknop automatisch ingedrukt houdt wanneer je de zijknop (X2) van je muis ingedrukt houdt.

Functionaliteit
Automatisch klikken: Drukt de linker muisknop herhaaldelijk in met een interval van 3 milliseconden
Muisluisteraar: Luistert naar muisknoppen, specifiek naar de zijknop (X2)
Threading: Gebruikt threading om klikken in de achtergrond uit te voeren zonder het hoofdprogramma vast te zetten

Vereisten
bash
pip install pynput

Hoe te gebruiken
Installeer de vereiste bibliotheek: pynput

Voer het script uit:
bash
python autoclicker.py

Houd de zijknop (X2) van je muis ingedrukt om te beginnen met automatisch klikken
Laat de knop los om te stoppen

Code Uitleg
Component	Beschrijving
mouse_controller	Bestuurt de muisbewegingen en klikken
clicking	Globale variabele om de clickstatus bij te houden
click_loop()	Functie die herhaaldelijk klikt terwijl clicking True is
on_click()	Callback-functie die geactiveerd wordt wanneer er op een muisknop wordt geklikt
mouse.Listener	Luistert naar muisgebeurtenissen
Aanpassingen
Kliksnelheid wijzigen: Verander time.sleep(0.003) naar een ander getal (in seconden). Lager = sneller klikken.
