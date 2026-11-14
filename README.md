<div align="center">

<img src="https://img.shields.io/badge/Enigma_3-1.7.24-1f6feb?style=for-the-badge&labelColor=0d1117&logo=github&logoColor=white" alt="Version 1.7.24" />
<img src="https://img.shields.io/badge/Ende--zu--Ende-verschl%C3%BCsselt-1a7f37?style=for-the-badge&logo=lock&logoColor=white" alt="Ende-zu-Ende-verschlüsselt" />
<img src="https://img.shields.io/badge/Windows·Linux·Android-303030?style=for-the-badge" alt="Plattformen" />

# Enigma 3

**Deine Nachrichten. Dein Server. Niemand sonst.**

Die App zum selbst gehosteten SecureChat-Server: Ende-zu-Ende verschlüsselte
Nachrichten, Anrufe und gemeinsame Räume — auf deiner eigenen Hardware,
nicht bei einem Konzern.

<br/>

[**⬇ JETZT HERUNTERLADEN**](https://github.com/JImmyB0nes/SecureChat-App/releases/latest)

</div>

---

## 📦 Downloads

Alle Downloads sind im neuesten Release dieses Repositories.

| Plattform | Datei | Startklar mit |
| :--- | :--- | :--- |
| 🪟 Windows 10/11 (x64) | `Enigma-3-Setup-<Version>.exe` | Ausführen. Ersetzt Vorversionen, behält alle Daten. |
| 🐧 Linux x86_64 | `Enigma-3-<Version>-x86_64.AppImage` | `chmod +x` — dann doppelklicken. |
| 🐧 Linux arm64 | `Enigma-3-<Version>-arm64.AppImage` | `chmod +x` — dann doppelklicken. |
| 🤖 Android 7+ | `Enigma-3-<Version>.apk` | Signierte Release-APK (`CN=Enigma 3`). |

🔐 Prüfsummen aller Dateien: [`SHA256SUMS.txt`](https://github.com/JImmyB0nes/SecureChat-App/releases/latest/download/SHA256SUMS.txt)

> **Empfehlung:** Immer direkt auf die neueste Version aktualisieren.
> Ältere Releases bleiben zum Nachlesen erhalten, sind aber nicht mehr
> empfohlen.

---

## ⚡ In drei Schritten loslegen

```text
1. Server   →  Ein laufender SecureChat-Server mit HTTPS.
2. App      →  Unten herunterladen und installieren.
3. Starten  →  Serveradresse eintragen, anmelden, loslegen.
```

<details>
<summary><b>Details &amp; häufige Fälle</b></summary>

- **Windows:** Der Installer ist unsigniert. SmartScreen zeigt einen Hinweis —
  nur bestätigen, wenn diese Seite die Quelle war.
- **Android:** Eine vorhandene Debug-APK vorher deinstallieren, der
  Release-Schlüssel ist ein anderer. Installation über „Unbekannte Quellen".
- **iPhone:** Wird nicht als App verteilt. Nutze die Web-App im Safari.
- **Upgrades:** Neue Version einfach über die bestehende installieren. Es
  bleiben alle Sitzungen, Einstellungen und Schlüssel erhalten.
- **Erster Start nach einem größeren Update:** Ab Version 1.7.24 ist die PIN
  8-stellig und am Desktop Pflicht. Bestehende Tresore mit alter PIN entsperren
  weiter; beim nächsten Mal bitte die neue Länge setzen.

</details>

---

## 🛡️ Was die App schützt

<table>
<tr>
<td width="50%">

### 🔒 Ende-zu-Ende
Dein Gerät verschlüsselt die Nachricht, bevor sie das Haus verlässt.
Der Server überträgt und speichert, was er nicht lesen kann.

### 🔁 Vorwärtsgeheimheit
Jede Nachricht hat einen eigenen Schlüssel. Ein verlorener Schlüssel
legt deine Vergangenheit nicht offen.

</td>
<td width="50%">

### 📱 Gerätesperre
Biometrie oder eine 8-stellige PIN versiegeln die Schlüssel im lokalen
Tresor (Argon2id mit Gerätegeheimnis als Pepper). Android nutzt den Keystore,
Windows DPAPI.

### ⏳ Selbstlöschung
Du entscheidest, wie lange deine Nachrichten bleiben —
auf dem Server und auf jedem Gerät.

</td>
</tr>
</table>

Kein Tracking. Kein Crash-Reporting. Kein Hintergrund-Download.
Updates kommen ausschließlich aus diesem Repository.

---

## 🔍 Integrität prüfen

```sh
sha256sum -c SHA256SUMS.txt
```

**Automatische Updates:** Die Desktop-App prüft jedes Update gegen zwei
Sicherheitsstufen:

1. Eine **Ed25519-Signatur** (`update-manifest.json` und `update-manifest.json.sig`
   im Release). Die App hat den Absendeschlüssel eingebaut.
2. Die **SHA-256-Prüfsumme** jeder Datei.

Ohne passende Signatur bietet die App kein Update an.

---

## 💬 Kontakt

Fragen, Fehler und Sicherheitshinweise:
[**GitHub Issues**](https://github.com/JImmyB0nes/SecureChat-App/issues)
