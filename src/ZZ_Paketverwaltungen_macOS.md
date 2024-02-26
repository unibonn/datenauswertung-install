# Paketverwaltungen macOS

Empfohlen wird, unter macOS eine Paketverwaltung wie [Homebrew](https://brew.sh/) oder [MacPorts](https://www.macports.org/) zu verwenden. Dies stellt sicher, dass Updates der installierten Anwendungen einfach und bei Bedarf auch automatisch eingespielt werden können, unabhängig von der Update-Funktionalität der Programme selbst. Außerdem wird dabei durch die Paketverwaltung sichergestellt, dass die heruntergeladenen Pakete aus zuverlässiger Quelle stammeb. 

## Homebrew

Zur Installation von Homebrew genügt ein Kommando, welches auf [der Homepage](https://brew.sh/) angegeben ist. Nach Installation von Homebrew können Pakete über folgendes Kommando installiert werden:
```shell
brew install --cask <Programmname>
```
Alternativ zur Kommandozeile kann auch eine grafische Oberfläche für Homebrew installiert werden, etwa [Applite](https://aerolite.dev/applite/index.html), [Cork](https://corkmac.app/) oder [Cakebrew](https://www.cakebrew.com/). 

## MacPorts

Eine alternative Paketverwaltung ist [MacPorts](https://www.macports.org/). Im Gegensatz zu Homebrew verfolgt MacPorts einen generischeren Ansatz der auch auf anderen Betriebssystemen funktioniert, was allerdings ebenfalls bedeutetet, dass es keine direkte Unterstützung für native Mac-Anwendungen bietet (bei Homebrew als "Casks" installierbar). Daher wird an dieser Stelle nicht im Detail auf MacPorts eingegangen.
