---
name: "menschlich"
description: Überarbeitet KI-generierte Texte (von Claude, ChatGPT usw.) so, dass sie wieder menschlich klingen, gestützt auf die Muster aus dem Wikipedia-Leitfaden "Signs of AI writing" (Stand Oktober 2026). Verwende diesen Skill immer, wenn der Nutzer "menschlich", "/menschlich", "humanisieren", "klingt nach KI", "klingt nach ChatGPT", "weniger KI-Sound", "natürlicher formulieren" oder "entschwurbeln" sagt, oder wenn er einen Text (E-Mail, Offerte, Brief, Blogpost, LinkedIn-Post, Website-Text, Bericht) überarbeitet haben will, damit er nicht maschinell wirkt. Auch verwenden, wenn ein neuer Text ausdrücklich natürlich und unaufgeregt geschrieben werden soll. Gilt für Deutsch und Englisch ("humanize", "sounds like AI", "make it sound human", "de-AI this").
---

# Menschlich

Ziel ist ein Text, der klingt, als hätte ihn eine sachkundige Person in Ruhe geschrieben: konkret, direkt, ohne Aufblähung. Ziel ist nicht, KI-Detektoren zu überlisten.

## Grundhaltung

Der Wikipedia-Leitfaden erklärt den Kern so: Sprachmodelle tendieren zum statistischen Mittelwert. Seltene, spezifische Fakten werden durch häufige, allgemeine und positive Formulierungen ersetzt. Aus "erfand die erste automatische Wagenkupplung" wird "ein revolutionärer Pionier der Industrie". Der Text wird gleichzeitig unschärfer und lauter.

Daraus folgt die wichtigste Regel dieses Skills: **Spezifität zurückholen.** Wörter auszutauschen reicht nicht; der Leitfaden warnt ausdrücklich, dass das Bekämpfen der Oberflächenmerkmale die eigentlichen Probleme nur versteckt. Deshalb gilt die Reihenfolge: zuerst Inhalt, dann Sprache, dann Form.

Menschlicher Text hat ausserdem Merkmale, die KI-Text meidet (Abschnitt F in `references/muster.md`): einfache "ist"- und "hat"-Sätze, schlichte statt gestelzter Wörter, klare Superlative ("der erste", "der einzige"), kleine Verstärker und Abschwächer ("sehr", "wohl", "eher"), gelegentlich eine umständliche Wendung. Ein menschlicher Text ist auch in der Zeichensetzung ungleichmässig: mal ein Doppelpunkt, mal eine Klammer, mal ein Semikolon, mal ein langer Satz mit drei Kommas.

## Ablauf

1. **Kontext erfassen.** Wer liest den Text, über welchen Kanal, in welcher Sprache? Wenn das aus dem Gespräch hervorgeht, nicht nachfragen.
2. **Inhalt prüfen** (Abschnitt A). Aufgeblasene Bedeutung, Werbesprache, Partizip-Anhängsel, vage "im Zusammenhang mit"-Verbindungen, vage Quellen, Absicherungs-Floskeln. Streichen oder durch Konkretes ersetzen.
3. **Sprache prüfen** (Abschnitt B). KI-Vokabular, die drei Varianten des negativen Parallelismus, Dreierreihen, "dient als" statt "ist".
4. **Rhythmus und Zeichensetzung prüfen** (Abschnitt C). Gedankenstriche, aber auch das Gegenteil: lauter gleich lange Sätze mit nur Punkt und Komma.
5. **Form prüfen** (Abschnitt D). Fettdruck, Listen mit fetten Mini-Titeln, Titel-Grossschreibung, "X und Y"-Überschriften, Mini-Tabellen, Emojis, Schlusszusammenfassung.
6. **Chatbot-Reste entfernen** (Abschnitt E). "Gerne!", "Ich hoffe, das hilft", Rückfragen, Platzhalter, Hinweise auf fehlende Quellen.
7. **Laut-Lese-Test.** Würde eine Fachperson das so sagen? Wo klingt es nach Broschüre oder nach Pressemitteilung? Dort nochmals ran.
8. **Ausgabe.** Den überarbeiteten Text liefern, ohne Einleitung. Danach höchstens zwei, drei Sätze, und nur wenn sie dem Nutzer etwas bringen: etwa dass ein Absatz gestrichen wurde, weil er nichts aussagte, oder dass eine Zahl fehlt. Keine Selbstbeschreibung im KI-Stil ("Ich habe den Text gestrafft, die Klarheit verbessert und den Kern beibehalten"); genau diese Sorte Änderungsnotiz führt der Leitfaden als eigenes KI-Merkmal auf.

Für kurze Texte (eine E-Mail, ein Absatz) reicht ein Durchgang mit der Kurzfassung unten. `references/muster.md` lesen, sobald der Text länger ist oder viele Muster enthält.

## Kurzfassung der wichtigsten Regeln

- Bedeutung zeigen statt behaupten. "spielt eine entscheidende Rolle", "ist ein Meilenstein", "unterstreicht die Bedeutung", "Diese Unterscheidung ist wichtig, weil" streichen; stattdessen sagen, was konkret passiert.
- Beziehungen direkt benennen. Nicht "steht im Zusammenhang mit der Geschäftsleitung", sondern "war CEO".
- Keine Werbeadjektive ohne Beleg: "innovativ", "nahtlos", "ganzheitlich", "massgeschneidert", "vielfältig", "beeindruckend", "Engagement für".
- Keinen der drei Kontraste als Reflex: "nicht nur X, sondern auch Y", "nicht X, sondern Y", "Y statt X".
- Dreierreihen aufbrechen. Zwei oder vier Punkte sind genauso legitim.
- "ist", "hat", "gibt es" statt "dient als", "fungiert als", "verfügt über", "bietet", "zeichnet sich aus durch".
- Schlichte Wörter: "schrieb" statt "verfasste", "nutzte" statt "setzte ein", "zog um" statt "verlegte seinen Wohnsitz".
- Keine Gedankenstriche als Stilmittel; ersetzen durch Doppelpunkt, Klammer, Semikolon oder einen neuen Satz. Nicht alles in Punkt und Komma auflösen, sonst entsteht das neuere KI-Muster der gleichförmigen Kurzsätze.
- Satzlängen mischen. Kein Text, in dem jeder Satz 8 bis 20 Wörter hat.
- Keine Absicherungs-Floskeln ("sollte eher als ... verstanden werden", "lässt sich daraus nicht ableiten", "auf Basis der verfügbaren Informationen").
- Vage Quellen ("Experten sind sich einig", "Studien zeigen") konkret benennen oder streichen.
- Fettdruck sparsam; Fliesstext statt Aufzählung, wenn die Punkte zusammenhängen.
- Kein Schlusssatz, der das Gesagte wiederholt.
- Keine Chatbot-Höflichkeit am Anfang oder Ende.

## Was nicht tun

- **Keine Fakten erfinden**, um Vages konkret zu machen. Fehlt eine Zahl oder ein Name, die Stelle streichen oder als `[Zahl ergänzen]` markieren und am Ende kurz darauf hinweisen.
- **Nicht übertreiben.** Keine eingebauten Tippfehler, kein gespielter Slang, keine künstliche Lockerheit. Menschlich heisst nicht nachlässig.
- **Keine Hexenjagd auf Einzelwörter.** Der Leitfaden nennt ausdrücklich unwirksame Indikatoren: perfekte Grammatik, formeller oder akademischer Ton, gemischte Register, einzelne Übergangswörter. Diese nicht "korrigieren". Es zählt die Häufung.
- **Synonyme nicht pauschal verbannen.** Dass ein Modell "underscore" überstrapaziert, heisst nicht, dass "betonen" verdächtig ist.
- **Bedeutung nicht verändern.** Aussagen, Zusagen, Preise, Termine bleiben exakt.
- **Den Ton des Kanals respektieren.** Eine Offerte bleibt sachlich, ein LinkedIn-Post darf persönlicher sein.
- **Menschliche Passagen in Ruhe lassen.** Bei gemischten Texten nur die maschinell klingenden Stellen anfassen. Ein plötzlicher Stilbruch innerhalb eines Textes ist selbst ein Merkmal.

## Deutsch und Schweizer Schreibweise

Bei deutschen Texten für die Schweiz: "ss" statt "ß", echte Umlaute (ä, ö, ü). Anführungszeichen einheitlich halten, so wie im Dokument oder beim Absender üblich. Der Wikipedia-Leitfaden beschreibt nur Englisch; die deutschen Entsprechungen in `references/muster.md` sind sinngemässe Übertragungen und Erfahrungswerte, keine belegten Wortlisten.

## Beispiel

Vorher:
> In der heutigen dynamischen Geschäftswelt spielt Künstliche Intelligenz eine entscheidende Rolle. Unsere innovative Lösung bietet nicht nur Effizienz, sondern auch Sicherheit und Skalierbarkeit – und unterstreicht damit unser Engagement für nachhaltige Digitalisierung. Zusammenfassend lässt sich sagen, dass KI die Zukunft ist.

Nachher:
> Unser System liest eingehende Rechnungen aus und legt sie direkt als Kreditor im ERP an. Bei einem Kunden mit rund 400 Rechnungen pro Monat spart das etwa zwei Arbeitstage (gemessen über drei Monate).

Der zweite Text ist kürzer, weil der erste fast nichts sagte. Die Zahlen im Beispiel sind fiktiv; in der Praxis nur Zahlen verwenden, die vorliegen.
