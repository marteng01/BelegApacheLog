# Belegarbeit "Programmierung I"
## Analyse Apache-Logfile

Lorem ipsum

## Notizen

### Reguläre Ausdrücke

Zeile mit einem Http-Statuscode nicht 2**:
`^.*?".*?"\s[^2][0-9]{2}\s`

Zeile mit einem Fehlercode (Http-Statuscode 4**):
`^.*?".*?"\s[4][0-9]{2}\s`

## Quelle der Beispieldatei:

https://github.com/elastic/examples/tree/master/Common%20Data%20Formats/apache_logs

## Format der Beispieldatei laut Configuration-File:

%{IPORHOST:clientip} %{USER:ident} %{USER:auth} \[%{HTTPDATE:timestamp}\] "%{WORD:verb} %{DATA:request} HTTP/%{NUMBER:httpversion}" %{NUMBER:response:int} (?:-|%{NUMBER:bytes:int}) %{QS:referrer} %{QS:agent}