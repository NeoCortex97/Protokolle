# Protokolle

Ein Protokoll ist nur ein Dokument, das Regeln festhält um Informationen zu transportieren. Als erstes ein paar einfache Übungen um abstrakt Protokolle zu definieren:

## Notation

Als erstes ein paar Beispiele für die Notation, die ich nachfolgend zum beschreiben von Protokollen benutze.  
Zuerst ein Beispiel für Protokolle, die nur aus text bestehen.
```text
  Formale Email:

  Felder:
    Empfänger
      name
    Sender
      name
    Nachricht
      inhalt

  Hallo <Empfänger.name>,
  <Nachricht.inhalt>
  
  Lieber Gruß, <Sender.name>
```
Als nächstes möchte ich ein Beispiel geben, dass Informationen dichter packt.
```text
  DS3231 zeit lesen:

  Sekunden  - Addresse 0
    Einer              (0-3)
    Zehner             (4-6)
    Ungenutzt          (7)
  Minuten   - Addresse 1
    Einer              (0-3)
    Zehner             (4-6)
    Ungenutzt          (7)
  Stunden   - Addresse 2
    Einer              (0-3)
    Zehn               (4)
    AM/PM oder zwantig (5)
    12/24 h            (6)
    Ungenutzt          (7)
  Wochentag - Addresse 3

```
Auch, wenn eine Tabelle besser zu verstehen wäre, kann man diese Notation einfacher in Code einbetten.
