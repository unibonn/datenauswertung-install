# Paketverwaltungen Windows

Empfohlen wird, unter Windows eine Paketverwaltung zu verwenden. Dies stellt sicher, dass Updates der installierten Anwendungen einfach und bei Bedarf auch automatisch eingespielt werden können, unabhängig von der Update-Funktionalität der Programme selbst. Außerdem wird dabei durch die Paketverwaltung sichergestellt, dass die heruntergeladenen Pakete aus zuverlässiger Quelle stammen. 

Verbreitete Paketverwaltungen unter Windows sind zunächst der eingebaute Windows Store, der allerdings nicht alle oft benötigten Programme beinhaltet. Ergänzen lässt er sich leicht etwa über [winget](https://learn.microsoft.com/de-de/windows/package-manager/winget/) oder [Chocolatey](https://chocolatey.org/). 

## Winget

Nach Einrichtung von winget durch Installation aus dem Windows-Store (siehe [Anleitung von Microsoft](https://learn.microsoft.com/de-de/windows/package-manager/winget/)) lassen sich Programme in der Kommandozeile etwa mit:
```shell
winget install <Programmname>
```
installieren. 

Als Alternative zur Kommandozeile stehen auch grafische Oberflächen für die Paketverwaltung zur Verfügung, etwa [WingetUI](https://www.marticliment.com/wingetui/).

## Chocolatey

Chocolatey selbst muss zunächst manuell wie auf der offiziellen Webseite [beschrieben](https://chocolatey.org/install#individual) installiert werden.
Der erste Schritt, das Angeben einer E-Mail-Adresse, ist dabei optional.
Danach können Programme per Kommandozeile etwa mit:
```shell
choco install <Programmname>
```
installiert werden.

Als Alternative zur Kommandozeile stehen auch grafische Oberflächen für die Paketverwaltung zur Verfügung, etwa [WingetUI](https://www.marticliment.com/wingetui/).
