# Stop Unwanted Email

Ein Agent Skill, der unerwünschte E-Mails untersucht und hilft, sie beim Verursacher abzustellen.

| Worum geht es? | Passender Skill |
|---|---|
| Werbeanrufe und Betrugsversuche am Telefon | [Stop Unwanted Calls](https://github.com/Skyfall91/stop-unwanted-calls) · `stop-unwanted-calls` |
| Spam, unerwünschte Newsletter und Phishing per Mail | **Stop Unwanted Email** · `stop-unwanted-email` |

## Was der Skill macht

Er untersucht die technischen Kopfzeilen einer E-Mail und prüft die Absender und beteiligten Dienste. Je nach Beleglage bereitet er eine Abmeldung von einem verifizierten Verteiler, einen Werbewiderspruch oder eine Meldung an den zuständigen Anbieter vor. Dabei schützt er den Zustand deines Postfachs und beschränkt jede Weitergabe auf die Daten, die der verifizierte Empfänger benötigt.

## Installieren

1. Lade das Repository über **Code → Download ZIP** herunter und entpacke es. Benenne den entpackten Ordner `stop-unwanted-email`.
2. **Mit Agent-Skills-Unterstützung:** Füge den Ordner mit `SKILL.md` über die Skill-Verwaltung deines Assistenten hinzu. Das Repository verwendet das offene [Agent-Skills-Format](https://agentskills.io/specification).
3. **Ohne Skill-Verwaltung:** Gib dem Assistenten `SKILL.md` als Datei oder kopiere den Text in den Chat. Starte anschließend mit dem Beispiel unten.

## Ausprobieren

```text
Nutze den Skill „Stop Unwanted Email“ für diese unerwünschten E-Mails.
Finde heraus, wer hinter dem Versand steckt, und bereite die passende
Maßnahme an der Quelle vor. Lass mein Postfach unverändert.
Öffne keine Tracking- oder Abmeldelinks aus verdächtigen Nachrichten.
Sag vor dem Versand, welche meiner Daten der Empfänger sehen würde.
```

## Zugriff und Ergebnis

Der Assistent braucht Zugriff auf die technischen Kopfzeilen oder den von dir bereitgestellten Nachrichtenquelltext. Der Skill selbst enthält nur die Anleitung. Ohne freigegebenen Versandweg erstellt der Assistent einen Entwurf. Bei einer ausgeführten Aktion meldet er, was gesendet wurde und welches Ergebnis der Anbieter bestätigt hat.
