# LaTeX Installation unter macOS

## Installation per Paketverwaltung

Bei Verwendung einer [Paketverwaltung](./ZZ_Paketverwaltungen_macOS.md) kann LaTeX unter dem Paketnamen `texlive` installiert werden.
Da es sich hierbei um eine Software ohne graphische Oberfläche handelt, lautet der exakte Befehl zum installieren:
```shell
brew install texlive
```

Wird eine graphische Oberfläche zur Entwicklung von LaTeX-Dokumenten gewünscht, kann eine solche über den folgenden Befehl installiert werden:
```shell
brew install --cask texstudio
```

## Installation per Hand

Die händische Installation erscheint zunächst einfacher, führt aber dazu, dass spätere Updates ebenfalls manuell eingespielt werden müssen. Für die händische Installation können die Pakete von der [Homepage von Texlive](https://www.tug.org/texlive/windows.html#install) heruntergeladen und installiert werden.
Das gleiche gilt für [TeXstudio](https://www.texstudio.org/#download).
