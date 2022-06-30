# Belegarbeit "Programmierung I"
## Analyse Apache-Logfile

Lorem ipsum


## Quelle der Beispieldatei:

https://github.com/elastic/examples/tree/master/Common%20Data%20Formats/apache_logs

## Format der Beispieldatei laut Configuration-File:

%{IPORHOST:clientip} %{USER:ident} %{USER:auth} \[%{HTTPDATE:timestamp}\] "%{WORD:verb} %{DATA:request} HTTP/%{NUMBER:httpversion}" %{NUMBER:response:int} (?:-|%{NUMBER:bytes:int}) %{QS:referrer} %{QS:agent}