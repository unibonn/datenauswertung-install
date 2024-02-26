# Paketverwaltungen Linux

Alle üblichen Linux-Distributionen bringen von Haus aus eine Paketverwaltung mit. Diese kümmert sich darum, von den Verwaltern der Distribution gepflegte Paketversionen zu installieren und aktuell zu halten, sowie sicherzustellen, dass die heruntergeladenen Pakete aus zuverlässiger Quelle stammeb. Hierbei verwendet jede "Distributionsfamilie" eine eigene Paketverwaltung, da meist hinter den Kulissen auch andere Paketformate verwendet werden, die jeweils verschiedene Vorteile und Nachteile bieten.

Je nach Linux-Distribution entsprechen die Versionen der Pakete dabei üblicherweise nicht dem allerletzten Stand der Entwickler, sondern werden üblicherweise von der Distribution mit Sicherheitsupdates versorgt und behalten ihre Versionsnummer bis zu einem Upgrade der Linux-Distribution auf die neue Version. Der Vorteil hierbei ist, dass sich das Linux-System innerhalb einer Version der Distribution stabil verhält, was insbesondere beim Erstellen von wissenschaftlichen Arbeiten sehr hilfreich sein kann. Aus diesem Grund ist es nicht ungewöhnlich, wenn die Versionen einzelner Programme etwas älter sind.

Im Folgenden eine nicht erschöpfende Übersicht für die verbreitetsten Linux-Distributionen.

## Debian / Ubuntu / Mint / Pop! OS

Dies betrifft ebenfalls weitere davon abgeleitete Linux-Distributionen wie KUbuntu, XUbuntu etc.

Diese Distributionen nutzen `apt` für die Paketverwaltung. Pakete lassen sich etwa mit:
```shell
apt install <Programmname>
```
Üblicherweise sind für die Installation administrative Rechte nötig. Je nach Distribution muss dazu dem Kommando noch `sudo` vorangestellt werden, also:
```shell
sudo apt install <Programmname>
```
oder es muss zuerst mit `su` in eine administrative Konsole gewechselt werden:
```shell
su -
apt install <Programmname>
```
Einige der genannten Distributionen bieten auch Pakete über eine grafische Softwareverwaltunge an, etwa "Synaptic" oder einfach "Software Center". Teils werden im Software Center jedoch auch Anwendungen aus externen Quellen angeboten, was ein Sicherheitsrisiko darstellen oder Probleme beim Update der Distribution verursachen kann. 

## RedHat / CentOS / RockyLinux / AlmaLinux / Fedora Linux

Diese Distributionen nutzen `dnf` für die Paketverwaltung, in älteren Versionen auch `yum`. Darüber lassen sich Pakete mit dem Kommando:
```shell
dnf install <Programmname>
```
installieren. Üblicherweise sind hier ebenfalls administrative Rechte nötig, sodass entweder `sudo` vorangestellt oder zuerst `su -` aufgerufen werden muss, wie vorstehend für die Debian-basierten Distributionen beschrieben.

## openSUSE

openSUSE nutzt eigentlich das gleiche Paketformat wie RedHat und davon abgeleitete Distributionen, verwendet allerdings eine andere Paketverwaltung. Hier kann das Kommandozeilentool `zypper` verwendet werden, also:
```shell
apt install <Programmname>
```
Üblicherweise sind hier ebenfalls administrative Rechte nötig, sodass entweder `sudo` vorangestellt oder zuerst `su -` aufgerufen werden muss, wie vorstehend für die Debian-basierten Distributionen beschrieben.

Unter openSUSE lassen sich Programmpakete ebenfalls mit der grafischen Oberfläche "YaST Software Management" installieren.

## ArchLinux / Manjaro

Unter ArchLinux-basierenden Distributionen wird für die Paketverwaltung `pacman` verwendet. Hiermit lassen sich Pakete über das Kommando:
```shell
pacman -Syu <Programmname>
```
installieren. Üblicherweise sind hier ebenfalls administrative Rechte nötig, sodass entweder `sudo` vorangestellt oder zuerst `su -` aufgerufen werden muss, wie vorstehend für die Debian-basierten Distributionen beschrieben.

## Gentoo / Funtoo / Calculate Linux

Unter Gentoo-basierenden Distributionen wird für die Paketverwaltung `emerge` verwendet. Hiermit lassen sich Pakete über das Kommando:
```shell
emerge -av <Programmname>
```
installieren. Üblicherweise sind hier ebenfalls administrative Rechte nötig, sodass entweder `sudo` vorangestellt oder zuerst `su -` aufgerufen werden muss, wie vorstehend für die Debian-basierten Distributionen beschrieben.
