# acamo PM Skills

Prompt-Bausteine für die KI-gestützte Projektführung, aus der Workshop-Praxis von
[acamo](https://acamo.com) (Marc Widmann).

Jeder Ordner ist ein eigenständiger Skill: eine `SKILL.md` mit Frontmatter und
Anweisungen in Markdown, optional ergänzt um Material im Unterordner `assets/`. Das
Format folgt der von Anthropic veröffentlichten Agent-Skills-Spezifikation. Der Inhalt
ist am Ende schlichtes Markdown und damit in jedem Werkzeug verwendbar.

## Warum ein Repository und keine Custom GPTs mehr

Diese Bausteine liefen bis zuletzt als ChatGPT Custom GPTs. OpenAI stellt Custom GPTs zum
**11. Dezember 2026** ein (Enterprise mit genehmigtem Aufschub: 11. Februar 2027);
danach sind die GPTs und ihre Seiten nicht mehr erreichbar, der Migrationspfad führt auf
Plugins.

Ein Prompt, der in einem Git-Repository liegt, überlebt solche Umbauten. Er ist
versionierbar, in beiden großen Ökosystemen verwendbar und notfalls per Copy-Paste in
jedem Chatfenster einsetzbar. Das Asset ist der Prompt, nicht das Gefäß.

## Inhalt

| Skill | Wofür |
|---|---|
| [`entscheidungsfindung-wrap`](entscheidungsfindung-wrap/) | Schwierige Entscheidung strukturiert durchdenken (WRAP nach Chip und Dan Heath) |
| [`meeting-protokoll`](meeting-protokoll/) | Transkript zu Protokoll inklusive Risiken, Aufgaben, Entscheidungen und Teamdynamik |
| [`belbin-teamrollen`](belbin-teamrollen/) | Interaktive Selbsteinschätzung zu den neun Teamrollen, DE/EN |
| [`interview-case`](interview-case/) | 30-Minuten-Fallstudie samt Bewertungsraster für Auswahlgespräche |
| [`kommunikationstest-4-ohren`](kommunikationstest-4-ohren/) | Interaktiver Selbsttest nach dem 4-Ohren-Modell (Schulz von Thun) |
| [`meeting-agenda`](meeting-agenda/) | Ergebnisorientierte Agenda im Dialog entwickeln |

## Verwendung

**Claude.** Eigene Skills lassen sich in der Weboberfläche hochladen. In Claude Code
funktioniert die Installation direkt aus einem Repository. Über die API können Skills
ebenfalls hinterlegt werden.

**ChatGPT.** Skills sind der Instruktionsteil eines Plugins, Referenzmaterial wird als
Datei angehängt. Wer kein Plugin bauen will, kopiert den Text unterhalb des Frontmatters
in ein Projekt oder in benutzerdefinierte Anweisungen.

**Alles andere** (Gemini, Copilot, Perplexity): Text unterhalb des Frontmatters kopieren
und als ersten Prompt einfügen.

Der Block zwischen den `---` am Dateianfang (`name`, `description`) steuert nur, wann ein
Assistent den Skill von sich aus heranzieht. Beim manuellen Einsatz wird er weggelassen.

## Was gegenüber den Custom GPTs geändert wurde

Die Bausteine stammen aus der Zeit von GPT-4. Beim Übertragen wurden sie an die heutige
Modellgeneration angepasst:

- **Rollen-Beschwörung reduziert.** Aufladungen wie „Act as an experienced project
  manager and organizational psychologist" bringen bei heutigen Modellen kaum noch
  Wirkung. Geblieben ist der Auftrag, weggefallen ist die Kostümierung.
- **Kontext statt Formulierungstricks.** Jeder Skill benennt jetzt ausdrücklich, welche
  Angaben und Dokumente er braucht, und fragt danach. Der Engpass ist heute fehlender
  Kontext, nicht die Wortwahl im Prompt.
- **Keine Denk-Aufforderungen.** Formeln wie „denke intensiv nach" oder „think step by
  step" sind bei Reasoning-Modellen wirkungslos und vermitteln ein falsches Bild davon,
  wie die Werkzeuge arbeiten.
- **Annahmen sichtbar.** Statt bei fehlenden Angaben stehenzubleiben, treffen die Skills
  eine Annahme und kennzeichnen sie. Das hält den Ablauf im Workshop am Laufen.
- **Grenzen benannt.** Bei den heiklen Anwendungen (Meeting-Analyse, Teamrollen,
  Kommunikationstest, Auswahlverfahren) steht jetzt ein Abschnitt zum Einsatz: was das
  Ergebnis ist, was es nicht ist, und was arbeitsrechtlich oder datenschutzrechtlich
  beachtet werden muss.
- **Zustandsführung bei interaktiven Tests.** Fortschrittsanzeige, Umgang mit ungültigen
  Eingaben, Unterbrechen und Fortsetzen.

## Offene Punkte

- `kommunikationstest-4-ohren/assets/situationen.md` ist ein Gerüst. Die zwölf
  Situationen aus dem Original-PDF müssen dort wörtlich eingesetzt werden. Sie wurden
  bewusst nicht nachgebildet, weil ein erfundener Fragebogen nicht zum Zuordnungs-
  schlüssel passen würde.
- Weitere Bausteine aus dem Workshop sind noch nicht übertragen: Konfliktgespräch,
  Risikoidentifikation, Selbstcoaching und Lernen, Statusbericht aus Jira,
  Stakeholderidentifikation, Prompt of Prompts.

## Hinweise

Alle Skills sind Arbeitsmittel für Menschen, die die Verantwortung behalten. Sie
ersetzen keine Führungsentscheidung, keine psychologische Diagnostik und keine
Personalauswahl. Wo ein Ergebnis personenbezogen wird, steht das im jeweiligen Skill.

Prüfe vor dem Einsatz, welche Daten in welches Werkzeug gegeben werden dürfen. Für
Transkripte, Bewerbungsunterlagen und Projektdaten gilt das besonders.

## Kontakt

Marc Widmann, acamo, [acamo.com](https://acamo.com)
