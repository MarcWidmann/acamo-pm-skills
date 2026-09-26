# acamo PM Skills

Neun einsatzfertige KI-Bausteine für die Projekt- und Führungspraxis, erprobt in den
Seminaren und Workshops von [acamo](https://acamo.com).

Kein Tool, kein Login, keine Plattformbindung. Jeder Baustein ist ein Skill im offenen
Agent-Skills-Format: eine `SKILL.md` mit Anweisungen in Markdown. Das läuft in Claude, in
ChatGPT und per Copy-Paste in jedem anderen Chatfenster.

## Die Skills

| Skill | Was er leistet |
|---|---|
| [`entscheidungsfindung-wrap`](entscheidungsfindung-wrap/) | Führt eine schwierige Entscheidung strukturiert durch den WRAP-Prozess nach Chip und Dan Heath. Für Go/No-Go, Priorisierung, Investitionen, Besetzungsfragen. |
| [`meeting-protokoll`](meeting-protokoll/) | Macht aus einem Transkript ein belastbares Protokoll: Entscheidungen, Aufgaben mit Verantwortlichen, Risiken, und auf Wunsch eine Analyse der Teamdynamik. |
| [`belbin-teamrollen`](belbin-teamrollen/) | Interaktive Selbsteinschätzung zu den neun Teamrollen, zweisprachig Deutsch und Englisch. Ideal als Einstieg in einen Teamworkshop. |
| [`interview-case`](interview-case/) | Erzeugt eine realistische 30-Minuten-Fallstudie für Auswahlgespräche, samt Bewertungsraster mit beschriebenen Ankerpunkten. |
| [`kommunikationstest-4-ohren`](kommunikationstest-4-ohren/) | Selbsttest nach dem 4-Ohren-Modell von Schulz von Thun: Auf welchem Ohr hören Sie zuerst? |
| [`meeting-agenda`](meeting-agenda/) | Entwickelt im Dialog eine Agenda, die auf Ergebnisse gebaut ist statt auf Themen. Präsenz, virtuell oder hybrid. |
| [`risikoregister`](risikoregister/) | Erstellt aus einem Projekt-Factsheet ein Risikoregister mit Eintrittswahrscheinlichkeit, Schaden, Erwartungswert, Frühindikatoren und Maßnahmen. |
| [`praesentation-scqa`](praesentation-scqa/) | Baut aus vorhandenem Material eine entscheidungsreife Präsentation in acht Folien nach SCQA und Pyramidenprinzip, samt Sprechernotizen. |
| [`prompt-of-prompts`](prompt-of-prompts/) | Entwickelt im Dialog einen wirksamen Prompt oder verbessert einen vorhandenen. Der Baustein, mit dem die anderen entstanden sind. |

## So setzen Sie sie ein

**Claude.** Skills lassen sich in der Weboberfläche hochladen, in Claude Code direkt aus
diesem Repository installieren und über die API hinterlegen.

**ChatGPT.** Skills sind der Instruktionsteil eines Plugins. Wer kein Plugin bauen will,
kopiert den Text unterhalb des Frontmatters in ein Projekt oder in die
benutzerdefinierten Anweisungen.

**Alles andere** (Gemini, Copilot, Perplexity): Text unterhalb des Frontmatters kopieren
und als ersten Prompt einfügen.

Der Block zwischen den `---` am Dateianfang steuert nur, wann ein Assistent den Skill von
sich aus heranzieht. Beim manuellen Einsatz lassen Sie ihn weg.

## Warum offene Dateien statt fertiger Bots

Plattformen bauen um, Produkte verschwinden, Anbieter wechseln. Ein Prompt, der als Datei
in einem Repository liegt, überlebt das. Er ist versionierbar, in jedem Ökosystem
einsetzbar und notfalls in zehn Sekunden per Copy-Paste im Einsatz. Das Asset ist der
Prompt, nicht das Gefäß.

## Haltung

Diese Skills sind Arbeitsmittel für Menschen, die die Verantwortung behalten. Sie
ersetzen keine Führungsentscheidung, keine psychologische Diagnostik und keine
Personalauswahl. Wo ein Ergebnis personenbezogen wird, steht der passende Hinweis im
jeweiligen Skill.

Prüfen Sie vor dem Einsatz, welche Daten in welches Werkzeug gegeben werden dürfen. Für
Transkripte, Bewerbungsunterlagen und Projektdaten gilt das besonders.

## Über acamo

Marc Widmann begleitet Organisationen dabei, Projekte mit KI zu führen: als Berater,
Seminarleiter und Speaker. Mehr dazu unter
[acamo.com](https://acamo.com) und im Seminar
[Projekte mit KI führen](https://acamo.com/seminar-projekte-mit-ki-fuehren).

Fragen, Anregungen, eigene Varianten: gern als Issue oder Pull Request.
