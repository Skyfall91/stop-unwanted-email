# Stop Unwanted Email

Ein Agent Skill, der unerwünschte E-Mails untersucht und hilft, sie beim Verursacher abzustellen.

| Worum geht es? | Passender Skill |
|---|---|
| Werbeanrufe und Betrugsversuche am Telefon | [Stop Unwanted Calls](https://github.com/Skyfall91/stop-unwanted-calls) · `stop-unwanted-calls` |
| Spam, unerwünschte Newsletter und Phishing per Mail | **Stop Unwanted Email** · `stop-unwanted-email` |

## Was der Skill macht

Der Skill wählt je nach Auftrag einen von drei getrennten Wegen:

- **Sicherer Schnellcheck:** Er vergleicht nur lokal sichtbare Metadaten seit dem letzten verlässlichen Prüfpunkt, ohne Nachrichten zu öffnen, vorzuschauen oder externe Inhalte zu laden.
- **Rein lesende Untersuchung:** Er wertet sicher verfügbare Kopfzeilen aus und trennt belegte Absender-, Versand- und Infrastrukturinformationen von bloßen Behauptungen.
- **Maßnahme an der Quelle:** Er bereitet eine verifizierte Abmeldung, einen Werbewiderspruch oder eine Meldung an den zuständigen Anbieter vor und führt externe Schritte nur mit der erforderlichen Freigabe aus.

Für rechtliche Aussagen bestimmt der Skill zuerst Nachrichtenart und Rechtsraum. Details werden nur bei Bedarf geladen und unmittelbar vor ihrer Verwendung anhand aktueller offizieller Gesetzes- oder Behördenquellen geprüft. Enthalten sind vorsichtige Routen für Deutschland/EU, das Vereinigte Königreich, die USA, Kanada und Australien.

Der Skill schützt den Zustand des Postfachs und beschränkt jede Weitergabe auf die Daten, die der verifizierte Empfänger tatsächlich benötigt. Er verspricht nicht, dass eine einzelne Maßnahme jeden zukünftigen Spam verhindert.

## Installieren

1. Lade das Repository über **Code → Download ZIP** herunter und entpacke es. Benenne den entpackten Ordner `stop-unwanted-email`. Lass `SKILL.md` und den Ordner `references` zusammen.
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

Das Repository enthält ausschließlich die Skill-Anleitung, ihre bedarfsgeladenen Referenzen, diese Erklärung und die Lizenz. Es enthält keine fallbezogenen Maildaten oder persönlichen Kontaktdaten.
