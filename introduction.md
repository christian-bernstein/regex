# Einführung reguläre Ausdrücke

## Cheatsheet


| Ausdruck | Beschreibung |
| :--- | ---: |
| .	| any character except newline |
| \w \d \s | word, digit, whitespace |	
| \W \D \S | not word, digit, whitespace |
| [abc] |	any of a, b, or c |
| [^abc] |	not a, b, or c |
| [a-g] [0-9] |	character between a & g, between 0 & 9 | 
| ^abc$ | start / end of the string |
| \\\. \\\* \\\\ | 	escaped special characters |
| (abc) | 	capture group |
| a* a+ a? | 0 or more, 1 or more, 0 or 1 |
| a{5} a{2,} | exactly five, two or more |
| a{1,3} | between one & three |
| ab\|cd |	match ab or cd |
###### Informationen von der Website [Regexr](https://regexr.com/)

## Regulärer Ausdruck für Benutzernamen
Entwickele einen regulären Ausdruck, der Benutzernamen erkennen kann. 
Ein Benutzername ist dann korrekt, wenn er keine Leerzeichen & Sonderzeichen enthält, mindestens 3 Zeichen lang & maximal 16 zeichen lang ist.
Alle hier aufgelisteten Benutzernamen müssen von deinem regulären Ausdruck gleichzeigig erfasst werden.
```
Max
Max_Mustermann
Max-2022
Max.Mustermann
Aysegül
```

Alle hier aufgelisteten Benutzernamen müssen von deinem regulären Ausdruck als inkorrekt erfasst werden (Dürfen im Editor nicht markiert werden).
```
M
Max_Mustermanns_zu_langer_Benutzername
Max Mustermann
```

## Regulärer Ausdruck für Email-Adressen
Entwickle einen regulären Ausdruck, der einfache Email-Adressen erkennen kann. 
Alle hier aufgelisteten Adressen müssen von deinem regulären Ausdruck gleichzeigig erfasst werden.

```
max-mustermann@gmail.com
Max@max-mustermann.de
max_mustermann@max-mustermann.de
max.mustermann@gmail.fr
```
**Zusatz:** Top Level Domains (de, com, uk, fr, net etc.) müssen mindestens zwei Zeichen lang sein. Beachte diese Limitierung bei deinem regulären Ausdruck.
