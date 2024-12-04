# Werbung mit Flipper

## Berufliches Gymnasium Technik  
**Tom Holland**  
**BGT221**  

---

## Erklärungen

BEIM CLONEN VOM GITHUB SIND ALLE DATIEN SCHON DRINNE - ORIGINAL UND ANGEPASST

### **BadUSB**
- **Funktion**: "Hackt" einen Computer:
  1. Öffnet ein "Ausführen"-Fenster.
  2. Startet die Eingabeaufforderung.
  3. Erstellt eine Editor-Datei mit Text + TBZ-Logo.
- **Hinweis**: Funktioniert nur auf **Windows**!

### **Evil-Portal**
- **Funktion**: Erstellt ein WLAN namens **"TBZ_guest"**. 
  - Ermöglicht das Einloggen, jedoch ohne echtes WLAN. 
  - Anmeldedaten werden auf dem Flipper angezeigt.
- **Hinweis**: Erinnert die Nutzer daran, **keine echten Daten** einzugeben!

---

## **Wichtige Hinweise**
- **Backups erstellen**: Vor jedem Versuch ein Backup machen, besonders bei Änderungen. Es kam häufig vor, dass aufwendige Projekte wie die Schranke neu erstellt werden mussten.

---

## **Nützliche Links**

### **BadUSB**  
(Siehe Firmware-Abschnitt und Dateien-Ordner für das spezielle TBZ-Logo.)

### **Evil-Portal**
- [Evil-Portal GitHub](https://github.com/bigbrodude6119/flipper-zero-evil-portal/tree/main?tab=readme-ov-file)
- [Grundlegendes Erklärungsvideo](https://www.youtube.com/watch?v=WPT7qeySf6g&t=337s)
- [Assets hinzufügen](https://github.com/bigbrodude6119/flipper-zero-evil-portal/releases)

### **Firmware**
1. [Firmware-Installation](https://github.com/DarkFlippers/unleashed-firmware/blob/dev/documentation/HowToInstall.md)
2. [Extra-Plugins](https://github.com/xMasterX/all-the-plugins#extra-pack)
3. [Firmware-Versionen](https://github.com/DarkFlippers/unleashed-firmware/releases)

---

## **Firmware**
- Updates über **QFlipper** setzen die Firmware automatisch auf die **originale Version** zurück.
- Unterschiedliche Firmware-Versionen bieten verschiedene Zusatzmodule (siehe Link 2.4).

| Kürzel  | Bedeutung                    |
|---------|------------------------------|
| **base apps** | Vorinstallierte Apps.        |
| **extra apps** | Zusätzliche Module.          |
| **rgb**        | Zusätzliche RGB-Funktion (nur modded, nicht für Schulflipper). |

---

## **Anleitung: BadUSB**
1. Base Apps oder offizielle Firmware updaten.
2. Siehe Dateien-Ordner für das spezielle TBZ-Logo.

---

## **Anleitung: Evil-Portal**

### **1. Dev Board einrichten**
1. **Wifi_dev_board.zip** herunterladen (siehe Link 2.2).  
2. FlipperLab öffnen:
   - Empfohlen: Chrome/Edge als Administrator.  
   - **Seriellen Port zulassen**: [Anleitung](https://support.google.com/chrome/answer/12576972?hl=de).
3. Dateien aus `wifi_dev_board.zip` hinzufügen:
   - `1000 - EvilPortal.ino.bootloader.bin`
   - `8000 - EvilPortal.ino.partitions.bin`
   - `e000 - boot_app0.bin`
   - `10000 - EvilPortal.ino.bin`

### **2. Flipper vorbereiten**
1. FlipperLab oder QFlipper öffnen.  
2. Firmware installieren:
   - **Download**: `unleashed-evil_portal.fap.zip`  
   - Datei entpacken und strukturieren:  
     ```
     apps/
       GPIO/
         evil_portal.fap
     apps_data/
       evil_portal/
     ```

### **3. Dateien anpassen**
1. `evil_portal_sd_folder.zip` herunterladen.  
2. Inhalte anpassen:
   - **ap.config.txt**: WLAN-Name ändern.  
   - **index.html**: Anzeige der Website (HTML/CSS anpassbar).  
3. Dateien in den Ordner `evil_portal` verschieben. oder von Github reinziehen

### **4. Evil-Portal starten**
- **Start**: Hotspot starten.  
  - Alle eingegebenen Daten werden angezeigt.  
- **Stop**: Hotspot stoppen.

---

## **Zusätzliche Hinweise**
- **Firmware zu alt?** Nicht einfach die neue installieren. Überprüfen, ob der richtige Buchstabe installiert ist.
