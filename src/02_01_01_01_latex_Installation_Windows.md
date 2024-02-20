# LaTeX Installation unter Windows

## Installation per Paketverwaltung

Nach [Einrichtung einer Paketverwaltung](./ZZ_Paketverwaltungen_Windows.md) lässt sich LaTeX mit Hilfe dieser installieren.
Für die Variante ohne graphische Oberfläche lautet der Paketname unter Chocolatey `texlive`.
Da einige sehr hilfreiche Erweiterungen nicht in der Basisversion mitgeliefert werden, ändert sich der empfohlene Installationsbefehl etwas ab:
```shell
choco install texlive --params="'/collections:latex,latexrecommended,langgerman,bibtexextra,latexextra /scheme:full'"
```
Damit diese Paketerweiterungen bei späteren Updates über Chocolatey mitbedacht werden, muss die Konfiguration für Chocolatey angepasst werden.
Dazu genügt das einmalige Ausführen des folgenden Befehls:
```shell
choco feature enable -n=useRememberedArgumentsForUpgrades
```
Als Variante mit graphischer Oberfläche empfiehlt sich TeXstudio.
Es gibt noch weitere Frameworks, die eine graphische Oberfläche zur Entwicklung von LaTeX-Dokumenten bieten, an dieser Stelle soll sich aber auf TeXstudio konzentriert werden.
Der Paketname hierfür lautet unter Chocolatey `texstudio`.
In diesem Fall kann der gewohnte Installationsbefehl benutzt werden.


Unter Winget lassen sich nur Frameworks mit graphischer Oberfläche installieren, entsprechend wird hier nur das Beispiel TeXstudio behandelt.
Der Installationsbefehl weicht leicht von der üblichen, leicht kürzeren, Syntax ab:
```shell
winget install -e --id TeXstudio.TeXstudio
```


## Installation per Hand

Die händische Installation erscheint zunächst einfacher, führt aber dazu, dass spätere Updates ebenfalls manuell eingespielt werden müssen. Für die händische Installation können die Pakete von der [Homepage von Texlive](https://www.tug.org/texlive/windows.html#install) heruntergeladen und installiert werden.
Das gleiche gilt für [TeXstudio](https://www.texstudio.org/#download).
