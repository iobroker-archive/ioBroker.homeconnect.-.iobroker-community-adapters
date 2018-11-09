![Logo](admin/homeconnect.png)
# ioBroker.homeconnect
=================



## Voraussetzungen vor der Installation

Es muß mindestens Node.js Version 6 installiert sein!!

Für den Adapter wird eine ClientID benötigt. Dazu muss man sich ersteinmal im Developer-Portal von Home-Connect registrieren.

https://developer.home-connect.com

![Screenshot](img/registrierung1.JPG)

Bei **Default Home Connect User Account for Testing** die E-Mail-Adresse angeben, mit der die Home-Connect-App
registriert wurde, diese wird später auch beim Authorization-Prozess benötigt.

![Screenshot](img/registrierung2.JPG)

Bei **Account Type** Individual auswählen. Die restlichen Daten sofern vorhanden ergänzen (keine Ahnung, ob das geprüft wird)

![Screenshot](img/application1.JPG)

Dann auf **Applications** und anschließend auf **Register Application** gehen.

![Screenshot](img/application2.JPG)

Bei **Application ID** einen Namen für die Application eintragen, z.B. ioBroker. Bei **OAuth Flow** Device Flow selektieren das 
letzte Feld kann leer bleiben. Dann Speichern und dann hat man die benötigte ClientID.



##  Konfiguration

In der Adapter-Config muss nur die ClientID eingetragen werden. Wenn der Adapter läuft, wird eine Authorization-URL generiert, diese wird im 
Log angezeigt. Die URL einfach kopieren und im Browser öffnen. Dann die Logindaten vom Home-Connect-Account (nicht vom Developer-Account) eingeben und bestätigen. Dann die Authorisierung bestätigen. Fertig.





## Changelog

### 0.0.2  (08.11.2018)

* (dna909) OAuth2 Deviceflow-Authorization, enumerate connected appliances

### 0.0.1

* (dna909) initial release

## License
The MIT License (MIT)

Copyright (c) 2018 dna909 <dna909@googlemail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
