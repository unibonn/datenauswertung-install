# Python/Matplotlib Installation unter Linux

Bei den meisten Linux-Systemen kommen vorinstallierte Python(3)-Module bei der OS-Installation mit.
Zum Aufsetzen einer virtuellen Umgebung, in die dann Matplotlib installiert werden kann, genügt in den meisten Fällen (`<name-meiner-umgebung>` ist dabei ein beliebig wählbarer Name für die Umgebung):
```shell
python3 -m venv <name-meiner-umgebung>
```

Falls dabei eine Fehlermeldung angezeigt wird, dass z.B. das Paket `python3.10-venv` zunächst installiert werden muss, so muss dies zuerst wie in der Meldung beschrieben nachgeholt werden.

Sobald diese Umgebung erstellt ist, kann man sie starten bzw. in die Umgebung wechseln, indem man den folgenden Befehl ausführt:
```shell
source <name-meiner-umgebung>/bin/activate
```

Danach kann Matplotlib über den bereits beschrieben Weg installiert werden:
```shell
pip install matplotlib
```
An dieser Stelle werden häufig Warnungen von `pip` ausgegeben, dass die Version von `pip` selber nicht mehr aktuell ist.
Auch wenn es generell empfehlenswert ist, `pip` aktuell zu halten, wird diese Warnung häufiger erscheinen, weil es sehr regelmäßige neue Updates dafür gibt.
Diese Warnung kann also durchaus auch für einige Zeit ignoriert werden.

Um die Arbeit zu einem späteren Zeitpunkt wieder aufzunehmen, genügt es, wieder in die erstellte Umgebung zu wechseln.
Matplotlib steht dann automatisch wieder zur Verfügung.
