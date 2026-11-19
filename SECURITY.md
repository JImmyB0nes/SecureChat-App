# Sicherheitshinweise

Enigma 3 ist Ende-zu-Ende verschlüsselt. Was das heißt und wo die Grenzen
liegen, steht im Sicherheitsmodell des Server-Repositories:

<https://git.jimmybones.de/jimmybones/securechat>

## Vertraulich melden

Bitte melde Sicherheitslücken **nicht öffentlich** über ein Issue. Nutze
einen der Wege:

- **E-Mail:** `security@jimmybones.de`
- **Verschlüsselt:** bitte einen Hinweis schicken, dann senden wir
  Public-Key und Fingerabdruck zu.

Wir bestätigen den Eingang innerhalb von 72 Stunden und liefern eine
Einordnung, spätestens nach 14 Tagen.

## Was wir als Lücke ansehen

- Alles, was die Ende-zu-Ende-Verschlüsselung umgeht oder entwertet.
- Schlüsselzugriff über die App (Tresor, Keystore, DPAPI, PIN-Umkreisung).
- Update-Pfad: Signaturprüfung, Prüfsummen, Manifest.
- Gerätebindung, die sich unbemerkt unterlaufen lässt.
- Remote ausnutzbare Fehler in der Web-View oder im Capacitor-Layer.

## Was wir nicht als Lücke ansehen

- Angriffe, für die bereits physischer Zugriff auf dein entsperrtes
  Gerät nötig ist.
- Kopien auf Empfängergeräten (Screenshots, Downloads).
- Warnungen von Virenscannern gegen den unsignierten Installer.
- Abhängigkeiten, die nur bei bereits kompromittierter Maschine zählen.

Im Zweifel: lieber einmal mehr melden.

## Updates

Updates laufen über die Desktop-App oder dieses Repository. Die App prüft
jede Version gegen eine eingebaute Ed25519-Signatur und die SHA-256-Prüfsumme
der Datei. Beides steht im Release.
