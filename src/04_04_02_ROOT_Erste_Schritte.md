# Erste Schritte

Das ROOT-Team stellt eine breite Auswahl an Ressourcen zur Einarbeitung in ROOT zur Verfügung, siehe [hier](https://root.cern/get_started/).
Dabei gibt es [allgemeine Hinweise](https://root.cern/primer/) zu ersten Schritten sowie [Tutorials](https://indico.cern.ch/event/395198/) inklusive Videos und Tutorials mit vorgefertigten [Code-Beispielen](https://root.cern/tutorials/).

## Allgemeine Hinweise

Die aktuellen ROOT-Versionen 6.26/xx leiden noch an einigen Kinderkrankheiten, die die Auswertung erschweren können. Falls eine solche Version installiert wurde, empfehlen wir aktuell, mit folgendem Kommando den TBrowser wieder in den "klassischen" Modus zurückzukonfigurieren:
```bash
echo "Browser.Name: TRootBrowser" >> ~/.rootrc
```
Die Probleme sind ab Version 6.28/00 gelöst, unter Windows empfiehlt sich aufgrund der grafischen Darstellung aber dennoch die vorstehende Konfiguration.

## Windows-spezifische Hinweise

Bei der Verwendung von Windows kann es manchmal zu Problemen bei der Darstellung von grafischen Elementen kommen.
Diese lassen sich häufig durch ein Update des Grafikkartentreibers beheben.

## Linux-spezifische Hinweise

Der Vollständigkeit halber sei erwähnt, dass theoretisch auch eine Installation per Snap möglich ist. Dabei ist aber das Laufenlassen eigener Software (wie des im Versuchs entwickelten Analyse-Codes) mit der root-Version aus dem Snap deutlich komplizierter.

## macOS-spezifische Hinweise

Bei der späteren Auswertung muss auf macOS Systemen das Makefile leicht angepasst werden. Hier muss die Option:
```
-Wl,--no-as-needed
```
entfernt werden, die auf Ubuntu-Systemen benötigt (und auf anderen Systemen ignoriert) wird, aber auf macOS zwar nicht benötigt ist, allerdings zu einer Fehlermeldung führt.

