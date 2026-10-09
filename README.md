# menschlich

Ein Skill für Claude, der KI-generierte Texte so überarbeitet, dass sie wieder nach einem Menschen klingen. Er funktioniert mit Texten aus Claude, ChatGPT oder anderen Modellen, auf Deutsch und Englisch.

Grundlage ist der Wikipedia-Leitfaden [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing), den das WikiProject AI Cleanup laufend pflegt. Der Skill übersetzt dessen Muster ins Deutsche und ergänzt sie um Schweizer Schreibweise.

Es geht nicht darum, KI-Detektoren zu überlisten. Ziel ist ein Text, den eine sachkundige Person so geschrieben haben könnte: konkret, direkt und ohne Aufblähung.

## Beispiel

Vorher:

> In der heutigen dynamischen Geschäftswelt spielt Künstliche Intelligenz eine entscheidende Rolle. Unsere innovative Lösung bietet nicht nur Effizienz, sondern auch Sicherheit und Skalierbarkeit – und unterstreicht damit unser Engagement für nachhaltige Digitalisierung. Zusammenfassend lässt sich sagen, dass KI die Zukunft ist.

Nachher:

> Unser System liest eingehende Rechnungen aus und legt sie direkt als Kreditor im ERP an. Bei einem Kunden mit rund 400 Rechnungen pro Monat spart das etwa zwei Arbeitstage (gemessen über drei Monate).

Die Zahlen sind erfunden. Der Skill selbst erfindet keine Fakten: Fehlt eine Angabe, markiert er die Stelle mit `[Zahl ergänzen]`.

## Was der Skill prüft

- **Inhalt:** aufgeblasene Bedeutung, Werbesprache, vage Quellen ("Experten sind sich einig"), Absicherungs-Floskeln
- **Sprache:** typisches KI-Vokabular nach Modellgeneration, "nicht nur X, sondern auch Y", reflexartige Dreierreihen, "dient als" statt "ist"
- **Rhythmus:** Gedankenstriche, aber auch das neuere Gegenteil, also lauter gleich lange Sätze mit nur Punkt und Komma
- **Form:** Fettdruck, Listen mit fetten Mini-Titeln, Emojis, Zusammenfassungen am Schluss
- **Chatbot-Reste:** "Gerne!", "Ich hoffe, das hilft", Platzhalter

Der ganze Katalog steht in [`menschlich/references/muster.md`](menschlich/references/muster.md).

## Installation

### claude.ai und Claude Desktop

1. Unter [Releases](../../releases/latest) die Datei `menschlich.zip` herunterladen.
2. In Claude die Einstellungen öffnen und im Bereich Skills die ZIP-Datei hochladen.
3. Den Skill aktivieren.

Dafür muss in deinem Konto die Code-Ausführung eingeschaltet sein.

### Claude Code

```bash
git clone https://github.com/jobieri/menschlich-skill.git
cp -R menschlich-skill/menschlich ~/.claude/skills/
```

## Verwendung

Text einfügen und dazuschreiben: "Mach das menschlich" oder "/menschlich". Auch "klingt nach KI", "humanisieren" oder auf Englisch "humanize" lösen den Skill aus.

## Lizenz und Quelle

Der Musterkatalog beruht auf [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) (Stand Oktober 2026) von den Autorinnen und Autoren der englischsprachigen Wikipedia. Die Inhalte wurden übersetzt, gekürzt, neu gegliedert und um deutsche Entsprechungen ergänzt.

Wie das Original steht dieser Skill unter [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.de). Du darfst ihn frei nutzen, verändern und weitergeben, auch kommerziell, solange du die Quelle nennst und Bearbeitungen unter derselben Lizenz weitergibst.

Erstellt von Joerg Bieri.
