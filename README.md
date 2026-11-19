<div align="center">

<img src="docs/assets/banner-dark.jpg" alt="Enigma 3 – Secure Encryption System" width="100%" />

<br/>

[![Version](https://img.shields.io/github/v/release/JImmyB0nes/SecureChat-App?style=for-the-badge&label=Enigma%203&color=1f6feb)](https://github.com/JImmyB0nes/SecureChat-App/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/JImmyB0nes/SecureChat-App/total?style=for-the-badge&label=downloads&color=2ea043)](https://github.com/JImmyB0nes/SecureChat-App/releases)
[![Ende-zu-Ende](https://img.shields.io/badge/Ende--zu--Ende-verschl%C3%BCsselt-1a7f37?style=for-the-badge&logo=protonmail&logoColor=white)](#schutz)
[![Letztes Update](https://img.shields.io/github/release-date/JImmyB0nes/SecureChat-App?style=for-the-badge&label=last%20release)](https://github.com/JImmyB0nes/SecureChat-App/releases/latest)
[![Plattformen](https://img.shields.io/badge/Windows·Linux·Android-0d1117?style=for-the-badge)](#downloads)

# Enigma 3

**Deine Nachrichten. Dein Server. Niemand sonst.**

Die App zum selbst gehosteten **SecureChat**-Server: Ende-zu-Ende verschlüsselte
Nachrichten, Anrufe und gemeinsame Räume — auf deiner eigenen Hardware,
nicht bei einem Konzern.

<br/>

[**⬇ JETZT HERUNTERLADEN**](https://github.com/JImmyB0nes/SecureChat-App/releases/latest)  [**🔐 Prüfsummen**](https://github.com/JImmyB0nes/SecureChat-App/releases/latest)  [**🖥️ Server-Repo**](https://git.jimmybones.de/jimmybones/securechat)

<br/>

[![Windows](https://img.shields.io/badge/🪟_Windows_10/11-0078D4?style=flat-square)](#downloads)
[![Linux x64](https://img.shields.io/badge/🐧_Linux_x86__64-E95420?style=flat-square)](#downloads)
[![Linux arm64](https://img.shields.io/badge/🐧_Linux_arm64-77216F?style=flat-square)](#downloads)
[![Android](https://img.shields.io/badge/🤖_Android_7+-3DDC84?style=flat-square)](#downloads)
[![iPhone](https://img.shields.io/badge/🍎_iPhone·Web--App-333333?style=flat-square)](#iphone)

</div>

---

<details>
<summary><b>📑 Inhalt</b> — zum Aufklappen</summary>

- [📦 Downloads](#downloads)
- [⚡ In drei Schritten loslegen](#loslegen)
- [🛡️ Was die App schützt](#schutz)
- [🔍 Integrität prüfen](#integritaet)
- [📱 iPhone und Web-App](#iphone)
- [❓ Häufige Fälle](#faelle)
- [💬 Kontakt](#kontakt)

</details>

---

<a id="downloads"></a>

## 📦 Downloads

Alles im [neuesten Release](https://github.com/JImmyB0nes/SecureChat-App/releases/latest). Ein Klick auf deine Plattform bringt dich zur Datei.

| Plattform | Datei | So startest du |
| :--- | :--- | :--- |
| 🪟 **Windows 10/11** (x64) | [`Enigma-3-Setup-<Version>.exe`](https://github.com/JImmyB0nes/SecureChat-App/releases/latest) | Ausführen. Ersetzt Vorversionen, behält alle Daten. |
| 🐧 **Linux x86_64** | [`Enigma-3-<Version>-x86_64.AppImage`](https://github.com/JImmyB0nes/SecureChat-App/releases/latest) | `chmod +x` — dann doppelklicken. |
| 🐧 **Linux arm64** | [`Enigma-3-<Version>-arm64.AppImage`](https://github.com/JImmyB0nes/SecureChat-App/releases/latest) | `chmod +x` — dann doppelklicken. |
| 🤖 **Android 7+** | [`Enigma-3-<Version>.apk`](https://github.com/JImmyB0nes/SecureChat-App/releases/latest) | Signierte Release-APK (`CN=Enigma 3`). |
| 🍎 **iPhone / iPad** | — | Über die Web-App deines Servers, kein Gerätevertrieb. |

**Immer inklusive:** `SHA256SUMS-<Version>.txt`, `update-manifest.json` und
`update-manifest.json.sig` — siehe [Integrität prüfen](#integritaet).

> **Empfehlung:** Immer direkt auf die neueste Version aktualisieren.
> Ältere Releases bleiben zum Nachlesen erhalten, sind aber nicht mehr empfohlen.

<details>
<summary><b>Warum keine Pakete über Windows Store oder Google Play?</b></summary>

Enigma 3 verteilt sich ausschließlich über dieses Repository. Ein
Store-Weg würde eine dritte Vertrauensstelle zwischen dich und deinen
Server setzen — und bei jedem Update eine Prüfung durch einen Anbieter.
Außerdem erlaubt ein Store-Vertrieb keine selbst gehostete Serveradresse
als gleichberechtigten Einstiegspunkt.

</details>

---

<a id="loslegen"></a>

## ⚡ In drei Schritten loslegen

<table>
<tr>
<td width="33%" align="center">

**1 · Server**
Ein laufender SecureChat-Server mit HTTPS.

[Server-Repo](https://git.jimmybones.de/jimmybones/securechat)

</td>
<td width="33%" align="center">

**2 · App**
Hier herunterladen und installieren.

[Downloads](#downloads)

</td>
<td width="33%" align="center">

**3 · Starten**
Serveradresse eintragen, anmelden, loslegen.

[Loslegen](#loslegen)

</td>
</tr>
</table>

Beim ersten Start trägst du nur `chat.example.com` ein. Alles Weitere
verschlüsselt die App auf deinem Gerät.

---

<a id="schutz"></a>

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
Tresor (Argon2id mit Gerätegeheimnis als Pepper). Android nutzt den
Keystore, Windows DPAPI.

### ⏳ Selbstlöschung
Du entscheidest, wie lange deine Nachrichten bleiben —
auf dem Server und auf jedem Gerät.

</td>
</tr>
</table>

**Kein Tracking. Kein Crash-Reporting. Kein Hintergrund-Download.**
Updates kommen ausschließlich aus diesem Repository.

---

<a id="integritaet"></a>

## 🔍 Integrität prüfen

```sh
sha256sum -c SHA256SUMS-<Version>.txt
```

**Automatische Updates:** Die Desktop-App prüft jedes Update gegen zwei
Sicherheitsstufen:

1. Eine **Ed25519-Signatur** (`update-manifest.json` und `update-manifest.json.sig`
   im Release). Die App hat den Absendeschlüssel eingebaut.
2. Die **SHA-256-Prüfsumme** jeder Datei.

Ohne passende Signatur bietet die App kein Update an.

<details>
<summary><b>Prüfsumme von Hand nachrechnen</b></summary>

```sh
# Windows (PowerShell)
Get-FileHash .\Enigma-3-Setup-<Version>.exe -Algorithm SHA256

# Linux / macOS
shasum -a 256 Enigma-3-<Version>-x86_64.AppImage
```

Vergleiche das Ergebnis mit der Zeile in `SHA256SUMS-<Version>.txt`.
Weicht es ab, installiere die Datei nicht und melde es in einem
[Sicherheitshinweis](SECURITY.md).

</details>

---

<a id="iphone"></a>

## 📱 iPhone und Web-App

Für iOS wird keine App über den App Store vertrieben. Stattdessen:

1. Im **Safari** `https://chat.example.com` öffnen.
2. Über **Teilen › Zum Home-Bildschirm** als Vollbildseite ablegen.
3. Wie eine App verwenden — Anmeldung, Anrufe und Benachrichtigungen laufen
   über die Web-App deines Servers.

Der Funktionsumfang entspricht der Web-App; Bildschirmfreigabe und
Hintergrund-Benachrichtigungen unterliegen den Grenzen von iOS.

---

<a id="faelle"></a>

## ❓ Häufige Fälle

<details>
<summary><b>Windows zeigt „Der Computer konnte diese App nicht überprüfen"</b></summary>

Der Installer ist bewusst unsigniert — ein Zertifikat wäre eine weitere
Vertrauensstelle, die man kaufen kann. Bestätige die Warnung nur, wenn
diese Seite die Quelle war, und prüfe die SHA-256-Prüfsumme.

</details>

<details>
<summary><b>Android: „App nicht installiert"</b></summary>

Eine vorhandene Debug-APK vorher deinstallieren — der Release-Schlüssel ist
ein anderer. Installation danach über „Unbekannte Quellen".

</details>

<details>
<summary><b>Update ohne Datenverlust</b></summary>

Neue Version einfach über die bestehende installieren. Es bleiben alle
Sitzungen, Einstellungen und Schlüssel erhalten.

</details>

<details>
<summary><b>Erster Start nach größerem Update</b></summary>

Ab Version **1.7.24** ist die PIN 8-stellig und am Desktop Pflicht.
Bestehende Tresore mit alter PIN entsperren weiterhin; beim nächsten Mal
bitte die neue Länge setzen.

</details>

---

<a id="kontakt"></a>

## 💬 Kontakt

| Thema | Weg |
| :--- | :--- |
| Fragen und Fehler | [**GitHub Issues**](https://github.com/JImmyB0nes/SecureChat-App/issues) |
| Sicherheitslücken | Vertraulich, siehe [SECURITY.md](SECURITY.md) |
| Server und Betrieb | [Server-Repo auf Forgejo](https://git.jimmybones.de/jimmybones/securechat) |
| Server-Quellcode | [CHANGELOG und Doku](https://git.jimmybones.de/jimmybones/securechat) |
